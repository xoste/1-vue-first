<template>
  <div>
    我的第一个vue程序<br/>
    {{text}}<br>
    输入：<input type="text" v-model="text"><br/>
    <ul>
      <li v-for="people in list">{{people.name}}</li>
    </ul>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        text: '大家好',
        list: [{name: '罗劲'} , {name: '陈文财'}, {name: '胡大军'}, {name: '李浪'}, {name: '汪林勇'}]
      }
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

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
