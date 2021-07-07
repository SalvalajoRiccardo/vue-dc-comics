<template>
  <section>
    <div class="m-container">
      <div id="jumbo">

      </div>

      <div v-for="(card,index) in Cards" :key="index" class="cards">
      

      </div>
    </div>

  </section>
  
</template>

<script>
import CardsData from '@/data/CardsData.js';
export default {
  name: 'MainContent',
  data(){
    return{
      Cards: CardsData

    }
  }
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

section {
  background-color: black;
  .m-container {
    #jumbo {
      height: 400px;
      background-image: url('../assets/img/jumbotron.jpg');
      background-size: cover;
      
    }
  }
  
}

</style>
