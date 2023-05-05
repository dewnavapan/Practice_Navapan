<template>
  <div>
    <input :value="text" v-on:input="convertToUpperCase" />
  </div>
</template>

<script>
export default {
  data() {
    return {
      text: "test",
    };
  },
  method: {
    convertToUpperCase(event) {
      this.text = event.target.value.ToUpperCase();
    },
  },
};
</script>