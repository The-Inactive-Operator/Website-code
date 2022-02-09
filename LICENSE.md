<!DOCTYPE html>
<html>
 <head>
  <title>M1.com</title>
  <style>
   :root {
    --bg-color: rgb(0, 0, 0);
    --typewriterSpeed: 3.5s;
    --typewriterCharacters: 25;
  }
  
  body {
    margin: 0;
    font-family: "Source Sans Pro";
    min-height: 100vh;
    display: grid;
    place-content: center;
    text-align: center;
    background: var(--bg-color);
  }  
  .subtitle {
    color: rgba(255, 255, 255, 0.883);
    font-size: 2rem;
    font-weight: 400;
    font-family: "Source Code Pro", monospace;
    opacity: 0;
    transform: translateY(3rem);
    animation: fadeInUp 1s ease calc(var(--typewriterSpeed) - 3s) forwards;
  }
  .subtitle2 {
    color: rgba(255, 255, 255, 0.883);
    font-size: 2rem;
    font-weight: 400;
    font-family: "Source Code Pro", monospace;
    opacity: 0;
    transform: translateY(3rem);
    animation: fadeInUp 1s ease calc(var(--typewriterSpeed) - 3.5s) forwards;
  }
  
  @keyframes fadeInUp {
    to {
      opacity: 1;
      transform: translateY(0);
    }
  }
  </style>
 </head>
 <body>
  <h1>Welcome to M1! Click below to renew your internet membership<h1>
  <p>An agent will get to you shortly. Please wait patiently.<p>
 </body>
</html>
