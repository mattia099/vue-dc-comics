<template>
  <header>
    <div class="container">
      
      <img src="../assets/dc-logo.png">
      
      <nav>
        <ul>
          <li v-for="(link,index) in headerLinks" :key="index" :class="link.active ? 'active' : '' "><a href="">{{link.nameLink}}</a></li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: 'appHeader',
  data: function() {
    return{
      headerLinks : [
        {
          nameLink : 'charachters',
          href: '',
          active: true
        },
        {
          nameLink : 'comics',
          href: ''
        },
        {
          nameLink : 'movies',
          href: ''
        },
        {
          nameLink : 'tv',
          href: ''
        },
        {
          nameLink : 'games',
          href: ''
        },
        {
          nameLink : 'collectibles',
          href: ''
        },
        {
          nameLink : 'videos',
          href: ''
        },
        {
          nameLink : 'fans',
          href: ''
        },
        {
          nameLink : 'news',
          href: ''
        },
        {
          nameLink : 'shop',
          href: ''
        },
      ]
    }
  }
}
</script>


<style lang="scss" scoped>
  .container{
    display: flex;
    justify-content: space-between;
    align-items: center;
    
    img{
      width: 80px;
      height: 80px;
      vertical-align: center;
    }
    

    nav{
      display: flex;
      align-items: center;
      ul{
        display: contents;
        list-style: none;

        li{
          padding: 40px 10px;
          position: relative;
          a{
            text-decoration: none;
            color: #464646;
            font-weight: 700;
            text-transform: uppercase;
            font-size: 13px;
            
            &:hover{
              color: #2392FA;
            }

            &:active{
              li.active::after{
                content: '';
                display: block;
                height: 4px;
                position: absolute;
                left: 0;
                right: 0;
                bottom: 0;
                background-color: #2392FA;
              }
            }
            
          }
        }
      }
    }
  }
</style>