<!-- src/views/ContactForm.vue -->

<template>
    <div class="contact">
      <h1>Contact Me</h1>
      <p>If you have any questions or would like to work together, feel free to reach out to me!</p>
      <form @submit.prevent="submitForm" action="https://formspree.io/f/mrgndgjw" method="POST">
        <div class="form-group">
          <label for="name">Name</label>
          <input type="text" id="name" v-model="name" required>
        </div>
        <div class="form-group">
          <label for="email">Email</label>
          <input type="email" id="email" v-model="email" required>
        </div>
        <div class="form-group">
          <label for="message">Message</label>
          <textarea id="message" v-model="message" required></textarea>
        </div>
        <button type="submit">Submit</button>
      </form>
    </div>
  </template>
  
  <script>
  export default {
    name: 'ContactForm',
    data() {
      return {
        name: '',
        email: '',
        message: ''
      }
    },
    methods: {
      submitForm() {
        // No need to send data here. Formspree will handle this.
        // Just clear the form fields after submission
        this.name = '';
        this.email = '';
        this.message = '';
      }
    }
  }
  </script>
  
  <style scoped>
  .contact {
    max-width: 600px;
    margin: 0 auto;
  }
  
  .form-group {
    margin-bottom: 20px;
  }
  
  label {
    display: block;
    font-weight: bold;
  }
  
  input[type="text"],
  input[type="email"],
  textarea {
    width: 100%;
    padding: 10px;
    font-size: 16px;
    border: 1px solid #ccc;
    border-radius: 5px;
  }
  
  textarea {
    height: 150px;
  }
  
  button {
    padding: 10px 20px;
    font-size: 16px;
    background-color: #007bff;
    color: #fff;
    border: none;
    border-radius: 5px;
    cursor: pointer;
  }
  
  button:hover {
    background-color: #0056b3;
  }
  </style>
  