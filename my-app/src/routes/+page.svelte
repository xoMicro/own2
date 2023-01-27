<script>
    let count = 0;
    let imageUrl = "a8569jQ_460s.jpg";
  
    function increment() {
      count++;
    }
  
    function decrement() {
      if (count > 0) {
        count--;
      }
    }
  </script>
  <div class="counter-container">
    <button class="counter-button" on:click={decrement}>-</button>
    <div class="counter-display">{count}</div>
    <button class="counter-button" on:click={increment}>+</button>
    <div class="my-element">...</div>
  </div>
  <img src="a8569jQ_460s.jpg" alt="" class="my-image-class">
  <style>
    .counter-container {
      display: flex;
      align-items: center;
      justify-content: center;
      position: absolute;
      top: 10%;
      left: 43%;
      transform: translate(-50%, -50%);
    }
  
    .counter-button {
      width: 40px;
      height: 40px;
      font-size: 20px;
      font-weight: bold;
      background-color: #333;
      color: white;
      border: none;
    }
    :global(body) {
      background-image: url("w1200h1200.jpg");
      background-repeat: no-repeat;
      background-color: black;
    
    }

    .my-image-class {
    width: 255px;
    height: 900px;
    position: relative;
    left: 82.5%;
    
    
}

    
  
    .counter-display {
      font-size: 30px;
      margin: 0 20px;
      color: #333;
      background-color: #fff;
      padding: 10px 20px;
      border-radius: 50%;
      transition: all 0.2s ease-in-out;
    }
  </style>