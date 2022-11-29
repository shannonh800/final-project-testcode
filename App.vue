<template>
  <h2>Login</h2>
  <div class="error" v-if="errorMessage">{{ message }}</div>
  <LoginForm msg="Welcome to Your Vue.js App"/>
</template>

<script>
import LoginForm from './components/LoginForm.vue'

export default {
  name: 'App',
  components: {
    LoginForm
  },
  data() {
    return {
      errorMessage: "Test Message" // how to get error message that's located on the backend?? & where do i post to?
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
