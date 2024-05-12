---
layout: single
title: "Submit your data"
permalink: /data/
---
<form id="userInfoForm">
  <label for="name">Name:</label>
  <input type="text" id="name" name="name" required><br>

  <label for="email">Email:</label>
  <input type="email" id="email" name="email" required><br>

  <label for="phone">Phone Number:</label>
  <input type="tel" id="phone" name="phone" required><br>

  <label for="password">Password:</label>
  <input type="password" id="password" name="password" required><br>

  <label for="age">Age:</label>
  <input type="number" id="age" name="age" required><br>

  <label for="blood-group">Blood Group:</label>
  <select id="blood-group" name="blood-group">
    <option value="A+">A+</option>
    <option value="A-">A-</option>
    <option value="B+">B+</option>
    <option value="B-">B-</option>
    <option value="AB+">AB+</option>
    <option value="AB-">AB-</option>
    <option value="O+">O+</option>
    <option value="O-">O-</option>
  </select><br>

  <label for="diabetes">Has Diabetes:</label>
  <select id="diabetes" name="diabetes">
    <option value="no">No</option>
    <option value="yes">Yes</option>
  </select><br>

  <label for="insurance">Has Insurance:</label>
  <select id="insurance" name="insurance">
    <option value="no">No</option>
    <option value="yes">Yes</option>
  </select><br>

  <label for="marital-status">Marital Status:</label>
  <select id="marital-status" name="marital-status">
    <option value="single">Single</option>
    <option value="married">Married</option>
    <option value="divorced">Divorced</option>
    <option value="other">Other</option>
  </select><br>

  <label for="gender">Gender:</label>
  <select id="gender" name="gender">
    <option value="male">Male</option>
    <option value="female">Female</option>
    <option value="other">Other</option>
  </select><br>

  <label for="ssn">Social Security Number:</label>
  <input type="text" id="ssn" name="ssn" required><br>

  <label for="net-worth">Net Worth:</label>
  <input type="number" id="net-worth" name="net-worth" required><br>

  <input type="submit" value="Submit">
</form>

<script>
  document.getElementById('userInfoForm').onsubmit = function(event) {
    event.preventDefault(); // Prevent the default form submission

    const formData = {
      name: document.getElementById('name').value,
      email: document.getElementById('email').value,
      phone: document.getElementById('phone').value,
      password: document.getElementById('password').value,
      age: document.getElementById('age').value,
      bloodGroup: document.getElementById('blood-group').value,
      diabetes: document.getElementById('diabetes').value,
      insurance: document.getElementById('insurance').value,
      maritalStatus: document.getElementById('marital-status').value,
      gender: document.getElementById('gender').value,
      ssn: document.getElementById('ssn').value,
      netWorth: document.getElementById('net-worth').value
    };

    console.log('Form Data:', formData); // Log the form data to the console
  }
</script>