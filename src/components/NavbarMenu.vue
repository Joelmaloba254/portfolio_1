<template>
    <nav class="navbar">
      <div class="container">
        <router-link to="/" class="navbar-brand">Portfolio</router-link>
        <button class="navbar-toggler" @click="toggleNavbar">
          <span></span>
          <span></span>
          <span></span>
        </button>
        <ul class="navbar-nav" :class="{ 'show': isNavbarOpen }" @click="closeNavbar">
          <li><router-link to="/" exact :class="{ 'active': $route.path === '/' }">Home</router-link></li>
          <li><router-link to="/about" :class="{ 'active': $route.path === '/about' }">About</router-link></li>
          <li><router-link to="/projects" :class="{ 'active': $route.path === '/projects' }">Projects</router-link></li>
          <li><router-link to="/contact" :class="{ 'active': $route.path === '/contact' }">Contact</router-link></li>
        </ul>
      </div>
    </nav>
  </template>
  
  <script>
  export default {
    name: 'NavbarMenu',
    data() {
      return {
        isNavbarOpen: false
      };
    },
    methods: {
      toggleNavbar() {
        this.isNavbarOpen = !this.isNavbarOpen;
      },
      closeNavbar() {
        if (this.isNavbarOpen) {
          this.isNavbarOpen = false;
        }
      }
    }
  };
  </script>
  
  <style scoped>
  .navbar {
    background-color: #3498db;
    color: #fff;
    padding: 10px 0;
  }
  
  .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  
  .navbar-brand {
    font-size: 1.5rem;
    font-weight: bold;
    text-decoration: none;
    color: #fff;
  }
  
  .navbar-nav {
    list-style: none;
    display: flex;
    margin: 0;
  }
  
  .navbar-nav li {
    margin-left: 20px;
  }
  
  .navbar-nav li a {
    text-decoration: none;
    color: #fff;
  }
  
  .navbar-nav li a.active {
    font-weight: bold;
  }
  
  .navbar-toggler {
    display: none;
    background: none;
    border: none;
    cursor: pointer;
    padding: 0;
  }
  
  .navbar-toggler span {
    display: block;
    width: 25px;
    height: 3px;
    background-color: #fff;
    margin: 5px 0;
  }
  
  @media (max-width: 768px) {
    .container {
      flex-direction: column;
    }
  
    .navbar-nav {
      display: none;
      flex-direction: column;
      padding: 10px 0;
    }
  
    .navbar-nav.show {
      display: flex;
    }
  
    .navbar-nav li {
      margin: 5px 0;
    }
  
    .navbar-toggler {
      display: block;
    }
  }
  </style>
  