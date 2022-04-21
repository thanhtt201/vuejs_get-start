<template>
  <div id="app">
    <!-- // v-model
    <input type="text" v-model="name">
    <input type="checkbox" v-model="accept"> Tôi đồng ý
    <p>{{ name }}</p> -->

    <!-- // v-show
    <div v-show="isShow">Trần Tiến Thành</div>
    <button @click="isShow = !isShow">Ẩn / Hiện</button> -->

    <!-- // :class
    <div :class="{showText: isShowText, color: color}">Hello Trần Tiến Thành</div>
    <button @click="isShowText = !isShowText">Show/Hide</button> -->

    // v-for
    <input type="text" v-model="newTodo">
    <button @click="addTodo()">Add Todo</button>
    <div v-for="(todo, index) in todos" :key="index">
      <input type="checkbox" v-model="todo.done">
      <span :class="{todoDone: todo.done}">{{ todo.name }}</span>
    </div>
  </div>
</template>

<script>
// import Menu from './components/Menu.vue'

export default {
  data(){
    return {
      name: 'Trần Tiến Thành',
      accept: true,
      isShow: true,
      isShowText: true,
      color: true,
      newTodo: '',
      todos: [
        { name: 'nấu cơm', done: false},
        { name: 'code', done: false},
        { name: 'đi chợ', done: false},
        { name: 'đi làm', done: true},
      ]
    }
  },
  methods: {
      addTodo: function(){
        this.todos.push({name: this.newTodo, done: false})
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
.showText{
  color: red;
}
.todoDone{
  text-decoration: line-through;
}
</style>
