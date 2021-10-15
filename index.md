

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
    .light {

        background-color: turquoise;
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
<body class="light">
  
  

<button onclick="window.location.href = 'test.html';" class="button"><span>Players </span></button>
<button style="background-color: #1e2cf4;" class="button"><span>Hover </span></button>
  
  
  
  
