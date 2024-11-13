<template>
    <section class="hero">
      <div class="hero-text">
        <h1>Welcome to My Portfolio</h1>
        <p>Bringing your ideas to life with code</p>
        <a href="#portfolio" class="cta-btn">View My Work</a>
      </div>
    </section>
  </template>
  
  <script>
  export default {
    name: 'HeroSection'
  }
  </script>
  
  <style scoped>
  .hero {
    background-image: url('/assets/cyberpunk-bg.jpg');
    background-size: cover;
    background-position: center;
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    color: white;
  }
  .hero h1 {
    font-size: 4rem;
    text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.7);
  }
  .hero p {
    font-size: 1.5rem;
    margin: 20px 0;
  }
  .cta-btn {
    padding: 10px 20px;
    background-color: neon;
    text-decoration: none;
    color: white;
    border-radius: 5px;
    transition: all 0.3s;
  }
  .cta-btn:hover {
    background-color: #ff00ff;
  }
  </style>
  