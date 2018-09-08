<template>
  <section>
    <div class="burger">
      <span class="burger-open" v-show="isOpen"></span>
      <span v-if="isOpen">
        <svg class="close" version="1.1" xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24">
          <title>x</title>
          <path d="M13.4 12l5.3-5.3c0.4-0.4 0.4-1 0-1.4s-1-0.4-1.4 0l-5.3 5.3-5.3-5.3c-0.4-0.4-1-0.4-1.4 0s-0.4 1 0 1.4l5.3 5.3-5.3 5.3c-0.4 0.4-0.4 1 0 1.4 0.2 0.2 0.4 0.3 0.7 0.3s0.5-0.1 0.7-0.3l5.3-5.3 5.3 5.3c0.2 0.2 0.5 0.3 0.7 0.3s0.5-0.1 0.7-0.3c0.4-0.4 0.4-1 0-1.4l-5.3-5.3z"></path>
        </svg>
      </span>
      <span v-else>
        <svg class="open" version="1.1" xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24">
          <title>menu</title>
          <path d="M21 11h-18c-0.6 0-1 0.4-1 1s0.4 1 1 1h18c0.6 0 1-0.4 1-1s-0.4-1-1-1z"></path>
          <path d="M3 7h18c0.6 0 1-0.4 1-1s-0.4-1-1-1h-18c-0.6 0-1 0.4-1 1s0.4 1 1 1z"></path>
          <path d="M21 17h-18c-0.6 0-1 0.4-1 1s0.4 1 1 1h18c0.6 0 1-0.4 1-1s-0.4-1-1-1z"></path>
        </svg>
      </span>
    </div>
    <div class="overlay" v-if="isOpen">
      <div class="menu-content">
        <ul>
          <li class="menu-active">
            <a href="#">Inicio</a>
          </li>
          <li>
            <a href="#">Estrenos</a>
          </li>
          <li>
            <a href="#">Cartelera</a>
          </li>
          <li>
            <a href="#">Mejores</a>
          </li>
        </ul>
      </div>
    </div>
  </section>
</template>
<script>
  export default{
    data () {
      return {
        isOpen: false,
      }
    },
  }
</script>
<style scoped>
  .overlay{
    position: fixed;
    width: 100%;
    height: 100vh;
    background: rgba(0,0,0,0.8);
    top:0;
    left: 0;
    z-index: 99;
  }
  .burger{
    position: fixed;
    width: 50px;
    height: 50px;
    border-radius:50%;
    background-color: #2a3555;
    top: 15px;
    right: 15px;
    z-index: 101;
  }
  .burger-open{
    position: absolute;
    width: 100%;
    height: 100%;
    background: #fff;
    left: 0;
    border-radius: 50%;
  }
  .open,
  .close{
    position: relative;
    display: block;
    margin: 0 auto;
    margin-top: 12px;
    fill:#ff1f6b;
  }
  .menu-content{
    position: relative;
    width: 80%;
    margin: 0 auto;
    background-color: #1f191a;
    padding: 30px 20px;
    border-radius:5px;
    margin-top:40px;
  }
  .menu-content ul,
  .menu-content ul li{
    padding:0px;
    margin:0px;
    text-align: left;
    list-style: none;
  }
  .menu-content ul li{
    padding: 20px 30px;
  }
  .menu-content ul li a{
    text-decoration:none;
    color: #6adbd3;
    font-size: 30px;
    font-weight: bold;
    padding: 20px 30px;
  }
  .menu-content ul li:hover{
    color:#ff1f6b;
    background-color: #313434;
  }
  .menu-active{
    background-color: #313434;
  }
  .menu-active a{
    color:#ff1f6b!important;
  }
</style>

