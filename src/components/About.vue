<template>
    <div>
      <section class="about-section">
        <div class="container">
          <h2>About Me</h2>
          <div class="about-content">
            <div class="intro">
              <h3>Hi, I'm Wanjala Joel Wangila Maloba</h3>
              <p>I'm a Fullstack Developer currently pursuing a Diploma course at Ramogi Institute of Advanced Technology (RIAT). I'm expected to graduate in November 2026. I consider myself an intermediate developer with skills in Vue.js, Python, and Django. I'm also exploring Kotlin programming.</p>
              <p>During my time at Kenya Power Lighting Company (KPLC) headquarters, I gained valuable experience in data networking and telecoms. I worked with switches, routers, network cable termination, and fiberoptic systems. I particularly enjoyed preventive maintenance (PM) tasks.</p>
              <p>My interests include Spreading the Gospel, Development, IoT, and I have a passion for Martial Arts (Shotokan Karate) and Cooking. I'm also looking forward to venturing into pentesting and cyber security.</p>
              <p>Feel free to contact me at +254 742705858 or via email at joelmaloba003@gmail.com</p>
            </div>
          </div>
        </div>
      </section>
    </div>
  </template>
  
  <script>
  export default {
    name: 'AboutPage'
  }
  </script>
  
  <style scoped>
  .about-section {
    padding: 80px 0;
    text-align: center;
  }
  
  .about-section h2 {
    font-size: 2rem;
    margin-bottom: 40px;
  }
  
  .about-content {
    display: flex;
    justify-content: center;
    align-items: flex-start;
  }
  
  .intro {
    flex: 1;
    text-align: left;
  }
  
  .intro h3 {
    font-size: 1.5rem;
    margin-bottom: 20px;
  }
  
  .intro p {
    font-size: 1.2rem;
    line-height: 1.6;
  }
  </style>
  