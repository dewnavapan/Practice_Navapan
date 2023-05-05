<template>
  <div>
    <input v-model="text" />
    <button @click="gotoHome()">GO</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      text: "",
    };
  },
  methods: {
    gotoHome() {
      this.$router.push({ path: "/", query: { msg: this.text } });
    },
  },
};
</script>