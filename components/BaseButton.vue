<style scoped>
.button {
  background: #ff4f4f;
  color: #fff;
  font-weight: 500;
}
</style>

<template>
  <button class="py-3 px-5 button">
    {{ text }}
  </button>
</template>

<script>
export default {
  name: 'BaseButton',
  props: {
    text: {
      type: String,
      default: ''
    }
  }
}
</script>
