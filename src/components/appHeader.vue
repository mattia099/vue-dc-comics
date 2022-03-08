<template>
  <header>
    <div class="container">
      <figure class="logo">
        <img src="../assets/dc-logo.png">
      </figure>
      <nav>
        <ul>
          <li v-for="(link,index) in headerLinks" :key="index"><a href="">{{link.nameLink}}</a></li>
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
          href: ''
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
    padding: 20px 0;
    .logo{
      img{
        width: 80px;
      }
    }

    nav{
      display: flex;
      align-items: center;
      
      ul{
        display: contents;
        list-style: none;

        li{
          padding: 12px;
          a{
            text-decoration: none;
            color: #464646;
            font-weight: 700;
            text-transform: uppercase;
            font-size: 13px;
            
            &:hover{
              color: #2392FA;
            }
          }
        }
      }
    }
  }
</style>