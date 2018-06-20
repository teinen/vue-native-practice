<template>
  <view class="container">
    <text class="text-container" v-for="todo in todos" :key="todo.id">
      {{ todo.text }}
    </text>
  </view>
</template>

<script>
export default {
  data () {
    return {
      todos: [
        { id: 1, text: "Learn JavaScript" },
        { id: 2, text: "Learn Vue" },
        { id: 3, text: "Build something awesome" }
      ]
    }
  }
}
</script>

<style>
.container {
  background-color: white;
  align-items: center;
  justify-content: center;
  flex: 1;
}
.text-container {
  color: blue;
  padding: 2;
}
</style>
