# jquery
<!DOCTYPE html>
<html>
<head>
  <title>jQuery Mobile Navbar with Icons</title>
  <link rel="stylesheet" href="https://code.jquery.com/mobile/1.4.5/jquery.mobile-1.4.5.min.css">
  <script src="https://code.jquery.com/jquery-1.11.3.min.js"></script>
  <script src="https://code.jquery.com/mobile/1.4.5/jquery.mobile-1.4.5.min.js"></script>
</head>
<!-- <script>
  $(document).on("pagecontainershow", function(event, ui) {
    var pageName = ui.toPage.attr("id");
    alert("You are on " + pageName);
  });
</script> -->
<body>
<!-- Homepage -->
<div data-role="page" id="home">
  <header data-role="header" data-theme="b">
    <h1>Mile Tracker</h1>
  </header>

  <div data-role="navbar">
    <ul>
      <li><a href="#home" data-icon="home" data-transition="slide">Home</a></li>
      <li><a href="#add" data-icon="plus" data-transition="slide">ADD</a>
      </li>
      <li><a href="#widgets" data-icon="arrow" data-transition="slide">widgets</a></li>
      <!-- <li><a href="#" data-icon="star">Favorites</a></li> -->
      <!-- <li><a href="#add" data-icon="plus">Add</a></li> -->
    </ul>
  </div>

  <div data-role="main" class="ui-content">
    <h3>Welcome to Mile Tracker</h3>
    <p>Track your running and Jogging details in this app</p>
    <h3>Your Latest Runs</h3>
    <ul id="stats" data-role="list-view" data-filter="true" data-filter-placeholder="Search Runs" data-inset="true"></ul>
    <br>
    <button id="clearruns" onclick="return confirm("Are You Sure")" data-theme="b">ClearRuns</button>
  </div>

  <footer data-role="footer" data-theme="b">
    <h4>Miletracker &copy;</h4>
  </footer>
</div>

<!-- AddPage -->


  <div data-role="page" id="add">
    <header data-role="header" data-theme="b">
      <h1>Mile Tracker</h1>
    </header>
  
    <div data-role="navbar">
      <ul>
        <li><a href="#home" data-icon="home">Home</a></li>
        <!-- <li><a href="#" data-icon="star">Favorites</a></li> -->
        <li><a href="#add" data-icon="plus">Add</a></li>
      </ul>
    </div>
  
    <div data-role="main" class="ui-content">
      <form id="add-form">
        <label for="addmiles">Enter Miles:</label>
        <input type="text" id="addmiles">
        <label for="AddDate">Enter AddDate:</label>
        <input type="text" id="AddDate" data-role="date" class="date" data-inline="true">
        <button id="submitadd" class="ui-btn ui-btn-b ui-btn-corner-all">Submit</button>
      </form>
    </div>
    
  
    <footer data-role="footer" data-theme="b">
      <h4>Miletracker &copy;</h4>
    </footer>
  </div>
  <div data-role="page" id="widgets">
    <div data-role="header">
      <h1>Layout Widgets</h1>
      <a href="#" class="ui-btn-right ui-btn ui-icon-grid ui-btn-icon-notext ui-corner-all">Menu</a>
    </div>
    
    <div data-role="panel" id="mypanel">
      <ul data-role="listview">
        <li><a href="#home">Home</a></li>
        <li><a href="#add">add 2</a></li>
        <li><a href="#widgets">Wids</a></li>
      </ul>
    </div>
    
  </div>



</body>
</html>
