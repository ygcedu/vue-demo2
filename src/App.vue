<template>
  <div id="app">
    你想要：{{ x }}
    <hr/>
    <select multiple v-model="x">
      <option value=""> -</option>
      <option v-for="item in array" :value="item.value" :key="item.value">
        {{item.text}}
      </option>
    </select>
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      x: [],
      array: [
        {text: '抽烟', value: 1},
        {text: '喝酒', value: 2},
        {text: '烫头', value: 3}
      ]
    }
  },
  components: {}
}
</script>