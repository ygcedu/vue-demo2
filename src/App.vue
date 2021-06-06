<template>
  <div id="app">
    你想要：{{x}}
    <label>
      <input name="want" type="radio" v-model="x" :value="1"/>
      <span>抽烟</span>
    </label>
    <label>
      <input name="want" type="radio" v-model="x" :value="2"/>
      <span>喝酒</span>
    </label>
    <label>
      <input name="want" type="radio" v-model="x" :value="3"/>
      <span>烫头</span>
    </label>
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