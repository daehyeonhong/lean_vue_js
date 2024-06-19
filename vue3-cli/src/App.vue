<template>
  <div>
    {{ message }}
  </div>
  <button @click="showAlert">경고</button>
</template>

<script>
export default {
  data() {
    return {
      message: 'Hello, World!'
    }
  },
  methods: {
    showAlert() {
      alert(this.message)
    }
  }
}
</script>

<style scoped>

</style>