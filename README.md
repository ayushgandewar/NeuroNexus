<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Simple Google-Style Form</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f0f4f8;
      margin: 0;
      padding: 20px;
    }

    .form-container {
      background-color: #fff;
      max-width: 600px;
      margin: 40px auto;
      padding: 30px;
      border-radius: 10px;
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
    }

    h2 {
      text-align: center;
      margin-bottom: 20px;
      color: #333;
    }

    .form-group {
      margin-bottom: 15px;
    }

    label {
      display: block;
      margin-bottom: 5px;
      font-weight: bold;
      color: #333;
    }

    input[type="text"],
    input[type="tel"],
    input[type="email"],
    textarea,
    select {
      width: 100%;
      padding: 10px;
      border: 1px solid #ccc;
      border-radius: 6px;
      font-size: 14px;
      box-sizing: border-box;
    }

    textarea {
      resize: vertical;
      min-height: 80px;
    }

    .radio-group {
      display: flex;
      gap: 15px;
      margin-top: 5px;
    }

    .radio-group label {
      font-weight: normal;
    }

    .submit-button {
      background-color: #1a73e8;
      color: white;
      border: none;
      padding: 12px 20px;
      font-size: 16px;
      border-radius: 6px;
      cursor: pointer;
      width: 100%;
    }

    .submit-button:hover {
      background-color: #1669c1;
    }
  </style>
</head>
<body>

  <div class="form-container">
    <h2>Contact Information Form</h2>
    <form>
      <div class="form-group">
        <label for="fullName">Full Name</label>
        <input type="text" id="fullName" name="fullName" required />
      </div>

      <div class="form-group">
        <label for="contactNumber">Contact Number</label>
        <input type="tel" id="contactNumber" name="contactNumber" required />
      </div>

      <div class="form-group">
        <label for="address">Address</label>
        <textarea id="address" name="address" required></textarea>
      </div>

      <div class="form-group">
        <label for="company">Company Name</label>
        <input type="text" id="company" name="company" />
      </div>

      <div class="form-group">
        <label for="email">Email Address</label>
        <input type="email" id="email" name="email" required />
      </div>

      <div class="form-group">
        <label for="department">Department</label>
        <select id="department" name="department" required>
          <option value="">Select</option>
          <option value="HR">HR</option>
          <option value="Sales">Sales</option>
          <option value="Development">Development</option>
          <option value="Marketing">Marketing</option>
          <option value="Others">Others</option>
        </select>
      </div>

      <div class="form-group">
        <label>Gender</label>
        <div class="radio-group">
          <label><input type="radio" name="gender" value="Male" required /> Male</label>
          <label><input type="radio" name="gender" value="Female" /> Female</label>
          <label><input type="radio" name="gender" value="Prefer not to say" /> Prefer not to say</label>
        </div>
      </div>

      <button type="submit" class="submit-button">Submit</button>
    </form>
  </div>

</body>
</html>
