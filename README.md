# f_code-

<!DOCTYPE html>
<html>
<head>
  <title>Login and Registration Page</title>
    <link rel ="stylesheet " href="m01.css">
  <style>
    /* CSS Styles */

    /* Step 2: Apply background image, set font-family, and text color */
    body {
      background-image: url('b.jpg');
      background-size: cover;
      font-family: Arial, sans-serif;
      color: #333;
    }

    /* Step 3: Style the heading */
    h1 {
      color: #fff;
      background-color: #333;
      padding: 10px;
      text-align: center;
    }

    /* Step 4: Style the option buttons container */
    .option-buttons {
      text-align: center;
      margin-bottom: 20px;
    }

    /* Step 5: Style the option buttons */
    .option-buttons button {
      padding: 10px 20px;
      margin: 0 10px;
      background-color: #333;
      color: #fff;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }

    /* Step 6: Style the active option button */
    .option-buttons button.active {
      background-color: #666;
    }

    /* Step 7: Style the form container */
    .form-container {
      width: 300px;
      margin: 0 auto;
      background-color: #f2f2f2;
      padding: 20px;
      border-radius: 5px;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    }

    /* Step 8: Hide the registration form initially */
    .form-container.hidden {
      display: none;
    }

    /* Step 9: Style the form labels */
    label {
      display: block;
      margin-bottom: 10px;
      font-weight: bold;
    }

    /* Step 10: Style the form inputs */
    input[type="text"],
    input[type="password"] {
      width: 100%;
      padding: 8px;
      margin-bottom: 20px;
      border-radius: 5px;
      border: 1px solid #ccc;
    }

    /* Step 11: Style the form submit button */
    input[type="submit"] {
      width: 100%;
      padding: 10px;
      background-color: #333;
      color: #fff;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }

    /* Step 12: Style the social media icons container */
    .social-media-icons {
      text-align: center;
      margin-top: 20px;
    }

    /* Step 13: Style the social media icons */
    .social-media-icons a {
      display: inline-block;
      margin: 5px;
    }

    /* Step 14: Style the social media icon images */
    .social-media-icons img {
      width: 30px;
    }
  </style>
  <script>
    // JavaScript function to show the selected form
    function showForm(formType) {
      const loginForm = document.getElementById('login-form');
      const registrationForm = document.getElementById('registration-form');
      const loginButton = document.getElementById('login-button');
      const registrationButton = document.getElementById('registration-button');

      if (formType === 'login') {
        loginForm.classList.remove('hidden');
        registrationForm.classList.add('hidden');
        loginButton.classList.add('active');
        registrationButton.classList.remove('active');
      } else if (formType === 'registration') {
        loginForm.classList.add('hidden');
        registrationForm.classList.remove('hidden');
        loginButton.classList.remove('active');
        registrationButton.classList.add('active');
      }
    }
  </script>
</head>
<body>
  <!-- Step 1: Create the login and registration page structure -->
  <h1>Lost and Found</h1>

  <div class="option-buttons">
    <!-- Step 15: Add button to switch to the login form -->
    <button id="login-button" class="active" onclick="showForm('login')">Login</button>
    <!-- Step 16: Add button to switch to the registration form -->
    <button id="registration-button" onclick="showForm('registration')">Registration</button>
  </div>

  <div class="form-container" id="login-form">
    <!-- Step 17: Create the login form -->
    <h2>Login</h2>
    <form>
      <!-- Step 18: Add input field for username -->
      <label for="username">Username:</label>
      <input type="text" id="username" name="username" required><br>

      <!-- Step 19: Add input field for password -->
      <label for="password">Password:</label>
      <input type="password" id="password" name="password" required><br>

      <!-- Step 20: Add submit button for login -->
      <input type="submit" value="Login">
    </form>

    <!-- Step 23: Add social media icons with links to admin's profiles -->
    <div class="social-media-icons">
      <a href="https://www.facebook.com/admin" target="_blank" title="Admin's Facebook">
        <img src="f.jfif" alt="Facebook">
      </a>
      <a href="https://www.twitter.com/admin" target="_blank" title="Admin's Twitter">
        <img src="t.png" alt="Twitter">
      </a>
      <a href="https://www.instagram.com/admin" target="_blank" title="Admin's Instagram">
        <img src="i.jfif" alt="Instagram">
      </a>
    </div>
  </div>

  <div class="form-container hidden" id="registration-form">
    <!-- Step 21: Create the registration form -->
    <h2>Registration</h2>
    <form>
      <!-- Step 22: Add input field for name -->
      <label for="name">Name:</label>
      <input type="text" id="name" name="name" required><br>

      <!-- Step 23: Add input field for email -->
      <label for="email">Email:</label>
      <input type="text" id="email" name="email" required><br>

      <!-- Step 24: Add input field for username -->
      <label for="username">Enrolment number:</label>
      <input type="text" id="username" name="username" required><br>

      <!-- Step 25: Add input field for password -->
      <label for="password">Password:</label>
      <input type="password" id="password" name="password" required><br>

      <!-- Step 26: Add submit button for registration -->
      <input type="submit" value="Register">
    </form>

    <!-- Step 27: Add social media icons with links to admin's profiles -->
    <div class="social-media-icons">
      <a href="https://www.facebook.com/admin" target="_blank" title="Admin's Facebook">
        <img src="f.jfif" alt="Facebook">
      </a>
      <a href="https://www.twitter.com/admin" target="_blank" title="Admin's Twitter">
        <img src="t.png" alt="Twitter">
      </a>
      <a href="https://www.instagram.com/admin" target="_blank" title="Admin's Instagram">
        <img src="i.jfif" alt="Instagram">
      </a>
    </div>
  </div>
</body>
</html>
