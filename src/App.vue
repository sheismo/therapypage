<template>
  <div class="container">
    <img src="" alt="logo" class="logo">
    <nav class="nav" id="nav">
      <ul id="list">
        <li>Home</li>
        <li>About Us</li>
        <li>Testimonials</li>
        <li>Contact Us</li>
      </ul>
    </nav>
    <i class="bi bi-list" @click="showNav" id="show"></i>
    <i class="bi bi-x" @click="closeNav" id="close"></i>
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
  },
  methods: {
    showNav(){
      document.getElementById("show").style.display = "none"
      document.getElementById("close").style.display = "block";
      document.getElementById("nav").style.display = "block";
      document.getElementById("list").style.display = "flex";
      document.getElementById("list").style.flexDirection = "column";
    },
    closeNav(){
      document.getElementById("show").style.display = "block";
      document.getElementById("close").style.display = "none";
      document.getElementById("nav").style.display = "none";
    }
  }
}
</script>

<style scoped>
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

i{
  display: none;
  color: rgb(99, 176, 243);
  font-size: 1.8rem;
}

@media (max-width:768px){
  .container{
    width: 80%;
    margin: 0 auto;
  }

  .bi-list{
    display: block;
    float: right;
    margin-right: -10px;
  }

  .bi-x{
    position: absolute;
    top: 5px;
    right: 5px;
  }

  .nav{
    display: none;
  }

  nav ul li{
    padding: 10px;
    margin: 5px;
  }
}
</style>
