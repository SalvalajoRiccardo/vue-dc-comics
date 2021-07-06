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
  background-color: #212121;
  height: 300px;

  .h-container {
    background-color: white;
    display: flex;
    justify-content: space-around;
    #logo-h {
      width: 100px;
    }
    nav {
      height: 100%;
      ul{
        list-style: none;
        li{
          height: 100px;
          display: inline-block;
          padding: 10px;
          a {
            color: black;
            text-decoration: none;
          }
        }
      }
    }

  }
}

.active {
  
  border-bottom: 2px solid #53b0f0;
  a{
    color: #53b0f0;
  }
}


</style>
