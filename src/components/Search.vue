<template>
  <section>
    <div class="search">
      <span class="search-icon">
        <svg version="1.1" xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24">
          <title>search</title>
          <path d="M21.7 20.3l-3.7-3.7c1.2-1.5 2-3.5 2-5.6 0-5-4-9-9-9s-9 4-9 9c0 5 4 9 9 9 2.1 0 4.1-0.7 5.6-2l3.7 3.7c0.2 0.2 0.5 0.3 0.7 0.3s0.5-0.1 0.7-0.3c0.4-0.4 0.4-1 0-1.4zM4 11c0-3.9 3.1-7 7-7s7 3.1 7 7c0 1.9-0.8 3.7-2 4.9 0 0 0 0 0 0s0 0 0 0c-1.3 1.3-3 2-4.9 2-4 0.1-7.1-3-7.1-6.9z"></path>
        </svg>
      </span>
      <input class="search-input" type="text" placeholder="Buscar Pelicula">
      <span class="search-remove">
        <svg version="1.1" xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24">
          <title>x</title>
          <path d="M13.4 12l5.3-5.3c0.4-0.4 0.4-1 0-1.4s-1-0.4-1.4 0l-5.3 5.3-5.3-5.3c-0.4-0.4-1-0.4-1.4 0s-0.4 1 0 1.4l5.3 5.3-5.3 5.3c-0.4 0.4-0.4 1 0 1.4 0.2 0.2 0.4 0.3 0.7 0.3s0.5-0.1 0.7-0.3l5.3-5.3 5.3 5.3c0.2 0.2 0.5 0.3 0.7 0.3s0.5-0.1 0.7-0.3c0.4-0.4 0.4-1 0-1.4l-5.3-5.3z"></path>
        </svg>
      </span>
    </div>
  </section>
</template>
<script>
  export default{
    
  }
</script>
<style scoped>
  .search{
    position: relative;
    width: 90%;
    margin: 0 auto;
    background-color: #010623;
    border-radius: 5px;
    border: 1px solid #1c2745;
  }
  .search-input{
    display: block;
    width: 70%;
    margin: 0 auto;
    padding: 15px 0px;
    background-color: #010623;
    color: #fff;
    border:0px;
    outline:none;
  }
  .search-icon,
  .search-remove{
    position: absolute;
  }
  .search-icon{
    left: 10px;
    top: 10px;
  }
  .search-icon svg{
    fill:#8d8988;
  }
  .search-remove{
    right: 10px;
    top: 10px;
  }
  .search-remove svg{
    fill: #ff1f6b;
  }
  @media (min-width:414px){
    .search{
      width: 380px;
    }
  }
</style>
