# game-4
<!DOCTYPE html>
<html lang="en_us">
<head> <meta charset="utf-8">
  <title>CrystalsCollector Game</title>
  
 <link href="game-4" ref="stylesheet" type="assets/css/resets.css"/>

  <link href="game-4" ref="stylesheet" type="assets/css/style.css"/>

<!-- Latest compiled and minified CSS -->
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" integrity="sha384-BVYiiSIFeK1dGmJRAkycuHAHRg32OmUcww7on3RYdg4Va+PmSTsz/K68vbdEjh4u" crossorigin="anonymous">



  <script
  src="https://code.jquery.com/jquery-3.2.1.js"
  integrity="sha256-DZAnKJ/6XZ9si04Hgrsxu/8s717jcIzLy3oi35EouyE="
  crossorigin="anonymous"></script>

</head>
 
 <body>

     <div class="container">
         <div class="jumbotron" style="background-color:#00F3FF">
     <h1>Crystals Collector</h1> 
       <div class="text-center">
        <button class="btn btn-warning btn-xs theme-button"><span class="glyphicon glyphicon-music"></span> Play Theme!</button>
        <button class="btn btn-default btn-xs pause-button"><span class="glyphicon glyphicon-pause"></span> Pause Song</button>
      </div>
  </div>
   <div class="instructions">
    <h3>Here's how you play the game</h3>
    </br>
     <ol> 
      <li>You will be given a random number at the start of the game.<span>"Number To Get"</span></li>
      <li>There are four crystals below.</li>
        <ul>
           
       </ul>
            <li>By clicking on a crystal, you will add a specific amount of points to your total score.</li>
           <li>You win the game by matching your total score to the random number.</li>
          <li>You lose the game if your total score goes above the random number.</li>
          <li>The value of each crystal is hidden from you until you click on it.</li>
          <li>Each time when the game starts, the game will change the values of each crystal.</li>
      </ol>
    </div>
     <div class="numberToMatch">
        <h2>Number To Get:
            <span id="randonNumber"></span>
       </h2>
    </div>
   <div class="winsAndLosses">
    <h2>Wins:
      <span id= "numberWins"></span>
      </br>
      Losses: 
      <span id= "numberLosses"></span>
    </h2>
  </div>
  <div class="gems" id="gemsbuttons">
      
      
         <img src="https://orig08.deviantart.net/c79f/f/2011/054/0/d/bejeweled_animated_gem_1_by_bedgear-d3a8yp4.gif" alt="" id="blue">
     

    <img src="http://orig03.deviantart.net/f451/f/2011/054/a/4/bejeweled_animated_gem_2_by_bedgear-d3a8yxl.gif" alt="" id="green"> 
    
  
    <img src="https://orig09.deviantart.net/34cd/f/2011/054/3/6/bejeweled_animated_gem_6_by_bedgear-d3a8z9m.gif" alt="" id="red">
   
  

    <img src="https://orig07.deviantart.net/e34a/f/2011/054/0/8/bejeweled_animated_gem_5_by_bedgear-d3a8z75.gif" alt="" id="yellow">
  
  
  <div class="userTotal">
    <h2>Your total score is:
      <span id="finalTotal"></span>
    </h2>
  </div>
   
           <style type="text/css">
             
             body{
              background: black;
             }
           </style>
 <script type="text/javascript">
   
  

   $(document).ready(function(){
       
  // generate music while playing my game
       var audioElement = document.createElement("audio");
      audioElement.setAttribute("src","assets/04 04 - I Kno (Peod By The Renegades).mp3");

      $("theme-button").on("click", function(){
        audioElement.play();
      });
      $(".pause-button").on("click", function() {
        audioElement.puse();

      });



        var crystal = {
  blue:
  {
    name: "Blue",
    value: 0
  },
  green:
  {
    name: "Green",
    value: 0
  },
  red:
  {
    name: "Red",
    value: 0
  },
  yellow:
  {
    name: "Yellow",
  
    value: 0
  }
};

var numberWins = 0;
var numberLosses = 0;

var numberToMatch = 0;
var finalTotal = 0;

  $(document).ready(function(){
    // creates random numbers between 1-100
    document.getElementById("randonNumber").innerHTML = Math.floor(Math.random() * 100) + 1;
    // Prints random numbers on the DOM.

    var randNumber = Math.floor(Math.random() * 100 ) + 1;
      });

   });

    

var startGame = function() {


};



 </script>
         

     </body>
</html>
