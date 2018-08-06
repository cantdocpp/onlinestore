<template lang="html">
  <div class="register">
    <h2>Create Account</h2>
    <form>
      <input class="uk-input uk-width-1-3 input" type="text" placeholder="First Name"><br />
      <input class="uk-input uk-width-1-3 input" type="text" placeholder="Last Name"><br />
      <input class="uk-input uk-width-1-3 input" type="text" placeholder="Email"><br />
      <input class="uk-input uk-width-1-3 input" type="password" placeholder="Password"><br />
      <button class="uk-button uk-button-secondary">Create</button>
    </form>
    <br />
    <router-link to="/login" class="p">Already have an account ?</router-link>
  </div>
</template>

<script>
export default {
  name: 'register'
}
</script>

<style lang="css">
  h2 {
    color: black
  }

  .register {
    margin: 30px 20px
  }
</style>
