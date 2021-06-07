<template>
  <div v-show="!homePage">
    <button class="btn btn__back" @click="goBack">wstecz</button>
  </div>
</template>
<script>
export default {
  name: "GoBack",
  methods: {
    goBack() {
      return this.$router.go(-1);
    },
  },
  computed: {
    homePage() {
      if (this.$route.path == "/" || this.$route.path == "/home") {
        return true;
      } else {
        return false;
      }
    },
  },
};
</script>