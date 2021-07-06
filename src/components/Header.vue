<template>
  <header>
    <div class="h-container">
      <div id="logo-h">
        <img src="@/assets/img/dc-logo.png" alt="logo-dc">
      </div>

      <nav>
        <ul>
          <li v-for="(link,index) in links" :key="index" :class="link.current ? 'active' : '' "><a :href="link.url">{{ link.text }} </a></li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: 'Header',
  data() {
    return {
      links :[
        {
          text: 'characters',
          url:'#',
          current: false,
        },
        {
          text: 'comix',
          url:'#',
          current: true,
        },
        {
          text: 'movies',
          url:'#',
          current: false,
        },
        {
          text: 'tv',
          url:'#',
          current: false,
        },
        {
          text: 'games',
          url:'#',
          current: false,
        },
        {
          text: 'collectibles',
          url:'#',
          current: false,
        },
        {
          text: 'videos',
          url:'#',
          current: false,
        },
        {
          text: 'fans',
          url:'#',
          current: false,
        },
        {
          text: 'news',
          url:'#',
          current: false,
        },
        {
          text: 'shop',
          url:'#',
          current: false,
        }
        
      ]
    }
  }
 
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

header {
  height: 140px;
  .h-container {
    background-color: white;
    display: flex;
    justify-content: space-around;
    align-items: center;
    height: 100px;
    
    #logo-h {
      width: 100px;
      height: 100%;
      padding: 20px;
    }
    nav {
      height: 100%;
      padding: 30px;
      ul{
        list-style: none;
        padding: 20px;
        li{
          display: inline-block;
          padding: 10px;
          a {
            display: inline-block;
            color: black;
            text-decoration: none;
            text-transform: uppercase;
            font-weight: 600;
            height: 80px;
          }
          &:hover, &.active {
            a{
            color: #0c7cec;
            border-bottom: 3px solid #0c7cec;
            }
          }
        }
      }
    }

  }
}




</style>
