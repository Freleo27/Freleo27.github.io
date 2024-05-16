<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>A Day in Puerto Rico</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background-color: #f0f0f0;
    }

    .container {
      max-width: 800px;
      margin: 50px auto;
      text-align: center;
    }

    input[type="text"] {
      padding: 10px;
      margin: 10px;
    }

    button {
      padding: 10px 20px;
      background-color: #007bff;
      color: #fff;
      border: none;
      cursor: pointer;
    }

    button:hover {
      background-color: #0056b3;
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>Welcome to One Day in Puerto Rico</h1>
    <input type="text" id="nameInput" placeholder="Enter your name">
    <button onclick="start()">Start!</button>
    <p id="greeting"></p>
  </div>

  <script>
    function start() {
      const nameInput = document.getElementById('nameInput');
      const greeting = document.getElementById('greeting');
      const name = nameInput.value.trim();

      if (name !== '') {
        greeting.textContent = 'Hello, ' + name + '!';
        // You can add code here to transition to the next section of the website
      } else {
        alert('Please enter your name.');
      }
    }
  </script>
</body>
</html>
