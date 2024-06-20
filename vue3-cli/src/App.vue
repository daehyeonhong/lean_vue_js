<template>
  <app-header/>
  <div>
    {{ message }}
  </div>
  <button @click="showAlert">경고</button>
</template>

<script>
// import 컴포넌트이름 from './컴포넌트경로'
import AppHeader from "@/components/AppHeader.vue";

export default {
  components: {
    'app-header': AppHeader,
  },
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