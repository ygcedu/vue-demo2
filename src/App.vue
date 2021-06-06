<template>
  <div id="app">
    登录
    <form @submit.prevent="onSubmit">
      <span>用户名</span>
      <label>
        <input type="text" v-model="user.username"/>
      </label>
      <span>密码</span>
      <label>
        <input type="password" v-model="user.password"/>
      </label>
      <button>登录</button>
    </form>
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      x: [],
      user: {
        username: '',
        password: ''
      }
    }
  },
  methods: {
    onSubmit() {
      console.log(this.user);
    }
  },
  components: {}
}
</script>