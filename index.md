


<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
  <style>
    .light {

        background-color: turquoise;
    }
    .dark {

background-color: rgb(224, 69, 64);
}
    .centre{
        display: flex;
        justify-content: center;
    }


    
</style>
  
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/1.12.0/jquery.min.js"></script>
    <script>
    $(document).ready(function(){
        table = $("#Players"); //set table name
        search_field = new Object();
        ///we create it as an object, initially empty
        $('.search-key').on('change keyup paste', function () {
            search_field['Position']      = $( "#Position" ).val();
            search_field['lastname']  = $("#lastname").val();
            search_field['Age']    =   $("#Age").val(); 

            table.find('tr').not(':first').each(function () {
                current_row = $(this); //keep track of the row being checked, iterate through it's cells
                var display = 0;
                current_row.show();
                $(this).find('td').each(function() {
                //when we stumble upon the data used as a search criteria
                    cell_value = $(this).html(); //gets the value of the cell being checked
                    if (cell_value == search_field[this.id] || search_field[this.id] == '') {
                        display++;    
                    }
                });
                if (display < 3) {
                    current_row.hide(); //if this cell is a match, or we no longer want to use it as a search criteria, the row is displayed
                }
            });

        });   
    });
    </script>
</head>
<body class="light">
  <div class="centre">
  
    <input list="Positions" id="Position" class="search-key" placeholder="Position">
    <datalist  id="Positions">
      <option value="CB">
      <option value="GK">
      <option value="ST">
    </datalist> 
  
  
    <input type="text" id="lastname" class="search-key" placeholder="lastname">
    <input type="number" id="Age" class="search-key" placeholder="Age">
  </div>
    <div class="centre">
    <p></p>
    <table border="5"
    cellspacing="15"
     id="Players">
        <tr>
            <th class="dark">Position </th>
            <th> Lastname </th> 
            <th> Age</th>
            <th> Contact </th>
            <th> Link </th>
        </tr>
        <tr>
            <td id="Position">CB</td>
            <td id="lastname">Arambarri</td> 
            <td id="Age">25</td>
            <td id="Contact">Alonso</td>
            <td> <a href="Arambarri.html"> <img src="pls.jpg" height="20" width="30"/> </td>
        </tr>

        <tr>
            <td id="Position">GK</td>
            <td id="lastname">Lynd</td> 
            <td id="Age">27</td>
        </tr>
        <tr>
            <td id="Position">ST</td>
            <td id="lastname">Mathis</td> 
            <td id="Age">25</td>
        </tr>
