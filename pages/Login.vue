<template>
  <a-layout :style="{ height: '100vh' }">
    <a-row
      type="flex"
      justify="center"
      align="middle"
      :style="{ height: '100vh' }"
    >
      <a-col :span="7" class="login-container padding-50-40 border-radius-10">
        <a-col :span="24" class="login-logo">
          <h1>
            <Logo />
          </h1>
        </a-col>

        <a-form class="clear-both">
          <a-form-item>
            <Input
              input-name="email"
              input-placeholder="E-Posta Adresi"
              input-type="text"
            />
          </a-form-item>
          <a-form-item>
            <Input
              input-name="password"
              input-placeholder="Şifre"
              input-type="password"
            />
          </a-form-item>
          <a-form-item>
            <a-col :span="12">
              <a-button type="primary" size="large">
                Giriş Yap
              </a-button>
            </a-col>
            <a-col :span="12" class="text-right">
              <ATag href-val="#" text-val="Şifremi unuttum" />
            </a-col>
          </a-form-item>
        </a-form>
      </a-col>
    </a-row>
  </a-layout>
</template>

<script>
import Input from '@/components/forms/input.vue'
import ATag from '@/components/forms/atag.vue'
import Logo from '@/components/SolvuoLogo.vue'

export default {
  layout: 'login',
  components: {
    Input,
    Logo,
    ATag
  }
}
</script>

<style lang="scss">
#__nuxt {
  height: 100%;
  #__layout {
    height: 100%;
    #login-layout {
      height: 100%;
      .login-container {
        background: #fff;
      }
      .padding-50-40 {
        padding: 50px 40px;
      }
      .border-radius-10 {
        border-radius: 10px;
      }
      .login-logo {
        h1 {
          text-align: center;
          color: #d96b53;
          margin: 0 0 35px 0;
          font-size: 40px;
          font-weight: 400;
        }
      }
      .text-right {
        text-align: right;
      }
      .clear-both {
        clear: both;
      }
      .ant-input:focus {
        border-color: #d96b53;
        outline: 0;
        box-shadow: 0 0 0 2px #d96b5340;
        border-right-width: 1px !important;
      }
      .ant-input:hover {
        border-color: #d96b53;
      }
    }
  }
}
</style>
