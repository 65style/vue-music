<template>
  <div class="sub-login auto-content">
    <div class="content-slot">
      <div class="text-input">
        <svg-icon
          icon-class="phone"
          class-name="icon-phone"
        ></svg-icon>
        <input type="number" placeholder="手机号" v-model="phone">
      </div>
      <div class="text-input">
        <svg-icon
          icon-class="passwd"
          class-name="icon-passwd"
        ></svg-icon>
        <input type="passwrod" placeholder="密码" v-modal="password">
      </div>
      <div class="login-btn">
        <input type="button">
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      type: null,
      phone: '',
      email: '',
      password: ''
    }
  },
  created () {
    this.type = this.$route.params.type
  }
}
</script>
