<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Review Cards Assignment</title>
  <style>
    body {
      margin: 0;
      font-family: 'Calibri';
      overflow: hidden;
    }
    header {
      width: 100%;
      height: 10vh;
      overflow: hidden;
      position: relative;
      font-weight: bold;
      text-align: center;
           }
    .color-block {
      width: 100%;
      height: 100%;
      background-color: #740001;
      position: absolute;
      top: 0;
      left: 0;
      animation: colorBlockAnimation 3s forwards;
    }
    div {
      width: 100%;
      height: 100%;
      display: flex;
      align-items: center;
      justify-content: center;
    }
    div p {
      margin: 0;
      color: #eeba30; 
      font-size: 60px; 
      animation: myAnimation 3s 1 forwards, colorChange 5s 1s infinite;
      position: relative;
      z-index: 1; 
    }
    @keyframes myAnimation {
      0% {
        font-size: 80px;
      }
      70% {
        font-size: 40px;
      }
      100% {
        font-size: 20px;
      }
    }
    @keyframes colorBlockAnimation {
      0% {
        transform: scaleX(0);
      }
      100% {
        transform: scaleX(1);
      }
    }
    @keyframes colorChange {
      0% {
        background-color: #740001; 
        color: #eeba30; 
	width: 100%
      }
      50% {
        background-color: #ae0001; 
        color: #f0c75e; 
	width: 100%	
      }
      100% {
        background-color: #d3a625; 
        color: #372e29; 
	width: 100%
	   }
    }
    .card-container {
      display: flex;
      flex-wrap: wrap;
      justify-content: space-around;
      margin-top: 20px;
    }
     card {
      position: relative;
      width: 200px;
      height: 200px;
      background-color: #740001; 
      color: #eeba30; 
      border: solid;
      border-width: 6px;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      font-size: 16px;
      font-weight: bold;
      cursor: pointer;
      margin: 10px;
      transition: transform 1s, color 1s, background-color 1s; 
    }
    .card:hover {
      transform: rotateY(180deg);
      color: #372e29; 
      background-color: #eeba30; 
    }
    .question,
    .answer {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      text-align: center;
      width: 100%;
      transition: opacity 1s; 
    }
    .card:hover .question {
      opacity: 0;
    }
    .answer {
  	display: none;
  	color: #372e29; 
  	transform: translateX(-50%) rotateY(180deg); 
  	text-align: center; 
  	transition: transform 1s, opacity 1s; 
    }
    .card:hover .answer {
      display: block;
    }
  </style>
</head>
<body>
  <header>
    <div class="color-block"></div>
    <div>
      <p>Harry Potter Beasts Quizz</p>
    </div>
  </header>
  <div class="card-container">
    <div class="card">
      <div class="question">  What’s the name of Hagrid’s 3-headed dog that protects the Philosopher’s Stone?       </div>
      <div class="answer"> Fluffy </div>
    </div>
    <div class="card">
      <div class="question">  What type of animal is Hagrid’s pet, Buckbeak?  </div>
      <div class="answer">Hippogriff</div>
    </div>
    <div class="card">
      <div class="question">  What is a thestral?  </div>
      <div class="answer"> An invisible winged horse </div>
    </div>
    <div class="card">
      <div class="question">  What was the name of the Black family’s house elf?  </div>
      <div class="answer"> Kreacher </div>
    </div>
    <div class="card">
      <div class="question">  What was the name of the animal that acted as the snitch in early Quidditch games?         </div>
      <div class="answer">Golden Snidget</div>
    </div>
    <div class="card">
      <div class="question">  When unearthed,    a mandrake will do what?  </div>
      <div class="answer">Scream</div> 
    </div>
    <div class="card">
      <div class="question">  Cedric Diggory faced what breed of dragon in the Triwizard Tournament?  </div>
      <div class="answer">Swedish Short-Snout</div>
    </div>
    <div class="card">
      <div class="question">  What’s the name of the gigantic spider that almost killed Harry, Ron and Fang in       the Forbidden Forest?  </div>
      <div class="answer"> Aragog </div>
    </div>
    <div class="card">
      <div class="question">  The tears of which animal are the only known antidote to basilisk venom?   </div>
      <div class="answer"> Phoenix </div>
    </div>
    <div class="card">
      <div class="question">  What are names of all 4 centaurs in the Harry Potter books?  </div>
      <div class="answer">  Bane // Firenze // Magorian // Ronan </div>
    </div>
  </div>
</body>
</html>
