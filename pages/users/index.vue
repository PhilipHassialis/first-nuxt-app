<template>
  <div class="">
    <h1>this is the users page - enter a user and press the button</h1>
    <input type="text" v-model="userId" />
    <button @click="onLoadUser">Load user</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      userId: "",
    };
  },
  methods: {
    onLoadUser() {
      this.$router.push("/users/" + this.userId);
    },
  },
};
</script>
