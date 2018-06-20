<template>
  <view>
    <button :title="message" :on-press="handleBtnPress"></button>
  </view>
</template>

<script>
export default {
  data () {
    return {
      message: "Hello, World!"
    }
  },
  methods: {
    handleBtnPress () {
      alert('Btn Press')
    }
  }
}
</script>

<style>

</style>
