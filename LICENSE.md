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
    cursor: url("https://s3-us-west-2.amazonaws.com/s.cdpn.io/9632/meh.png"), auto;
    
  }

  h1 {
    font-size: clamp(1rem, 3vw + 1rem, 4rem);
    position: relative;
    color: rgba(255, 255, 255, 0.883);
    font-family: "Source Code Pro", monospace;
    position: relative;
    width: max-content;
  }
  
  h1::before,
  h1::after {
    content: "";
    position: absolute;
    top: 0;
    right: 0;
    bottom: 0;
    left: 0;
  }
  
  h1::before {
    background: var(--bg-color);
    animation: typewriter var(--typewriterSpeed)
      steps(var(--typewriterCharacters)) 1s forwards;
  }
  
  h1::after {
    width: 0.125em;
    background: rgb(255, 255, 255);
    animation: typewriter var(--typewriterSpeed)
        steps(var(--typewriterCharacters)) 1s forwards,
      blink 750ms steps(var(--typewriterCharacters)) infinite;
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

  .socialIcon {
    color: rgb(255, 255, 255);
    font-size: xxx-large;
    animation: fadeInUp 1s ease calc(var(--typewriterSpeed) - 3s) forwards;
  }
  
  @keyframes typewriter {
    to {
      left: 100%;
    }
  }
  
  @keyframes blink {
    to {
      background: rgba(255, 255, 255, 0);
    }
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
