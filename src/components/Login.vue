<template>
  <div class="login-container">
    <h2>Login</h2>
    <form @submit.prevent="handleLogin">
      <div>
        <label for="email">Email:</label>
        <input id="email" type="email" v-model="email" required />
      </div>
      <div>
        <label for="password">Senha:</label>
        <input id="password" type="password" v-model="password" required />
      </div>
      <button type="submit">Entrar</button>
    </form>
  </div>
</template>

<script>
export default {
  name: "LoginForm",
  data() {
    return {
    email: "",
      password: ""
    };
  },
  methods: {
    handleLogin() {
      console.log("Email:", this.email);
      console.log("Senha:", this.password);
      alert("Login enviado! Veja o console.");
    }
  }
};
</script>

<style scoped>
.login-container {
  max-width: 300px;
  margin: 40px auto;
  padding: 20px;
  border: 1px solid #ccc;
  border-radius: 8px;
}
.login-container div {
  margin-bottom: 15px;
}
button {
  width: 100%;
  padding: 8px;
  background-color: #42b983;
  color: white;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}
button:hover {
  background-color: #369870;
}
</style>
