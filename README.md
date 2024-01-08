<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Registration Form</title>
  <style>
    body {
      font-family: bold;
      background-color: #f4f4f4;
      margin: 0;
      padding: 0;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
    }

    form {
      background-color: #fff;
      padding: 20px;
      border-radius: 8px;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    }

    label {
      display: block;
      margin-bottom: 8px;
    }

    input {
      width: 100%;
      padding: 8px;
      margin-bottom: 16px;
      box-sizing: border-box;
    }

    button {
      background-color: #4caf50;
      color: #fff;
      padding: 10px 20px;
      border: none;
      border-radius: 4px;
      cursor: pointer;
      font-size: 16px;
    }
  </style>
</head>
<body>

  <form action="#" method="post">
    <label for="username">Username:</label>
    <input type="text" id="username" name="username" required>

    <label for="email">Email:</label>
    <input type="email" id="email" name="email" required>

    <label for="phone">Phone Number:</label>
    <input type="tel" id="phone" name="phone" pattern="[0-9]{10}" title="Phone number must contain exactly 10 digits" required>

    <label>Gender:</label>
    <div>
      <input type="radio" id="male" name="gender" value="male"   required>
      <label for="male">Male</label>
    </div>
    <div>
      <input type="radio" id="female" name="gender" value="female" required>
      <label for="female">Female</label>
    </div>
    

    <label for="password">Password (exactly 10 numbers):</label>
    <input type="password" id="password" name="password" pattern="[0-9]{10}" title="Password must contain exactly 10 numbers" required>

    
    <button type="submit">Register</button>
  </form>
</body>
</html>
