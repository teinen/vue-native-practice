<template>
  <view class="container">
    <button
      :on-press="handleBtnClickCount"
      :title="btnTitle"
    />
    <text class="text-container">{{ btnClickCount }}</text>
  </view>
</template>

<script>
export default {
  data () {
    return {
      btnTitle: 'Click me!',
      btnClickCount: 0
    }
  },
  methods: {
    handleBtnClickCount () {
      this.btnClickCount += 1
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
  font-size: 20;
}
</style>
