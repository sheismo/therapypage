<template>
  <div class="footer">
      <div class="foot1">
          <img src="" alt="logo" class="logo">
      </div>

      <div class="foot2">
          <ul>
              <li>Licensing & Agreement</li>
              <li>Pricing</li>
              <li>Advertising</li>
              <li>Legal</li>
          </ul>
      </div>

      <div class="foot3">
          <p>Follow us on social media:</p>
            <i class="bi bi-twitter"></i>
            <i class="bi bi-linkedin"></i>
            <i class="bi bi-facebook"></i>
            <i class="bi bi-instagram"></i>
      </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
@import url("https://cdn.jsdelivr.net/npm/bootstrap-icons@1.4.1/font/bootstrap-icons.css");

*{
    box-sizing: border-box;
    list-style: none;
}

.footer{
    display: flex;
    justify-content: space-between;
    align-items:center;
    width: 100%;
    height:30vh;
    margin: 0;
    padding: 30px 20%;
    color: white;
    background-color: rgb(50, 154, 245);
}

.foot1, .foot3{
    width: 26%;
    margin:0;
    text-align: center;
}

.foot2{
    width: 45%;
    margin:0;
    text-align: center;
}

.foot2 ul li{
    margin-bottom: 15px;
}

i{
    margin-left: 10px;
    margin-right: 20px;
}

@media (max-width: 1068px){
    .footer{
        flex-direction: column;
        align-items: stretch;
        height:100%;
        padding: 30px 10%;
        margin-top: 30px;
    }
    
    .foot1, .foot2, .foot3{
        width: 100%;
        height: 32%;
        margin-top: 10px;
        text-align: justify;
    }

    i{
        font-size: 0.9rem;
    }
}
</style>