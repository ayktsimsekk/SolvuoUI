<template>
  <a-layout-header>
    <a-row>
      <a-col :span="8">
        <Logo />
      </a-col>
      <a-col :span="8">
        <ul class="haeder-menu">
          <li>
            <ATag href-val="#" text-val="Talep Oluştur" class-val="active" />
          </li>
          <li>
            <ATag href-val="#" text-val="Talep Listem" />
          </li>
          <li>
            <ATag href-val="#" text-val="Yardım Dokümanları" />
          </li>
        </ul>
      </a-col>
      <a-col :span="8" class="text-right">
        <a-avatar icon="user" /> &nbsp;Aykut ŞİMŞEK
      </a-col>
    </a-row>
  </a-layout-header>
</template>

<script>
import Input from '@/components/forms/input.vue'
import ATag from '@/components/forms/atag.vue'
import Logo from '@/components/SolvuoLogo.vue'

export default {
  name: 'Header',
  components: {
    Logo,
    ATag
  }
}
</script>

<style scoped lang="scss">
.ant-layout-header {
  background: #f6f6f6;
  padding-top: 30px;
  padding-bottom: 30px;
  height: auto;
  line-height: normal;
}
ul.haeder-menu {
  margin: 0;
  padding: 0;
  li {
    float: left;
    list-style-type: none;
    padding: 0 10px;
    a {
      color: #444;
      padding: 10px 15px;
      border-radius: 7px;
    }
    a.active {
      background-color: #4dcc87;
      color: #fff;
    }
  }
}
.text-right {
  text-align: right;
}
</style>
