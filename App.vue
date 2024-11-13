 
<template>
  <div id="app">
    <Navbar />
    <HeroSection />
    <AboutMe />
    <Portfolio />
    <Skills />
    <Testimonials />
    <ContactForm />
    <Footer />
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue'
import HeroSection from './components/HeroSection.vue'
import AboutMe from './components/AboutMe.vue'
import Portfolio from './components/Portfolio.vue'
import Skills from './components/Skills.vue'
import Testimonials from './components/Testimonials.vue'
import ContactForm from './components/ContactForm.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Navbar,
    HeroSection,
    AboutMe,
    Portfolio,
    Skills,
    Testimonials,
    ContactForm,
    Footer
  }
}
</script>

<style>
@import './styles/style.css';
</style>
