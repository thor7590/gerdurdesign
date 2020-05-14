<template>
  <div class="mywork">
      <section id="box-container">
            <div id="container">
                <div id="box-1">
                    <img src="~@/assets/illustrator1.jpg">
                </div>
                <div id="box-2">
                    <img src="~@/assets/illustrator.jpg">
                </div>
                <div id="box-3">
                    <img src="~@/assets/logo.jpg">
                </div>
                <div id="box-4">
                    <img src="~@/assets/photoshop.jpg">
                </div>
            </div>
        </section>
  </div>
</template>

<script>
  export default {

    
  }
</script>

<style scoped>

#box-container {
    
    display: flex;
    justify-content: center; /* þetta færir öll boxin í miðjuna */
    width: 100%;

}

#container {
    display: flex;
    flex-flow: row wrap;
    width: auto;
    justify-content: center;
    }

#box-1, #box-2, #box-3, #box-4 {
    height: 200px;
    width: 200px;
    margin-left: 10px; 
    margin-top: 50px;
    margin-bottom: 50px;
}


#container img {
    height: 200px;
    width: 200px;
    object-fit: cover;
}

img {
    
}

</style>
