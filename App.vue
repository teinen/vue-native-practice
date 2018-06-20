<template>
  <view class="container">
    <!-- <text class="text-color-primary">{{ message }}</text> -->
    <model-comp></model-comp>
  </view>
</template>

<script>
import Button from './src/modules/Button.vue'
import Loop from './src/modules/Loop.vue'
import ToDo from './src/modules/Todo.vue'
import ClickCount from './src/modules/ClickCount.vue'
import Model from './src/modules/Model.vue'

export default {
  components: {
    'button-comp': Button,
    'loop-comp': Loop,
    'todo-comp': ToDo,
    'click-count-comp': ClickCount,
    'model-comp': Model
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
