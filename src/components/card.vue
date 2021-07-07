<template>
    <div class="card">
        <img :src="item.thumb" alt="">
        <h4>{{item.series}}</h4>
    </div>
</template>

<script>
export default {
  name: 'Card',
  props: ["item"]
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    .card {
        padding: 10px;
        width: 15%;
        margin: 10px;
        h4{
            color: white;
            text-transform: uppercase;
        }
        img {
            width: 100%;
        }
    }
</style>
