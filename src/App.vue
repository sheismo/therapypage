<template>
  <div class="container">
    <img src="" alt="logo" class="logo">
    <nav class="nav">
      <ul>
        <li>Home</li>
        <li>About Us</li>
        <li>Testimonials</li>
        <li>Contact Us</li>
      </ul>
    </nav>
    <br/>
    <Home />
  </div>
    <Footer />
</template>

<script>
import Home from './components/Home.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {Home, Footer},
  data () {
    return{
    
    }
  }
}
</script>

<style>
#app {
  font-family:'Times New Roman', Times, serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #1f1f1f;
}

*{
  box-sizing: border-box;
  list-style: none;
  cursor:pointer;
}
.container{
  width: 60%;
  margin: 0 auto;
}
.logo{
  float: left;
  margin-bottom: 5px;
  margin-left: 10px;
}
.nav{
  margin-top:0;
  margin-bottom:20px;
  float: right;
}
.nav ul li{
  display: inline; 
  margin-right: 30px;
  color: rgb(99, 176, 243);
}

nav ul li:hover{
  background-color: white;
  padding: 10px;
  border-radius: 15px;
  box-shadow: 1px 1px 1px #eee;
}
</style>
