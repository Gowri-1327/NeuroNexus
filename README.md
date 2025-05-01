<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Simple Web Form</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color:#00FFFF ;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
    }

    .form-container {
      background-color:  #FFB6C1;
      padding: 20px 30px;
      border-radius: 10px;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
      max-width: 400px;
      width: 100%;
    }

    .form-container h2 {
      text-align: center;
      margin-bottom: 20px;
    }

    label {
      display: block;
      margin-top: 15px;
      font-weight: bold;
    }

    input[type="text"],
    input[type="tel"],
    input[type="email"],
    select,
    textarea {
      width: 100%;
      padding: 8px;
      margin-top: 5px;
      border: 1px solid #ccc;
      border-radius: 5px;
      box-sizing: border-box;
    }

    textarea {
      resize: vertical;
    }

    .gender-options {
      margin-top: 5px;
    }

    .gender-options label {
      font-weight: normal;
      margin-right: 10px;
    }

    button[type="submit"] {
      margin-top: 20px;
      width: 100%;
      padding: 10px;
      background-color: #4CAF50;
      color: white;
      border: none;
      border-radius: 5px;
      font-size: 16px;
      cursor: pointer;
      transition: background-color 0.3s ease;
    }

    button[type="submit"]:hover {
      background-color: #45a049;
    }
  </style>
</head>
<body>
  <div class="form-container">
    <h2>Contact Form</h2>
    <form>
      <label for="fullname">Full Name</label>
      <input type="text" id="fullname" name="fullname" required>

      <label for="phone">Contact Number</label>
      <input type="tel" id="phone" name="phone" required>

      <label for="address">Address</label>
      <textarea id="address" name="address" rows="3" required></textarea>

      <label for="company">Company Name</label>
      <input type="text" id="company" name="company">

      <label for="email">Email Address</label>
      <input type="email" id="email" name="email" required>

      <label for="department">Department</label>
      <select id="department" name="department" required>
        <option value="">Select</option>
        <option value="HR">HR</option>
        <option value="Sales">Sales</option>
        <option value="Development">Development</option>
        <option value="Marketing">Marketing</option>
        <option value="Others">Others</option>
      </select>

      <label>Gender</label>
      <div class="gender-options">
        <label><input type="radio" name="gender" value="Male"> Male</label>
        <label><input type="radio" name="gender" value="Female"> Female</label>
        <label><input type="radio" name="gender" value="Prefer not to say"> Prefer not to say</label>
      </div>

      <button type="submit">Submit</button>
    </form>
  </div>
</body>
</html>
