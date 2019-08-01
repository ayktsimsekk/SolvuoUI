<template>
  <a-layout-header>
    <Logo />
  </a-layout-header>
</template>

<script>
import Input from '@/components/forms/input.vue'
import ATag from '@/components/forms/atag.vue'
import Logo from '@/components/SolvuoLogo.vue'

export default {
  name: 'Header',
  components: {
    Logo
  }
}
</script>

<style scoped>
.ant-layout-header {
  background: #f6f6f6;
  padding-top: 30px;
  padding-bottom: 30px;
  height: auto;
  line-height: normal;
}
</style>
