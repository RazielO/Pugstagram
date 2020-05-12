<style>
  .container {
    width: 75%;
    display: flex;
    justify-content: space-evenly;
    padding: 25%;
  }

  .dot {
    background-color: black;
    height: 50px;
    width: 50px;
    border-radius: 50%;
    animation: load 1s infinite;
    position: relative;
  }

  #dot-1 {
    animation-delay: 0;
  }

  #dot-2 {
    animation-delay: 0.3s;
  }

  #dot-3 {
    animation-delay: 0.6s;
  }

  @keyframes load {
    0% {
      opacity: 1;
      top: 0px;
    }
    50% {
      opacity: 0.5;
      top: 10px;
    }
    100% {
      opacity: 1;
      top: 0px;
    }
  }
</style>

<div class="Loading">
  <div class="container">
    <div class="dot" id="dot-1" />
    <div class="dot" id="dot-2" />
    <div class="dot" id="dot-3" />
  </div>
</div>
