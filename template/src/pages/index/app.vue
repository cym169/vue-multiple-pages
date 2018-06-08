<template>
  <div id="app">
    <el-card class="index-card">
      <div slot="header">
        My Codes
      </div>
      <ul>
        <li>
          <a href="https://github.com/cym169/vue-multiple-pages" target="_blank">
            Vue Multiple Pages
          </a>
        </li>
      </ul>
      <el-button type="primary" plain @click="tototo">To User Login Page</el-button>
    </el-card>
  </div>
</template>

<script>
  import logo from 'assets/img/logo.png'
  import modal from 'components/modal.vue'
  export default {
    components: {
      modal
    },
    data () {
      return {
        msg: 'Use Vue 2.0 Today!',
        logoImg: logo
      }
    },
    methods: {
      tototo () {
        location.assign('../login.html')
      }
    }
  }
</script>

<style lang="postcss">
  .index-card {
    width: 800px;
    margin: 100px auto;
  }
</style>
