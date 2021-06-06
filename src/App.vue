<template>
  <div id="app">
    <input v-model="message" placeholder="editme"/>
    <p>Message is: {{ message }}</p>
    <p>
      <button @click="message = 'frank'">set message to frank</button>
    </p>
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      message: 'hi'
    }
  },
  components: {}
}
</script>