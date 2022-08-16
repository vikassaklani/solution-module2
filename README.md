<!DOCTYPE html>
<html>
<head>

<title>Responsive Layout</title>
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="D:\project\css\style.css">

</head>
<body>
<h1>Our Menu</h1>
  <div class="col-lg-4 col-md-6 col-sm-12">
  	<div class="row">
  		<p class="box-name box1">Chicken</p>
  		<p class="box">Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
  		tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
  		quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
  		consequat.</p>
  	</div>
  </div>

  <div class="col-lg-4 col-md-6 col-sm-12">
  	<div class="row">
   		<p class="box-name box2">Beef</p>
   		<p class="box">Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
   		tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
   		quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
   		consequat. </p>
  	</div>
  </div>

  <div class="col-lg-4 col-md-12 col-sm-12">
  	<div class="row">
   		<p class="box-name box3">Sushi</p>
   		<p class="box">Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
   		tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
   		quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
   		consequat. </p>
  	</div>	
  </div>
</body>
</html>

* {
  box-sizing: border-box;
}

body{

	font-family: cursive;
}

h1 {
  text-align: center;
}

.row{
  width: 100%;
  overflow: none;
  margin-top: 3%;
  margin-bottom: 3%;
}

.box-name{
  overflow: none;
  text-align: center;
  border: 2px solid black;
  width: 100px;
  
  float: right;
  margin-right: 36px;
  margin-top: 0px;
  font-weight: bold;
  position: sticky;
}

.box{
  border: 3px solid black;
  width: 90%;
  margin: 2.5%;
  color: black
  font-size: 25px;
  padding: 2%;
  padding-top: 53px;
  background-color: grey;
}

.box1{
  background-color: darksalmon;
}

.box2{
  color: white;
  background-color: darkred;
}
.box3{
  background-color: palegoldenrod;
}
/********** Medium devices only **********/
@media (min-width: 768px) and (max-width: 991px) {
  .col-md-6,.col-md-12 {
    float: left;
  }
  .col-md-6 {
    width: 50%;
  }
  .col-md-12 {
    margin-left: -10px;
  }
  .box3{
    margin-right: 71px;
    width: 100px;
  }
  .row{
  	width:100%;
  }
}

@media (min-width: 0px) and (max-width: 767px) {
  .col-sm-12 {
  	float: left;
    width: 100%;
  }
  .box-name{
    margin-right: 50px;
    overflow: none;
  }
}
/********** Large devices only **********/
@media (min-width: 992px) {
  .col-lg-4 {
  	float: left;
    width: 33.33%;
  }
  .box-name{
  	margin-right: 37px;
  }
}
