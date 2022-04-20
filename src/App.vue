<template>
  <div id="app">
    <!-- // v-model
    <input type="text" v-model="name">
    <input type="checkbox" v-model="accept"> Tôi đồng ý
    <p>{{ name }}</p> -->

    // v-show
    <div v-show="isShow">Trần Tiến Thành</div>
    <button @click="isShow = !isShow">Ẩn / Hiện</button>
  </div>
</template>

<script>
// import Menu from './components/Menu.vue'

export default {
  data(){
    return {
      name: 'Trần Tiến Thành',
      accept: true,
      isShow: true
    }
  },
  // components: {
  //   Menu
  // },
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
