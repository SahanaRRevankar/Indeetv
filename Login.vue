<template>
  <div class="login-container">
    <h2>Login</h2>
    <form @submit.prevent="login">
      <div class="form-group">
        <label for="username">Username/Email:</label>
        <input type="text" id="username" v-model="username" required />
      </div>
      <div class="form-group">
        <label for="password">Password:</label>
        <input type="password" id="password" v-model="password" required />
      </div>
      <div class="form-group">
        <input type="checkbox" id="remember-me" v-model="rememberMe" />
        <label for="remember-me">Remember Me</label>
      </div>
      <button type="submit">Login</button>
    </form>
    <a href="#" @click.prevent="forgotPassword">Forgot Password?</a>
  </div>
</template>

<script>
export default {
  data() {
    return {
      username: '',
      password: '',
      rememberMe: false
    };
  },
  methods: {
    login() {
      // Mocking login process
      // You can implement actual authentication logic here
      console.log('Logging in with:', this.username, this.password, 'Remember Me:', this.rememberMe);
      // Display a success message or redirect to another page
    },
    forgotPassword() {
      // Open an alert for forgot password
      alert('Forgot Password?');
    }
  }
};
</script>

<style scoped>
body {
  margin: 0;
  padding: 0;
  background-image: url('https://cdn.pixabay.com/photo/2017/08/30/01/05/milky-way-2695569_960_720.jpg');
  background-size: cover;
  background-position: center;
}

.login-container {
  max-width: 400px;
  margin: 0 auto;
  padding: 20px;
  background-color: rgba(255, 255, 255, 0.8); /* Adding a semi-transparent white background */
}

.form-group {
  margin-bottom: 15px;
}

label {
  display: block;
}

input[type="text"],
input[type="password"],
button {
  width: 100%;
  padding: 10px;
  font-size: 16px;
}

button {
  background-color: #007bff;
  color: #fff;
  border: none;
  cursor: pointer;
}

a {
  display: block;
  text-align: right;
  color: #007bff;
  text-decoration: none;
}
</style>
