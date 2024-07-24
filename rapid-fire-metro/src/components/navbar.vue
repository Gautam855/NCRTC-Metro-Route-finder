<template>
    <nav>
        <div class="navbar">
          <div class="logo"><a href="#"><img :src="logo" alt=""></a></div>
          <ul class="menu">
            <li><router-link to="/">Home</router-link></li>
            <li><router-link to="/about">About</router-link></li>
            <li><router-link to="/map">Find Map</router-link></li>
            <li><router-link to="/contact-us">Contact us</router-link></li>

          </ul>
        </div>
      </nav>
</template>

<script setup>
import logo from "@/assets/logo.png"
</script>


<style scoped>

@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@200;300;400;500;600;700&display=swap');
*{

  padding: 0;
  box-sizing: border-box;
  font-family: 'Poppins', sans-serif;
}



nav{
    margin: 0;
 position: relative;
 left: 0;
 top: 0;
 width: 100%;
 height: 75px;
 background: #062539;
 box-shadow: 0 5px 10px rgba(0, 0, 0, 0.1);
 z-index: 1;
}
nav .navbar{
 display: flex;
 align-items: center;
 justify-content: space-between;
 height: 100%;
 max-width: 90%;
 background: #062539;
 margin: auto;
}
nav .navbar .logo img{
  color: #fff;
  width: 100px;
}
nav .navbar .menu{
  display: flex;
}
.navbar .menu li{
  list-style: none;
  margin: 0 15px;
}
.navbar .menu li a{
  color: #fff;
  font-size: 17px;
  font-weight: 500;
  text-decoration: none;
}
</style>