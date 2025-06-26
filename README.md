<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Responsive Login Page</title>
  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }

    body, html {
      height: 100%;
    }

    body {
      background: linear-gradient(to right, rgba(0,0,0,0.6), rgba(0,0,0,0.6)), 
                  url('https://images.unsplash.com/photo-1517245386807-bb43f82c33c4?auto=format&fit=crop&w=1650&q=80') no-repeat center center/cover;
      display: flex;
      justify-content: center;
      align-items: center;
    }

    .login-container {
      background-color: rgba(255, 255, 255, 0.95);
      padding: 40px 30px;
      border-radius: 10px;
      width: 100%;
      max-width: 400px;
      box-shadow: 0 0 20px rgba(0,0,0,0.3);
    }

    .login-container h2 {
      text-align: center;
      margin-bottom: 25px;
      color: #333;
    }

    .form-group {
      margin-bottom: 20px;
    }

    .form-group label {
      display: block;
      margin-bottom: 6px;
      font-weight: bold;
      color: #333;
    }

    .form-group input {
      width: 100%;
      padding: 12px;
      border-radius: 6px;
      border: 1px solid #ccc;
      transition: 0.3s;
    }

    .form-group input:focus {
      border-color: #4a90e2;
      outline: none;
    }

    .btn-login {
      width: 100%;
      padding: 12px;
      background-color: #4a90e2;
      border: none;
      color: white;
      font-weight: bold;
      font-size: 16px;
      border-radius: 6px;
      cursor: pointer;
      transition: background 0.3s;
    }

    .btn-login:hover {
      background-color: #357ABD;
    }

    .footer-text {
      text-align: center;
      margin-top: 15px;
      font-size: 14px;
      color: #555;
    }

    @media (max-width: 480px) {
      .login-container {
        padding: 30px 20px;
      }

      .login-container h2 {
        font-size: 22px;
      }
    }
  </style>
</head>
<body>

  <div class="login-container">
    <h2>Login to Your Account</h2>
    <form>
      <div class="form-group">
        <label for="email">Email Address</label>
        <input type="email" id="email" placeholder="Enter your email" required>
      </div>
      <div class="form-group">
        <label for="password">Password</label>
        <input type="password" id="password" placeholder="Enter your password" required>
      </div>
      <button type="submit" class="btn-login">Login</button>
    </form>
    <p class="footer-text">Don't have an account? <a href="#" style="color:#4a90e2; text-decoration:none;">Sign up</a></p>
  </div>

</body>
</html>
