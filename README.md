# payment-form
<!DOCTYPE html>
<html>
<head>
  <title>Payment Form</title>
  <style>
    body {
      background-color: black;
      color: white;
      font-family: Arial, sans-serif;
    }

    .container {
      width: 400px;
      margin: 0 auto;
      padding: 20px;
      border: 1px solid #ccc;
      border-radius: 5px;
    }

    .container h1 {
      text-align: center;
    }

    .form-group {
      margin-bottom: 15px;
    }

    .form-group label {
      display: block;
      font-weight: bold;
    }

    .form-group input[type="text"],
    .form-group input[type="email"],
    .form-group select {
      width: 100%;
      padding: 10px;
      border: 1px solid #ccc;
      border-radius: 4px;
    }

    .form-group .card-group {
      display: flex;
    }

    .form-group .card-group label {
      margin-right: 10px;
    }

    .form-group .card-group input[type="radio"] {
      margin-right: 5px;
    }

    .form-group button {
      background-color: #4CAF50;
      color: white;
      padding: 10px 20px;
      border: none;
      border-radius: 4px;
      cursor: pointer;
      float: right;
    }

    .form-group button:hover {
      background-color: #45a049;
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>Payment Form</h1>
    <form>
      <div class="form-group">
        <label for="name">Name:</label>
        <input type="text" id="name" name="name" required>
      </div>

      <div class="form-group">
        <label for="email">Email:</label>
        <input type="email" id="email" name="email" required>
      </div>

      <div class="form-group">
        <label for="card-number">Card Number:</label>
        <input type="text" id="card-number" name="card-number" required>
      </div>

      <div class="form-group">
        <label for="expiry-date">Expiry Date:</label>
        <input type="text" id="expiry-date" name="expiry-date" required>
      </div>

      <div class="form-group">
        <label for="cvv">CVV:</label>
        <input type="text" id="cvv" name="cvv" required>
      </div>

      <div class="form-group">
        <label>Card Type:</label>
        <div class="card-group">
          <label>
            <input type="radio" name="card-type" value="visa" required> Visa
          </label>
          <label>
            <input type="radio" name="card-type" value="mastercard" required> Mastercard
          </label>
          <label>
            <input type="radio" name="card-type" value="amex" required> Amex
          </label>
        </div>
      </div>

      <div class="form-group">
        <button type="submit">Pay Now</button>
      </div>
    </form>
  </div>
</body>
</html>
