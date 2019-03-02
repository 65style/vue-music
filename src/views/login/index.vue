<template>
  <div class="vm-login">
    <div class="login-content">
      <div class="logo">
        <svg-icon
          icon-class="logo2"
          class-name="logo-class"
        ></svg-icon>
      </div>
      <router-link
        class="btn-login"
        to="/login/phone"
      >手机号登陆</router-link>
      <router-link
        class="btn-login"
        to="/login/email"
      >邮箱登录</router-link>
      <router-view></router-view>
    </div>
  </div>
</template>

<style lang="scss">
.vm-login {
  width: 100%;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  background: url(~@/assets/login-bg.jpg) no-repeat;
  background-size: cover;

  .login-content {
    width: 80%;
    height: auto;

    .logo {
      padding: p2r(0.5rem);
      .logo-class {
        display: block;
        margin: 0 auto;
        width: 230px;
        height: 44px;
      }
    }

    .btn-login {
      display: block;
      line-height: p2r(0.8rem);
      border: 1px solid $primary_color;
      color: #fff;
      font-size: $f_auto_l;
      border-radius: p2r(0.5rem);
      margin: p2r(0.3rem) 0;
    }
  }
  .login-ruoter {
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    overflow: hidden;
  }
}
</style>
