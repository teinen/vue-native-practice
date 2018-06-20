<template>
  <view class="container">
    <todo-item
      class="text-container"
      v-for="todo in todos"
      :key="todo.id"
      :item="todo"
    ></todo-item>
  </view>
</template>

<script>
import TodoItem from '../components/todoItem.vue'

export default {
  components: {
    'todo-item': TodoItem
  },
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
  font-size: 22;
}
.text-input-container {
  width: 300;
  height: 40;
  font-size: 22;
  border-color: gray;
}
</style>
