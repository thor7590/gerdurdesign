<template>
  <div class="home">
    <div id="container">
      <img id="img" src="~@/assets/tobba.png"/>
    </div>
  </div>
</template>

<script>
  export default {
    
  }
</script>

<style scoped>

#container {
    display: flex;
    justify-content: center; /* þetta færir öll boxin í miðjuna */
    width: 100%;
    
}

#img {
  padding: 50px;
  height: 500px;
  width: 500px;
}


</style>

