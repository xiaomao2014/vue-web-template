<template>
  <div>
    <h1>{{ $route.meta.title || 'User list'}}</h1>
    <el-button type="primary">Primary button</el-button>
    <el-button type="primary" @click="goToEdit">用户编辑列表1</el-button>
    <router-link to="/users/edit">用户编辑列表2</router-link>
    <base-test></base-test>
    <base-input></base-input>
  </div>
</template>

<script>
export default {
  methods: {
    goToEdit () {
      // this.$router.replace('/users/edit')
      this.$router.push('/users/edit')
    }
  }

}
</script>

<style lang="scss">
h1 {
  color: $--color-success;
}
</style>
