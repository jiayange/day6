<template>
  <div id="app">
    <div class="main">
      <router-view/>
    </div>
    
    <footer>
      <router-link to='/home'>首页</router-link>
      <router-link to='/wode'>我的</router-link>
    </footer>
    
  </div>
</template>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  display: flex;flex-direction: column;
}
*{
  padding: 0;margin: 0;list-style: none;box-sizing: border-box;text-decoration: none;
}
html,body,#app{
  width: 100%;height: 100%;overflow: hidden;
}
footer{
  line-height: 50px;border-top: 1px solid #ccc;text-align:center;display: flex;
  a{
    flex: 1;color:#000;
    &.router-link-active{
      color: red
    }
  }
}
.main{
  flex: 1;overflow: hidden;
}
</style>
