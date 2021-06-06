<template>
  <div id="app">
    <textarea v-model="message" placeholder="editme"/>
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