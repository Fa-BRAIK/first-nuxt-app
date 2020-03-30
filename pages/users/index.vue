<template>
  <div>
    This should be the users page
    <input type="text" v-model="userId">
    <button @click="onLoadUser()"> Visit User </button>
  </div>
</template>

<script>
export default {
  data: () => ({
    userId: ''
  }),
  methods: {
    onLoadUser() {
      this.$router.push('/users/' + this.userId)
    }
  }
}
</script>
