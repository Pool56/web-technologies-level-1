# web-technologies-level-1
# Program 1: Display Personal Information
void main() 
    { String name = "John"; 
    int age = 25; 
    String school = "XYZ School";  
    String hobby = "Playing guitar"; 

    print("My name is $name. I am $age years old, studying at $school, and my hobby is $hobby."); 
} 
# Program 2: Perform Mathematical Operations with Functions
void main() {
  // Function to add two numbers
  int add(int a, int b) {
    return a + b;
  }
  
  // Function to multiply two numbers
  int multiply(int a, int b) {
    return a * b;
  }
  
  int num1 = 10;
  int num2 = 5;
  
  print("The sum of $num1 and $num2 is ${add(num1, num2)}");
  print("The product of $num1 and $num2 is ${multiply(num1, num2)}");

}
# Program 3: Determine Grade Based on Marks
void main() {
  int marks = 78;
  
  if (marks > 85) {
    print("Excellent");
  } else if (marks >= 75 && marks <= 85) {
    print("Very Good");
  } else if (marks >= 65 && marks < 75) {
    print("Good");
  } else {
    print("Average");
  }
}

# 2. WEB TECHNOLOGIES CSS


/* styles.css */

/* Task 1: Blue heading and red paragraph */
h1 {
  color: blue;
}

p {
  color: red;
  font-size: 15px;
}

/* Task 3: Green border on image */
.image-section img {
  width: 500px;
  height: 500px;
  border: 2px solid green;
}

/* Task 4: Form styling */
form {
  margin-top: 20px;
}

fieldset {
  margin-bottom: 10px;
}

input[type="text"],
input[type="email"],
input[type="tel"],
input[type="password"],
select {
  width: 100%;
  padding: 8px;
  margin-bottom: 10px;
}

input[type="radio"],
input[type="checkbox"] {
  margin-right: 5px;
}

input[type="submit"],
input[type="button"] {
  padding: 10px 20px;
  background-color: #4CAF50;
  color: white;
  border: none;
  cursor: pointer;
}

input[type="submit"]:hover,
input[type="button"]:hover {
  background-color: #45a049;
}

input[type="reset"] {
  padding: 10px 20px;
  background-color: #f44336;
  color: white;
  border: none;
  cursor: pointer;
}

input[type="reset"]:hover {
  background-color: #da190b;
}
# HTML
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Web Technologies Level 1 Hackathon</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>

  <!-- Task 1: Basic HTML structure -->
  <header>
    <h1>Web Technologies Hackathon</h1>
  </header>

  <!-- Task 2: Link to an external resource -->
  <a href="https://example.com" target="_blank">Visit Example</a>

  <!-- Task 3: Section with image -->
  <section class="image-section">
    <img src="path/to/your/image.jpg" alt="Image Description">
  </section>

  <!-- Task 4: Form -->
  <section class="form-section">
    <form action="#" method="post">
      <fieldset>
        <label for="name">Name:</label>
        <input type="text" id="name" name="name" required>
      </fieldset>
      <fieldset>
        <label for="email">Email Address:</label>
        <input type="email" id="email" name="email" required>
      </fieldset>
      <fieldset>
        <label for="phone">Phone Number:</label>
        <input type="tel" id="phone" name="phone" required>
      </fieldset>
      <fieldset>
        <label for="age">Age:</label>
        <input type="number" id="age" name="age" required>
      </fieldset>
      <fieldset>
        <legend>Gender:</legend>
        <label for="male"><input type="radio" id="male" name="gender" value="male"> Male</label>
        <label for="female"><input type="radio" id="female" name="gender" value="female"> Female</label>
      </fieldset>
      <fieldset>
        <label for="subjects">Subjects:</label>
        <select id="subjects" name="subjects[]" multiple required>
          <option value="English">English</option>
          <option value="Math">Math</option>
          <option value="Science">Science</option>
          <option value="Art and Craft">Art and Craft</option>
          <option value="Agriculture">Agriculture</option>
          <option value="Geography">Geography</option>
          <option value="History">History</option>
        </select>
      </fieldset>
      <fieldset>
        <label for="password">Password:</label>
        <input type="password" id="password" name="password" required>
      </fieldset>
      <input type="hidden" id="sessionId" name="sessionId" value="your_session_id_here">
      <fieldset>
        <input type="button" value="Cancel" onclick="clearForm()">
        <input type="submit" value="Register">
      </fieldset>
    </form>
  </section>

  <script>
    function clearForm() {
      document.querySelector('form').reset();
    }
  </script>

</body>
</html>


