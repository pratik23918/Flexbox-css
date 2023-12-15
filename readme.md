flexbox
-> by default flex dirn is row 
->flex is divided into categories
1. main axis- along the row left to roght 
2. cross axis - along the column top to bottom
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Flex Direction</title>
  <!-- HINT:
  https://developer.mozilla.org/en-US/docs/Web/CSS/Universal_selectors
  https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Selectors/Combinators 
  -->
  <style>
    .container {
      color: black;
      border: 5px solid gold;
      display: inline-flex;
      flex-direction: column;
    }
    .container>div{
     /* padding: 100px; */
     flex-basis:100px ;
    }
    

    /*
Select all the elements that are the direct
children of the .container class.
    */

    .red {background-color: #eb4d4b;}
    .orange {background-color: #f0932b;}
    .yellow {background-color: #f6e58d;}
    .green {background-color: #6ab04c;}
    .blue {background-color: #4834d4;}
    .indigo {background-color: #30336b;}
    .purple {background-color: #be2edd;}
  </style>
</head>

<body>
  <div class="container">
    <div class="red">Red</div>
    <div class="orange">Orange</div>
    <div class="yellow">Yellow</div>
    <div class="green">Green</div>
    <div class="blue">Blue</div>
    <div class="indigo">Indigo</div>
    <div class="purple">Purple</div>
  </div>
  
</body>

</html>
<!DOCTYPE html>
<html lang="en">

<!-- 
TODO: Change the background color for each device
[lightsalmon] Mobile Devices: 319px — 480px
[powderblue] iPads and Tablets: 481px — 1200px
[limegreen] Laptops: 1201px — 1600px
[seagreen] Desktops: 1601px and more
-->

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1, minimum-scale=1" />
  <title>Media Query</title>
  <style>
    body {
      background-color: aquamarine;
    }
    @media (min-width:319px) and (max-width:480px){
      body{
        background-color: lightsalmon;
      }
    }
    @media (min-width:481px) and (max-width:1200px){
     body{
      background-color: powderblue;
     }
     @media (min-width:1201px) and (max-width:1600px){
     body{
      background-color:limegreen;
     }
    }
    @media  (max-width:1601px){
     body{
      background-color:seagreen;
     }
    }

  </style>
</head>

<body>
</body>

</html>