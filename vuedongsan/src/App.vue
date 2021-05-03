<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <div class="menu">
    <a v-for="a in 메뉴들" :key="a">{{a}}</a>
  </div>
<div>
  원룸샵
</div>
  <div v-for="r in products" :key="r">
    <h4 >{{r}}</h4>
    <p>50 만원</p>
  </div>
</template>

<script>


export default {
  name: 'App',
  data(){
    return {
      메뉴들 : ['Home', 'Shop', 'About'],
      price1 : 60,
      price2 : 70,
      스타일 : 'color : blue',
      products : ['역삼동원룸', '천호동원룸', '구로구원룸'],
    }
  },
  components: {
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.menu{
  background: darkslateblue;
  padding: 15px;
  border-radius: 5px;
}
.menu a {
  color: white;
  padding-left: 10px;
}
</style>
