<template>
    <div>
      <section class="intro-section">
        <div class="container">
          <h1>Welcome to My Portfolio</h1>
          <p>I'm Joel Maloba, a Fullstack Developer currently studying at Ramogi Institute of Advanced Technology (RIAT). I'm passionate about creating interactive web experiences using Vue.js and Django.</p>
          <router-link to="/about" class="btn">Learn More</router-link>
        </div>
      </section>
      
      <!-- Other sections can be added here -->
    </div>
  </template>
  
  <script>
  export default {
    name: 'HomePage'
  }
  </script>
  
  <style scoped>
  .intro-section {
    background-color: #f2f2f2;
    padding: 80px 0;
    text-align: center;
  }
  
  .intro-section h1 {
    font-size: 2.5rem;
    margin-bottom: 20px;
  }
  
  .intro-section p {
    font-size: 1.2rem;
    margin-bottom: 40px;
  }
  
  .btn {
    display: inline-block;
    background-color: #3498db;
    color: #fff;
    padding: 10px 20px;
    border-radius: 5px;
    text-decoration: none;
    transition: background-color 0.3s ease;
  }
  
  .btn:hover {
    background-color: #2980b9;
  }
  </style>
  