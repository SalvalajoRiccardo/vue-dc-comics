<template>
    <section>
        <div class="bluenav">
            <div>
                <img :src="require('../assets/img/buy-comics-digital-comics.png')" alt="">
                <span>digital comics</span>
            </div>
            <div>
                <img :src="require('../assets/img/buy-comics-merchandise.png')" alt="">
                <span>dc merchandise</span>
            </div>
            <div>
                <img :src="require('../assets/img/buy-comics-subscriptions.png')" alt="">
                <span>subscription</span>
            </div>
            <div>
                <img :src="require('../assets/img/buy-comics-shop-locator.png')" alt="">
                <span>comic shop local</span>
            </div>
            <div>
                <img :src="require('../assets/img/buy-dc-power-visa.svg')" alt="">
                <span>digital comics</span>
            </div>
            
        </div>
    </section>
</template>

<script>
export default {
  name: 'BlueCutter',
  
  
}
</script>

<style scoped lang="scss">
section {
    background-color: #0c7cec;
    .bluenav {
        width: 80%;
        margin: 0 auto;
        display: flex;
        justify-content: center;
        align-items: center;
        padding: 0 100px;
        div {
            display: flex;
            align-items: center;
            padding: 20px;
            span {
                color: white;
                text-transform: uppercase;
                vertical-align: center;
                margin-left: 20px;
            }
            img {
                vertical-align: center;
                width: 60px;
            }
        }
    }
}
    
</style>