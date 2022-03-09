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
                    <li v-for="(item,index) in icons" :key="index">
                        <img :src="item.image">
                        {{item.text}}
                    </li>
                </ul>
            </div>
        </div>
    </main>
</template>

<script>
export default {
    name : 'appMain',
    data : function(){
        return {
            icons:[
                {
                    image : require('../assets/buy-comics-digital-comics.png'),
                    text : 'digital comics'
                },
                {
                    image : require('../assets/buy-comics-merchandise.png'),
                    text : 'dc merchandise'
                },
                {
                    image : require('../assets/buy-comics-subscriptions.png'),
                    text : 'subscription'
                },
                {
                    image : require('../assets/buy-comics-shop-locator.png'),
                    text : 'comic shop locator'
                },
                {
                    image : require('../assets/buy-dc-power-visa.svg'),
                    text : 'dc power visa'
                },
            ]
        }
    }
    
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