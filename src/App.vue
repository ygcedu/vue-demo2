<template>
  <div id="app">
    {{user}}
    <hr/>登录
    <form @submit.prevent="onSubmit">
      <label>
        <span>用户名</span>
        <MyInput :value="user.username" @input="user.username = $event"/>
      </label>
      <label>
        <span>密码</span>
        <input type="password" v-model="user.password"/>
      </label>
      <button type="submit">登录</button>
    </form>
  </div>
</template>

<script>
import MyInput from "@/MyInput";
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
  components: {MyInput}
}
</script>