

<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
.button {
  border-radius: 4px;
  background-color: #f4511e;
  border: none;
  color: #FFFFFF;
  text-align: center;
  font-size: 28px;
  padding: 20px;
  width: 200px;
  transition: all 0.5s;
  cursor: pointer;
  margin: 5px;
}

.button span {
  cursor: pointer;
  display: inline-block;
  position: relative;
  transition: 0.5s;
}

.button span:after {
  content: '\00bb';
  position: absolute;
  opacity: 0;
  top: 0;
  right: -20px;
  transition: 0.5s;
}

.button:hover span {
  padding-right: 25px;
}

.button:hover span:after {
  opacity: 1;
  right: 0;
}
body {
        background: #67B26F;  /* fallback for old browsers */
        background: -webkit-linear-gradient(to right, #4ca2cd, #67B26F);  /* Chrome 10-25, Safari 5.1-6 */
        background: linear-gradient(to right, #4ca2cd, #67B26F); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
        padding: 0;
        margin: 0;
        font-family: 'Lato', sans-serif;
        color: #000;
    }
    .new {

background-color: rgb(224, 69, 64);
}
    .centre{
        display: flex;
        justify-content: center;
    }


    
</style>
  
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/1.12.0/jquery.min.js"></script>
    
</head>
<body>
  
  

<button onclick="window.location.href = 'Playerlist.html';" class="button"><span>Players </span></button>
<button style="background-color: #1e2cf4;" onclick="window.location.href = 'teams.html';" class="button"><span>Youth </span></button>
  <button style="background-color: #1a9212" onclick="window.location.href = 'update.html';" class="button"><span>New </span></button>
  <button style="background-color: #1a9212" onclick="window.location.href = 'Requirements.html';" class="button"><span>New </span></button>
  
  
  
