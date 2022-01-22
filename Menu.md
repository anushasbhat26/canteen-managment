# canteen-managment
<!DOCTYPE html>
<html>
<title>W3.CSS Template</title>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="https://www.w3schools.com/w3css/4/w3.css">
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Amatic+SC">
<style>
    body, html {height: 180%}
    body,h1,h2,h3,h4,h5,h6 {font-family: "Amatic SC", sans-serif}
    .menu {display: none}
</style>
<body>
    <!-- Menu Container -->
    <div class="w3-container w3-black w3-padding-64 w3-xxlarge" id="menu">
      <div class="w3-content">
      
        <h1 class="w3-center w3-jumbo" style="margin-bottom:64px">THE MENU</h1>
        <div class="w3-row w3-center w3-border w3-border-dark-grey">
          <a href="javascript:void(0)" onclick="openMenu(event, 'Snacks');" id="myLink">
            <div class="w3-col s4 tablink w3-padding-large w3-hover-red">Snacks</div>
          </a>
          <a href="javascript:void(0)" onclick="openMenu(event, 'Lunch');">
            <div class="w3-col s4 tablink w3-padding-large w3-hover-red">Lunch</div>
          </a>
          <a href="javascript:void(0)" onclick="openMenu(event, 'Drinks');">
            <div class="w3-col s4 tablink w3-padding-large w3-hover-red">Drinks</div>
          </a>
        </div>
    
        <div id="Snacks" class="w3-container menu w3-padding-32 w3-white">
          <h1><b>Lays</b> <span class="w3-right w3-tag w3-dark-grey w3-round">₹10</span></h1>
          <p class="w3-text-grey">tangy tomato </p>
          <hr>
       
          <h1><b>Doritos</b> <span class="w3-right w3-tag w3-dark-grey w3-round">₹10</span></h1>
          <p class="w3-text-grey">spicy sweet chilli</p>
          <hr>
          
          <h1><b>Kurkure</b> <span class="w3-right w3-tag w3-dark-grey w3-round">₹10</span></h1>
          <p class="w3-text-grey">masala munch</p>
          <hr>
    
          <h1><b>Lotte Choco Pie</b> <span class="w3-right w3-tag w3-dark-grey w3-round">₹10</span></h1>
          <p class="w3-text-grey"></p>
          <hr>

          <h1><b>Snickers </b> <span class="w3-right w3-tag w3-dark-grey w3-round">₹10</span></h1>
          <p class="w3-text-grey">choclate</p>
          <hr>

          <h1><b>Dairy Milk </b> <span class="w3-right w3-tag w3-dark-grey w3-round">₹10</span></h1>
          <p class="w3-text-grey">choclate</p>
          <hr>
        </div>

    
        <div id="Lunch" class="w3-container menu w3-padding-32 w3-white">
          <h1><b>Parota</b> <span class="w3-tag w3-grey w3-round"></span> <span class="w3-right w3-tag w3-dark-grey w3-round">₹50</span></h1>
          <p class="w3-text-grey"></p>
          <hr>
       
          <h1><b>Gobi Manchurain</b> <span class="w3-right w3-tag w3-dark-grey w3-round">₹50</span></h1>
          <p class="w3-text-grey"></p>
          <hr>
          
          <h1><b>Pulao</b> <span class="w3-right w3-tag w3-dark-grey w3-round">₹60</span></h1>
          <p class="w3-text-grey"></p>
          <hr>

          <h1><b>Fried Rice</b> <span class="w3-right w3-tag w3-dark-grey w3-round">₹60</span></h1>
          <p class="w3-text-grey"></p>
          <hr>

          <h1><b>Chapathi and Curry</b> <span class="w3-right w3-tag w3-dark-grey w3-round">₹60</span></h1>
          <p class="w3-text-grey"></p>
          <hr>
    
          <h1><b>Noodles</b> <span class="w3-right w3-tag w3-dark-grey w3-round">₹60</span></h1>
          <p class="w3-text-grey"></p>
        </div>
    


    
        <div id="Drinks" class="w3-container menu w3-padding-32 w3-white">
          <h1><b>Coke</b> <span class="w3-tag w3-grey w3-round"></span><span class="w3-right w3-tag w3-dark-grey w3-round">₹15</span></h1>
          <p class="w3-text-grey"></p>
          <hr>
       
          <h1><b>Sprite</b> <span class="w3-right w3-tag w3-dark-grey w3-round">₹15</span></h1>
          <p class="w3-text-grey"></p>
          <hr>
          
          <h1><b>Fanta</b> <span class="w3-right w3-tag w3-dark-grey w3-round">₹15</span></h1>
          <p class="w3-text-grey"></p>
          <hr>

          <h1><b>Fizz</b> <span class="w3-right w3-tag w3-dark-grey w3-round">₹15</span></h1>
          <p class="w3-text-grey"></p>
          <hr>
          
          <h1><b>7 UP</b> <span class="w3-right w3-tag w3-dark-grey w3-round">₹15</span></h1>
          <p class="w3-text-grey"></p>
          <hr>

          <h1><b>Mazza</b> <span class="w3-right w3-tag w3-dark-grey w3-round">₹15</span></h1>
          <p class="w3-text-grey"></p>
        </div><br>
    
      </div>
    </div>

    <script>
        // Tabbed Menu
        function openMenu(evt, menuName) {
          var i, x, tablinks;
          x = document.getElementsByClassName("menu");
          for (i = 0; i < x.length; i++) {
             x[i].style.display = "none";
          }
          tablinks = document.getElementsByClassName("tablink");
          for (i = 0; i < x.length; i++) {
             tablinks[i].className = tablinks[i].className.replace(" w3-red", "");
          }
          document.getElementById(menuName).style.display = "block";
          evt.currentTarget.firstElementChild.className += " w3-red";
        }
        document.getElementById("myLink").click();
     </script>
        
</body>  
</html>
  


