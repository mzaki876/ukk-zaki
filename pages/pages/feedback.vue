<template>
     <div class="feedback-container">
        <h2>Berikan Feedback Anda</h2>
        <form id="feedbackForm">
            <label for="name">Nama Anda:</label>
            <input type="text" id="name" name="name" required placeholder="Masukkan nama Anda">

            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required placeholder="Masukkan email Anda">

            <label for="message">Pesan Feedback:</label>
            <textarea id="message" name="message" rows="5" required placeholder="Tulis feedback Anda"></textarea>

            <button type="submit">Kirim Feedback</button>
        </form>

        <div id="feedbackResponse" class="response-message"></div>
    </div>
  </template>
  
  <script setup></script>
  
  <style scoped>
  /* style.css */
body {
    font-family: Arial, sans-serif;
    background-color: #f4f4f9;
    margin: 0;
    padding: 0;
}

.feedback-container {
    width: 100%;
    max-width: 600px;
    margin: 50px auto;
    padding: 20px;
    background-color: #fff;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    border-radius: 8px;
}

h2 {
    text-align: center;
    color: #333;
}

label {
    display: block;
    margin-top: 10px;
    font-weight: bold;
}

input, textarea {
    width: 100%;
    padding: 10px;
    margin-top: 5px;
    border: 1px solid #ccc;
    border-radius: 4px;
    font-size: 14px;
}

button {
    width: 100%;
    padding: 10px;
    background-color: #4CAF50;
    color: white;
    font-size: 16px;
    border: none;
    border-radius: 4px;
    cursor: pointer;
    margin-top: 20px;
}

button:hover {
    background-color: #45a049;
}

.response-message {
    margin-top: 20px;
    padding: 10px;
    font-size: 16px;
    border-radius: 4px;
    text-align: center;
    display: none;
}

.response-message.success {
    background-color: #d4edda;
    color: #155724;
}

.response-message.error {
    background-color: #f8d7da;
    color: #721c24;
}

  </style>
  