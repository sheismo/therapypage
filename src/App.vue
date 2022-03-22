<template>
    <section>
    <header>
      <div class="container">
        <img src="" alt="logo" class="logo">
        <nav id="nav">
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
      </div>
    </header>
    <Home />
    <Footer />
  </section>
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
@import url('https://fonts.googleapis.com/css2?family=Poppins&display=swap');

#app {
  font-family: 'Poppins', sans-serif;
}

*{
  box-sizing: border-box;
  list-style: none;
  cursor:pointer;
}

header{
  width: 100%;
  margin: 0;
  padding: 0;
  box-shadow: 3px 3px 3px #ddd,3px 3px 3px #ddd;
}

.container{
  width: 70%;
  margin: auto;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo{
  width: 25%;
  margin-left: 10px;
}

nav{
  width: 70%;
}

nav ul li{
  padding: 10px;
  margin-right: 50px;
  display: inline; 
  color: rgb(99, 176, 243);
}

nav ul li:hover{
  background-color: white;
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
