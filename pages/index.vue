<template>
  <head>
    <meta charset="UTF-8">
  </head>
  <body id="index">
    <h1>Galaxy Raiders</h1>
    <h2>EP3 - TecProg2 - 2023</h2>
    <div id="buttons">
      <button>Start Game</button>
      <button>Leatherboard</button>
      <button>Quit</button>
    </div>
  </body>
</template>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Tektur&display=swap');
  @import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@200&family=Tektur&display=swap');
  #index
  {
    background-color: #010507;
  }
  h1
  {
    color: white;    
    text-align: center;
    font-family: Tektur;
    margin-top: 15%;
    margin-bottom: 2%;
    font-size: 60pt;
  }
  h2 {
    font-family: Montserrat;
    color: white;
    text-align: center;
    margin-bottom: 5%;
    font-size: 20pt;
    text-transform: uppercase;
  }
  #buttons
  {
    margin-left: auto;
    margin-right: auto;
    display: table;

  }
  button
  {
    background: none;
    border-color: white;
    color: white;
    padding: 20px 50px;
    margin-right: 20px;
    transition-duration: 0.4s;
    font-size: 15pt;
    border-style: double;
    font-family: Montserrat;
    text-transform: uppercase;
    font-weight: bold;
  } 
  button:hover
  {
    background-color: white;
    color: black;
  }
  button:active
  {
    background-color: rgba(0, 18, 44, 0.616);
    color: white;
  }
</style>