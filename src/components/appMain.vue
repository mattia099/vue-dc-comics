<template>
    <main>
        <figure class="jumbotron">
            <div class="container">
                <span>Current series</span>
            </div>
            </figure>
        <div class="content">
            
            <div class="container">
                <comics-card class="grid-item" v-for="(card,index) in fumetti" :key="index" :element="card"/>
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

import comicsCard from './comicsCard.vue'

export default {
    name : 'appMain',
    components : {
        comicsCard
    },
    data : function(){
        return {
            fumetti:[
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel"
                }
                ],
            
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
        .jumbotron{
            background-image: url('../assets/jumbotron.jpg');
            height: 400px;
            .container{
                height: 100%;
                position: relative;
                span{
                    position: absolute;
                    top:100%;
                    left:-10px;
                    transform: translateY(-50%);
                    background-color: #0282F9;
                    font-size: 20px;
                    font-weight: 700;
                    text-transform: uppercase;
                    padding: 15px 25px;
                }
            }
        }
        .content{
            background-color: #1C1C1C;
            font-size: 20px;
            font-weight: 700;
            .container{
                padding:50px 0;
                display: flex;
                justify-content: space-between;
                flex-wrap: wrap;
                gap:20px;
                .grid-item{

                }
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