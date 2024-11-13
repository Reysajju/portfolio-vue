 
<template>
    <section class="contact">
      <h2>Contact Me</h2>
      <form @submit.prevent="submitForm">
        <input type="text" v-model="name" placeholder="Your Name" required />
        <input type="email" v-model="email" placeholder="Your Email" required />
        <textarea v-model="message" placeholder="Your Message" required></textarea>
        <button type="submit" class="submit-btn">Send Message</button>
      </form>
    </section>
  </template>
  
  <script>
  export default {
    data() {
      return {
        name: '',
        email: '',
        message: ''
      };
    },
    methods: {
      submitForm() {
        const formData = {
          name: this.name,
          email: this.email,
          message: this.message
        };
  
        // Use Formspree or another service to handle form submission
        fetch('https://formspree.io/f/mayllrqp', {
          method: 'POST',
          body: JSON.stringify(formData),
          headers: {
            'Content-Type': 'application/json',
          },
        })
        .then((response) => {
          if (response.ok) {
            alert('Message sent successfully!');
            this.name = '';
            this.email = '';
            this.message = '';
          } else {
            alert('Something went wrong.');
          }
        })
        .catch((error) => {
          console.error('Error sending message:', error);
          alert('Something went wrong.');
        });
      }
    }
  };
  </script>
  
  <style scoped>

  
  .contact {
    background-color: #333;
    color: white;
    padding: 50px;
    text-align: center;
  }
  input, textarea {
    width: 100%;
    padding: 10px;
    margin: 10px 0;
    border-radius: 5px;
    border: none;
  }
  .submit-btn {
    padding: 12px 30px;
    background-color: neon;
    color: white;
    border-radius: 5px;
    cursor: pointer;
    transition: all 0.3s;
  }
  .submit-btn:hover {
    background-color: #ff00ff;
  }
  </style>
  