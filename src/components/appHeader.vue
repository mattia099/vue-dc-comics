<template>
  <header>
    <div class="container">
      <figure class="logo">
        <img src="../assets/dc-logo.png">
      </figure>
      <nav>
        <ul>
          <li><a href="">charachters</a></li>
          <li><a href="">comics</a></li>
          <li><a href="">movies</a></li>
          <li><a href="">tv</a></li>
          <li><a href="">games</a></li>
          <li><a href="">collectibles</a></li>
          <li><a href="">videos</a></li>
          <li><a href="">fans</a></li>
          <li><a href="">news</a></li>
          <li><a href="">shop</a></li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: 'appHeader',
  
}
</script>


<style lang="scss" scoped>
  .container{
    display: flex;
    justify-content: space-between;
    
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