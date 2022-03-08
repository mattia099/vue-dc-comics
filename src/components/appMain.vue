<template>
    <main>
        <div class="content">
            <div class="container">
                --> Content goes here
            </div>
        </div>
        <div class="menu">
            <div class="container">
                <ul>
                    <li><img src="../assets/buy-comics-digital-comics.png">digital comics</li>
                    <li><img src="../assets/buy-comics-merchandise.png">dc merchandise</li>
                    <li><img src="../assets/buy-comics-subscriptions.png">subscriptions</li>
                    <li><img src="../assets/buy-comics-shop-locator.png">comic shop location</li>
                    <li><img src="../assets/buy-dc-power-visa.svg">dc power visa</li>
                </ul>
            </div>
        </div>
    </main>
</template>

<script>
export default {
    name : 'appMain',
    
}
</script>

<style lang="scss" scoped>
    main{
        color: white;
        
        .content{
            background-color: #1C1C1C;
            font-size: 20px;
            font-weight: 700;
            .container{
                padding:50px 0;
            }
        }
        
        .menu{
            background-color: #0282F9;
        
            .container{
                padding: 50px 0;
                ul{
                    list-style: none;
                    display: flex;
                    justify-content: center;
                    text-align: center;
                    text-transform: uppercase;
                    font-size: 13px;
                    li{
                        flex-basis: 0%;
                        flex-grow: 1;
                        display: flex;
                        align-items: center;
                        justify-content: center;
                        gap:15px;
                        img{
                            width: 44px;
                            max-height: 57px;
                        }
                    }
                }
            }
            
        }
    }
</style>