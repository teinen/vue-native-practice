<template>
  <view class="container">
    <!-- <text class="text-color-primary">{{ message }}</text> -->
    <todo-comp></todo-comp>
  </view>
</template>

<script>
import Button from './src/modules/Button.vue'
import Loop from './src/modules/Loop.vue'
import ToDo from './src/modules/Todo.vue'

export default {
  components: {
    'button-comp': Button,
    'loop-comp': Loop,
    'todo-comp': ToDo
  },
  data () {
    return {
      message: 'Hello, World!'
    }
  }
}
</script>


<style>
.container {
  flex: 1;
  background-color: white;
  align-items: center;
  justify-content: center;
}
.text-color-primary {
  color: blue;
  font-size: 30;
}
</style>
