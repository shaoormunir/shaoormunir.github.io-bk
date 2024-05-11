---
layout: single
title: "Contact Form"
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
  <input type="text" id="blood-group" name="blood-group" required><br>

  <label for="diabetes">Has Diabetes:</label>
  <input type="checkbox" id="diabetes" name="diabetes"><br>

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
      diabetes: document.getElementById('diabetes').checked,
      ssn: document.getElementById('ssn').value,
      netWorth: document.getElementById('net-worth').value
    };

    console.log('Form Data:', formData); // Log the form data to the console
  }
</script>