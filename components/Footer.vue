<template>
    <footer class="footer">
      <p>&copy; 2024 Your Name. All rights reserved.</p>
      <div class="social-links">
        <a href="#" target="_blank">LinkedIn</a>
        <a href="#" target="_blank">GitHub</a>
        <a href="#" target="_blank">Twitter</a>
      </div>
    </footer>
  </template>
  
  <script>
  export default {
    name: 'Footer'
  }
  </script>
  
  <style scoped>
  .footer {
    background-color: #222;
    color: white;
    text-align: center;
    padding: 20px;
  }
  .social-links a {
    margin: 0 10px;
    color: white;
    text-decoration: none;
    font-size: 18px;
  }
  .social-links a:hover {
    color: #ff00ff;
  }
  </style>
  