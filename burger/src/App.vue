<template> 
<div>
  <Navbar :logo="logo_nav" :alt="alt_nav"/> 

    <router-view/>
    
  
  <Footer/>
  
  
  </div> 
  
</template>

<script>
import Footer from './components/Footer.vue'
import Navbar from './components/Navbar.vue'
export default {
  components: { 
    Navbar,
    Footer },
    data() {
      return {
        logo_nav: "/img/logo.png",
        alt_nav:"Faça seu Hamburger"
      }
    },

}
</script>

<style>
  * {
    font-family: Helvetica;
    padding: 0 0;
    margin: 0;
    box-sizing: border-box;
  }

  .main-container {
    margin: 50px;
    min-height: 250px;
  }

  h1 {
    text-align: center;
    font-size: 42px;
    margin-bottom: 30px;
    color: #222;
  }
</style>