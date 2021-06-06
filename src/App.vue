<template>
  <div id="app">
    你想要：{{ x }}
    <hr/>
    <select v-model="x">
      <option value=""> -</option>
      <option :value="1">抽烟</option>
      <option :value="2">喝酒</option>
      <option :value="3">烫头</option>
    </select>
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      x: ''
    }
  },
  components: {}
}
</script>