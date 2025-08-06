# NT-1: Student Registration Form with HTML5 Validation

## 🎯 Aim

To design and implement a basic student registration form using HTML5 that collects user information and performs client-side input validation.

---

## 📚 Theory

HTML5 introduces built-in form validation through specific attributes and input types, reducing the need for JavaScript. These include:

- `required`: Ensures the field must be filled.
- `type="email"`: Validates proper email format.
- `type="number"`: Restricts input to numerical values.
- `min`, `max`: Define number input boundaries.
- `pattern`: Supports custom regular expressions.
- `placeholder`: Offers helpful hints to the user.

These features improve **user experience** and ensure **data integrity** before submission.

---

## 🛠 Procedure

1. Create a new HTML file named `student-registration.html`.
2. Inside the `<body>`, add a `<form>` with input fields for:
   - Full Name
   - Email Address
   - Age
3. Apply HTML5 validation attributes like `required`, `type`, `min`, and `placeholder`.
4. Add a styled submit button.
5. Open the file in a web browser and test with different inputs.

---

## 💻 Code

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Student Registration Form</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 40px;
      background-color: #f2f2f2;
    }
    form {
      background-color: white;
      padding: 20px;
      border-radius: 8px;
      max-width: 400px;
      margin: auto;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    }
    input, label {
      display: block;
      margin-top: 10px;
      width: 100%;
    }
    input {
      padding: 8px;
      margin-top: 5px;
    }
    button {
      margin-top: 15px;
      padding: 10px;
      background-color: #4CAF50;
      border: none;
      color: white;
      font-size: 16px;
      cursor: pointer;
      width: 100%;
    }
    button:hover {
      background-color: #45a049;
    }
  </style>
</head>
<body>

  <form>
    <h2>Student Registration</h2>

    <label for="name">Full Name:</label>
    <input type="text" id="name" name="name" required placeholder="Enter your full name">

    <label for="email">Email Address:</label>
    <input type="email" id="email" name="email" required placeholder="example@email.com">

    <label for="age">Age:</label>
    <input type="number" id="age" name="age" required min="5" max="100" placeholder="Enter your age">

    <button type="submit">Register</button>
  </form>

</body>
</html>
