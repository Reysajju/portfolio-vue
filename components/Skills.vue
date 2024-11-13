 
<template>
    <section id="skills" class="skills">
      <h2>My Skills</h2>
      <div class="skills-list">
        <div class="skill" v-for="skill in skills" :key="skill.name">
          <div class="skill-name">{{ skill.name }}</div>
          <div class="skill-bar" :style="{ width: skill.proficiency + '%' }"></div>
        </div>
      </div>
    </section>
  </template>
  
  <script>
  export default {
    name: 'Skills',
    data() {
      return {
        skills: [
          { name: 'Vue.js', proficiency: 85 },
          { name: 'CSS', proficiency: 90 },
          { name: 'JavaScript', proficiency: 75 },
          { name: 'HTML', proficiency: 95 }
        ]
      }
    }
  }
  </script>
  
  <style scoped>
  .skills {
    padding: 60px 20px;
    background-color: #222;
    color: white;
  }
  .skills-list {
    display: flex;
    flex-direction: column;
    gap: 10px;
  }
  .skill {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  .skill-name {
    font-size: 18px;
  }
  .skill-bar {
    width: 0;
    height: 8px;
    background-color: #00ff00;
    transition: width 1s;
  }
  </style>
  