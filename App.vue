<template>
  <view class="container">
    <text class="text-color-primary">{{ message }}</text>
    <button-comp></button-comp>
  </view>
</template>

<script>
import Button from './modules/Button.vue'

export default {
  components: {
    'button-comp': Button
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
