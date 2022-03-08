<template>
    <footer>
        <div class="footer_first-section">
            <div class="container">
                <section>
                    <ul>
                        <h3>dc comics</h3>
                        <li><a href="">lorem</a></li>
                        <li><a href="">lorem</a></li>
                        <li><a href="">lorem</a></li>
                        <li><a href="">lorem</a></li>
                        <li><a href="">lorem ipsum dolor</a></li>
                        <li><a href="">lorem</a></li>
                        <li><a href="">lorem</a></li>
                        <h3>shop</h3>
                        <li><a href="">lorem</a></li>
                        <li><a href="">lorem</a></li>
                    </ul>

                    <ul>
                        <h3>dc</h3>
                        <li><a href="">lorem</a></li>
                        <li><a href="">lorem</a></li>
                        <li><a href="">lorem</a></li>
                        <li><a href="">lorem</a></li>
                        <li><a href="">lorem</a></li>
                        <li><a href="">lorem</a></li>
                        <li><a href="">lorem</a></li>
                        <li><a href="">lorem</a></li>
                        <li><a href="">lorem</a></li>
                        <li><a href="">lorem</a></li>
                        <li><a href="">lorem</a></li>
                    </ul>

                    <ul>
                        <h3>sites</h3>
                        <li><a href="">lorem</a></li>
                        <li><a href="">lorem</a></li>
                        <li><a href="">lorem</a></li>
                        <li><a href="">lorem</a></li>
                        <li><a href="">lorem</a></li>
                    </ul>
                </section>
                        
                <figure>
                    <img src="../assets/dc-logo-bg.png" alt="">
                </figure>
            </div>
        </div>

        <div class="footer_bottom">
            <div class="container">
                <a class="sign-up" href="">sign-up now!</a>

                <div class="container-logo">
                    <a href="">follow us</a>
                    <img src="../assets/footer-facebook.png" alt="">
                    <img src="../assets/footer-twitter.png" alt="">
                    <img src="../assets/footer-youtube.png" alt="">
                    <img src="../assets/footer-pinterest.png" alt="">
                    <img src="../assets/footer-periscope.png" alt="">
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name : 'appFooter'
}
</script>

<style lang="scss" scoped>
    footer{
        color: white;
        .footer_first-section{
            background-image: url('../assets/footer-bg.jpg');
            background-repeat: no-repeat;
            background-size: cover;
            .container{
                display: flex;
                justify-content: space-between;
                section{
                    display: flex;
                    gap: 30px;
                    ul{
                        list-style: none;
                        text-transform: uppercase;
                        h3{
                            padding: 20px 0;
                        }
                        li{
                            padding: 5px 0;
                            a{
                                text-decoration: none;
                                color: #959595;
                                font-size: 12px;
                            }
                        }
                    }

                }
                figure{
                    overflow: hidden;
                    img{
                        margin:-90px 0;
                    }
                }
            }
        }
       
       .footer_bottom{
           background-color: #303030;
           text-transform: uppercase;
           font-weight: 700;
           padding: 25px 0;
           .container{
               .sign-up{
                   color: white;
                   border: 2px solid #0282F9;
                   padding: 15px;
                   text-decoration: none;
               }
               display: flex;
               justify-content: space-between;
               .container-logo{
                   display: flex;
                   align-items: center;
                   gap: 20px;
                   a{
                       text-decoration: none;
                       color:#0282F9
                   }
               }
           }
       }
        
    }
</style>