<template lang="html">
  <div class="login">
    <h2>Login</h2>
    <form>
      <input class="uk-input uk-width-1-3 input" type="text" placeholder="Email"><br />
      <input class="uk-input uk-width-1-3 input" type="password" placeholder="Password"><br />
      <button class="uk-button uk-button-secondary">Sign In</button>
    </form>
    <br />
    <router-link to="/register" class="p">Don't have account yet ?</router-link>
  </div>
</template>

<script>
export default {
  name: 'login'
}
</script>

<style lang="css">
  h2 {
    font-family: Helvetica,"Helvetica Neue",Arial,"Lucida Grande",sans-serif;
    font-weight: 400;
    color: black;
    letter-spacing: 1px;
  }

  .login {
    margin: 30px 20px
  }

  .input {
    margin: 10px 0
  }

  .p {
    color: black;
    font-weight: 400;
    font-family: Helvetica,"Helvetica Neue",Arial,"Lucida Grande",sans-serif;
  }

  .p:hover {
    color: black;
  }
</style>
