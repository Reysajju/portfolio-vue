<template>
    <nav class="navbar">
      <div class="logo">
        <img src="/assets/logo.png" alt="Logo" />
      </div>
      <ul class="nav-links">
        <li><a href="#home">Home</a></li>
        <li><a href="#portfolio">Portfolio</a></li>
        <li><a href="#skills">Skills</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </template>
  
  <script>
  export default {
    name: 'Navbar'
  }
  </script>
  
  <style scoped>
  .navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: #222;
    padding: 10px 20px;
  }
  .nav-links {
    list-style: none;
    display: flex;
    gap: 20px;
  }
  .nav-links li {
    transition: transform 0.3s ease;
  }
  .nav-links li:hover {
    transform: scale(1.1);
  }
  .nav-links a {
    text-decoration: none;
    color: white;
    font-size: 18px;
  }
  </style>
  