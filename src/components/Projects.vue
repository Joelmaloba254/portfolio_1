<template>
    <div>
      <section class="projects-section">
        <div class="container">
          <h2>Projects</h2>
          <div class="projects">
            <div class="project" v-for="(project, index) in projects" :key="index">
              <h3>{{ project.title }}</h3>
              <p>{{ project.description }}</p>
              <p><strong>Technologies Used:</strong> {{ project.technologies }}</p>
              <!-- Add more project details as needed -->
            </div>
          </div>
        </div>
      </section>
    </div>
  </template>
  
  <script>
  export default {
    name: 'ProjectsPage',
    data() {
      return {
        projects: [
          {
            title: 'LIVING THE TRUTH',
            description: 'This is an online ministry. The ministry is about spreadig the gospel more so to the online comumnity, targeting youths to live the truth.',
            technologies: ' Django'
            // Add more project details as needed
          },
          {
            title: 'M-Hardware',
            description: 'This is  an ecomerce site for a hardware',
            technologies: 'Django'
            // Add more project details as needed
          },
          {
            title: 'ONLINE HAPPY BIRTHDAY CARD',
            description: 'The card was for a friend of mine who was turnimg 26 years old and I had this to offer as a gift  to her.',
            technologies: 'HTML, CSS, JAVASCRIPT'
            // Add more project details as needed
          },
          {
            title: 'SSPOUSE GIFT',
            description: 'I had to have a gift to my brothe for his girlfriend as a site.',
            technologies: 'HTML ,CSS, JAVASCRIPT'
            // Add more project details as needed
          },
          // Add more projects as needed
        ]
      }
    }
  }
  </script>
  
  <style scoped>
  .projects-section {
    padding: 80px 0;
    text-align: center;
  }
  
  .projects-section h2 {
    font-size: 2rem;
    margin-bottom: 40px;
  }
  
  .projects {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    grid-gap: 30px;
  }
  
  .project {
    background-color: #f2f2f2;
    padding: 20px;
    border-radius: 5px;
    text-align: left;
  }
  
  .project h3 {
    font-size: 1.5rem;
    margin-bottom: 10px;
  }
  
  .project p {
    font-size: 1.2rem;
    margin-bottom: 10px;
  }
  </style>
  
