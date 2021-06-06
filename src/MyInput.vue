<template>
  <div class="red wrapper">
    <input :value="_value" @input="_value= $event.target.value"/>
    <input v-model="_value"/>
  </div>
</template>

<script>
export default {
  name: "MyInput",
  props: {
    value: {
      type: String
    }
  },
  computed: {
    _value: {
      get() {
        return this.value
      },
      set(newValue) {
        this.$emit('input', newValue);
      }
    }
  },
  methods: {
    // onInput(e) {
    //
    // }
  }
};
</script>

<style scoped>
.red {
  background: red;
}

.wrapper {
  display: inline-block;
}
</style>