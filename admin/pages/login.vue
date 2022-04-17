<template>
  <div id="LoginBody" class="text-center">
    <form class="form-signin">
      <img class="mb-4" src="/favicon.ico" alt="" width="72" height="72">
      <h1 class="h3 mb-3 font-weight-normal">Please sign in</h1>

      <b-form-input
        type="email"
        placeholder="Email address"
        required
        autofocus
      ></b-form-input>

      <b-form-input
        type="password"
        placeholder="Password"
        required
      ></b-form-input>

      <div class="mb-3">
        <b-form-checkbox
          :value="true"
          :unchecked-value="false"
        > Remember me</b-form-checkbox>
      </div>

      <b-button
        type="button"
        size="lg"
        variant="primary"
        block
      >Sign in</b-button>

      <p class="mt-5 mb-3 text-muted">&copy; 2017-2021</p>

    </form>
  </div>
</template>

<script lang="ts">
import { Vue, Component } from 'nuxt-property-decorator'

export default class Login extends Vue {

}

</script>

<style>
html,
body {
  height: 100%;
}

#__nuxt {
  height: 100%;
}

#__layout {
  height: 100%;
}

#LoginBody {
  display: -ms-flexbox;
  display: flex;
  -ms-flex-align: center;
  align-items: center;
  padding-top: 40px;
  padding-bottom: 40px;
  background-color: #f5f5f5;
  height: 100%;
}

.form-signin {
  width: 100%;
  max-width: 330px;
  padding: 15px;
  margin: auto;
}
.form-signin .checkbox {
  font-weight: 400;
}
.form-signin .form-control {
  position: relative;
  box-sizing: border-box;
  height: auto;
  padding: 10px;
  font-size: 16px;
}
.form-signin .form-control:focus {
  z-index: 2;
}
.form-signin input[type="email"] {
  margin-bottom: -1px;
  border-bottom-right-radius: 0;
  border-bottom-left-radius: 0;
}
.form-signin input[type="password"] {
  margin-bottom: 10px;
  border-top-left-radius: 0;
  border-top-right-radius: 0;
}

.bd-placeholder-img {
  font-size: 1.125rem;
  text-anchor: middle;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

@media (min-width: 768px) {
  .bd-placeholder-img-lg {
    font-size: 3.5rem;
  }
}
</style>
