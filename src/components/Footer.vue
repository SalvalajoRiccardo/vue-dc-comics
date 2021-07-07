<template>
    <footer>
        <div class="container-f">
            <!-- links -->
            <div class="links">
                <div >
                    <ul> <h3>dc comics</h3>
                        <li>Chacters</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>TV</li>
                        <li>Games</li>
                        <li>Videos</li>
                        <li>News</li>
                    </ul>

                    <ul> <h3>shop</h3>
                        <li>Shop DC</li>
                        <li>Shop DC Collectibles</li>
                    </ul>
                </div>
                <div>
                    <ul><h3>DC</h3>
                        <li>Terms Of Use</li>
                        <li>Private policy(New)</li>
                        <li>Ad Choices</li>
                        <li>Advertising</li>
                        <li>Jobs</li>
                        <li>Subscriptions</li>
                        <li>Talent Workshop</li>
                        <li>CPSC Certificates</li>
                        <li>Rating</li>
                        <li>Shop Help</li>
                        <li>Contact Us</li>
                    </ul>
                </div>
                <div>
                    <ul><h3>sites</h3>
                        <li>DC</li>
                        <li>MAD Megazine</li>
                        <li>DC Kids</li>
                        <li>DC Universe</li>
                        <li>DC Power Visa</li>
                    </ul>
                </div>
            </div>
            <!-- links -->

            <div id="img-footer">
                <!-- <img :src="require('../assets/img/dc-logo-bg.png')" alt=""> -->
            </div>
        </div>

        <!-- social -->
        <div id="social">
            <div class="box">
                <button>SIGN-UP NOW</button>
                <div>
                    <h2>follow us</h2>
                    <img :src="require('@/assets/img/footer-facebook.png')"
                    alt="facebook">
                    <img :src="require('@/assets/img/footer-twitter.png')"
                    alt="twitter">
                    <img :src="require('@/assets/img/footer-youtube.png')"
                    alt="youtube">
                    <img :src="require('@/assets/img/footer-pinterest.png')"
                    alt="pinterest">
                    <img :src="require('@/assets/img/footer-periscope.png')"
                    alt="periscope">
                </div>

            </div>
            
        </div>
        <!-- social -->
    </footer>
  
</template>

<script>
export default {
  name: 'Footer',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

footer {
    background-image: url('../assets/img/footer-bg.jpg');
    background-size: cover;
    background-repeat: no-repeat;
    height: 400px;
    .container-f {
        width: 80%;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
        .links {
            display: flex;
            padding: 50px 0;
            h3 {
                text-transform: uppercase;
                color: white;
                margin: 15px 0;
            }
            ul {
                list-style: none;
                margin-right: 20px;
                color: gray;
                li {
                    font-size: 14px;
                    line-height: 18px;
                }
            }
        }
        #img-footer {
            background-image: url('../assets/img/dc-logo-bg.png');
            width: 50%;
            background-repeat: no-repeat;
            background-size: cover;
            background-position: center;
        }
    }

    #social {
        background-color: #303030;
        .box{
            width: 80%;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            padding: 30px;
            button {
                background-color: #303030;
                border: 2px solid #0c7cec;
                color: white;
                font-size: 18px;
                padding: 15px;
            }
            div {
                display: flex;
                justify-content: space-between;
                align-items: center;
                width: 400px;
                h2 {
                    text-transform: uppercase;
                    color: #0c7cec;
                    flex-shrink: 0;
                    margin-right: 50px;
                }
                img{
                    margin: 10px;
                }
            }
        }

    }
  
}

</style>
