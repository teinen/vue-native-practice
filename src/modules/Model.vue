<template>
  <view class="container">
    <text-input
      class="text-input-container"
      placeholder="Type here!"
      v-model="textContent"
    />
    <text class="text-container">{{ textContent }}</text>
  </view>
</template>

<script>
export default {
  data () {
    return {
      textContent: ''
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
