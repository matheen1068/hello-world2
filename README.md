<!DOCTYPE html>
<html>
<head>
  <title>Sample Web App</title>
</head>
<body>
  <h1>Welcome to My Web App</h1>

  <form>
    <label for="name">Enter your name:</label>
    <input type="text" id="name" name="name" required>

    <button type="submit">Submit</button>
  </form>

  <div id="result"></div>

  <script>
    // Get the form element
    const form = document.querySelector('form');

    // Add an event listener for form submission
    form.addEventListener('submit', function(event) {
      event.preventDefault(); // Prevent form submission

      // Get the entered name
      const name = document.querySelector('#name').value;

      // Display the result
      const resultDiv = document.querySelector('#result');
      resultDiv.textContent = 'Hello, ' + name + '! Welcome to the web app.';
    });
  </script>
</body>
</html>
