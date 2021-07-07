<template>
  <section>
    <div class="m-container">
      <div id="jumbo">

      </div>

      <!-- <div v-for="(card,index) in Cards" :key="index" class="cards">
        <img :src=card.thumb alt="">

      </div> -->
      <div class="cards">
        <Card v-for="(card,index) in Cards" :key="index" :item="card"/>
        <button>load more</button>
      </div>
      
    </div>

  </section>
  
</template>

<script>
import CardsData from '@/data/CardsData.js';
import Card from '@/components/Card.vue';
export default {
  name: 'MainContent',
  components: {
    Card
  },
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
  background-color: #1c1c1c;
  .m-container {
    #jumbo {
      height: 400px;
      background-image: url('../assets/img/jumbotron.jpg');
      background-size: cover;
      
    }
    .cards {
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      flex-shrink: 0;
      padding: 40px;
      width: 80%;
      margin: 0 auto;
    }
    button {
      width: 150px;
      height: 30px;
      text-transform: uppercase;
      color: white ;
      background-color: #0c7cec;
      border: none;
      margin: 40px 0 0 0;
    }
  }
  
}

</style>
