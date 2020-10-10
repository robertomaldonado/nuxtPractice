<template>
  <div>
    <h3>
      USER NAMES
    </h3>
    <input type="text" v-model="userId">
    <button @click="onLoadUser"> Load User </button>
  </div>
</template>

<script>
export default {
  data(){
    return {
      userId: ""
    }
  },
  methods: {
    onLoadUser(){
      this.$router.push("/users/" + this.userId)
    }
  }
}
</script>