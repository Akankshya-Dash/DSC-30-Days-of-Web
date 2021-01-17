# Project 4: Complete both the projects

### **First project**
- Make a TODO List website using everything you have learnt so far. 
<!DOCTYPE html> 
<html lang="en" dir="ltr"> 

<head> 
	<meta charset="utf-8"> 
	<title>TODO LIST</title>
	<link rel="stylesheet" href="style.css"> 

	<!-- Latest compiled and minified CSS -->
	<link rel="stylesheet" href= 
"https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/css/bootstrap.min.css"> 
</head> 
<body> 
	<div class="container"> 
		<h1 class="row"> 

		TODO LIST 

		</h1> 
		<br/><br/> 
		<div class="row"> 
			<form class="form-inline col-sm-offset-3"> 
				<div class="input-group"> 
					<span class="input-group-addon"> 
					<i class="glyphicon glyphicon-pencil"></i> 
					</span> 
					<input type="text" class="form-control"
						placeholder="todo-item"
						id="box" style="width: 30vw" /> 
				</div> 
				<div class="form-group"> 
					<input type="button"
						class="btn btn-primary form-control"
						value="add" style="width: 10vw"
						onclick="add_item()" /> 
				</div> 
			</form> 
		</div> 
		<div class="row"> 
			<ul id="list_item"> 
			</ul> 
		</div> 
	</div> 
    <script type="text/javascript" src="main.js">
    // Function called while clicking add button 
function add_item()
 { 

// Getting box and ul by selecting id; 
let item = document.getElementById("box"); 
let list_item = document.getElementById("list_item"); 
if(item.value != ""){ 

    // Creating element and adding value to it 
    let make_li = document.createElement("LI"); 
    make_li.appendChild(document.createTextNode(item.value)); 

    // Adding li to ul 
    list_item.appendChild(make_li); 

    // Reset the value of box 
    item.value=""

    // Delete a li item on click 
    make_li.onclick = function(){ 
        this.parentNode.removeChild(this); 
    } 


else{ 

    // Alert msg when value of box is "" empty. 
    alert("plz add a value to item"); 
} 


    </script> 
</body> 
</html> 


### **Second Project**
- Add to your portfolio:-
  * Save contact form details in a variable, Tabular structure with flex boxes.
  * For each entry, create a new row with the details entered.
  * Do not allow repeated or empty fields.
  * Whenever they enter a new thing, it will have a small fade in effect.
  * Animations and functionalities.

  <html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@4.5.3/dist/css/bootstrap.min.css" integrity="sha384-TX8t27EcRE3e/ihU7zmQxVncDAy5uIKz4rEkgIXeMed4M0jlfIDPvg6uqKI2xXr2" crossorigin="anonymous">

    <title>Save the world</title>
</head>
<body>

    <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
        <a class="navbar-brand" href="#">Overview</a>
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
      
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
          <ul class="navbar-nav mr-auto">
            <li class="nav-item active">
              <a class="nav-link" href="#">Home <span class="sr-only">(current)</span></a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">Link</a>
            </li>
            <li class="nav-item dropdown">
              <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                see options
              </a>
              <div class="dropdown-menu" aria-labelledby="navbarDropdown">
                <a class="dropdown-item" href="#">stuff1</a>
                <a class="dropdown-item" href="#">stuff2</a>
                <div class="dropdown-divider"></div>
                <a class="dropdown-item" href="#">again some stuff</a>
              </div>
            </li>
            <li class="nav-item">
              <a class="nav-link disabled" href="#" tabindex="-1" aria-disabled="true">Disabled</a>
            </li>
          </ul>
          <form class="form-inline my-2 my-lg-0">
            <input class="form-control mr-sm-2" type="search" placeholder="Search" aria-label="Search">
            <button class="btn btn-outline-success my-2 my-sm-0" type="submit">Search</button>
          </form>
        </div>
      </nav>
    <h2>Avengers</h2>
    <form action="">
      <br>
        <label for="">NAME :</label><input type="text" name="fname" id=""><br><br>
        <label for="">SUPERPOWER :</label> <input type="text" name="" id=""><br><br>
        <label for="">EMAIL ID :</label><input type="email" name="" id=""><br><br>
        <label for="">CONTACT NO. :</label><input type="number" name="" id=""><br><br>
        <button type="submit">Submit</button>
    </form>
    <br><br>
    <table>
        <tr>
            <th>Name</th>
            <th>City</td>
            <th>Age</th>
        </tr>
        <tr>
            <td>Tony Stark</td>
            <td>US</td>
            <td>48</td>
        </tr>
    </table>
    <br><br>
    <video width="600px" controls>
        <source src="./mylivewallpapers.com-Zombie-Invasion.mp4" type="video/mp4">
        Your browser does not support HTML video.
    </video>
    <br><br>
    <img style="width: 430px; height: 200px;" src="C:\Users\akank\Desktop\532d0341186be12412c6a4362cc08710.jpg" alt="Avengers' logo pic">
    <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js" integrity="sha384-DfXdz2htPH0lsSSs5nCTpuj/zy4C+OGpamoFVy38MVBnE+IbbVYUew+OrCXaRkfj" crossorigin="anonymous"></script>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@4.5.3/dist/js/bootstrap.bundle.min.js" integrity="sha384-ho+j7jyWK8fNQe+A12Hb8AhRq26LrZ/JpcUGGOn+Y7RsweNrtN/tE3MoK7ZeZDyx" crossorigin="anonymous"></script>
    <form>
      <ul class="flex-outer">
   
        <li>
          <label .flex-outer li p {
            flex: 1 0 120px;
            max-width: 220px;
          }for="first-name">First Name</label>
          <input type="text" id="first-name" placeholder="Enter your first name here">
         
        </li>
        <li>
          <label .flex-outer li p {
            flex: 1 0 120px;
            max-width: 220px;
          }
            for="last-name">Last Name</label>
          <input type="text" id="last-name" placeholder="Enter your last name here">
        </li>
        <li>
          <label .flex-outer li p {
            flex: 1 0 120px;
            max-width: 220px;
          }
            for="email">Email</label>
          <input type="email" id="email" placeholder="Enter your email here">
        </li>
        <li>
          <label for="phone">Phone</label>
          <input type="tel" id="phone" placeholder="Enter your phone here">
        </li>
        <li>
          <label for="message">Message</label>
          <textarea rows="6" id="message" placeholder="Enter your message here"></textarea>
        </li>
        <li>
          <p>Age</p>
          <ul class="flex-inner">
            <li>
              <input type="checkbox" id="twenty-to-twentynine">
              <label .flex-inner {
                flex: 1 0 220px;
              } for="twenty-to-twentynine">20-29</label>
            </li>
            <li>
              <input type="checkbox" id="thirty-to-thirtynine">
              <label for="thirty-to-thirtynine">30-39</label>
            </li>
          </ul>
        </li>
        <li>
          <button .flex-outer li button {
            margin-left: auto;
            padding: 8px 16px;
            border: none;
            background: #333;
            color: #f2f2f2;
            text-transform: uppercase;
            letter-spacing: .09em;
            border-radius: 2px;
          }  type="submit">Submit</button>
        </li>
      </ul>
    </form>


  </body>

<footer style="position: fixed;bottom: 1px;">Copyright All rights reserved</footer>
</html>


  