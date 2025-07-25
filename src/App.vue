<template>
  <div id="app">
    <LoginForm />
  </div>
</template>

<script>
import LoginForm from './components/Login.vue'

export default {
  name: 'App',
  components: {
    LoginForm
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  text-align: center;
  margin-top: 60px;
}
</style>
