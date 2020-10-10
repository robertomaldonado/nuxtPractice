<template>
  <div>
    <h3>
      This is a single user with id: {{ this.$route.params.id }}
    </h3>
  </div>
</template>

<script>
export default {
  validate (data){
    return /^\d+$/.test(data.params.id) //Test for numbers only
  }
}
</script>