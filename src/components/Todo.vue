<template>
  <div id="todo">
    {{ todo.name }}
  </div>
</template>

<script>
export default {
  name: 'Todo',
  props: {
      todo: Object,
  }
}
</script>

<style>

</style>
