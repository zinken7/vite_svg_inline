<template>
  <SvgIcon name="sun" style="width: 200px" />
</template>
<script lang="ts">
  import { defineComponent } from 'vue'
  import SvgIcon from "./components/SvgIcon.vue"
  export default defineComponent({
    components: {
      SvgIcon
    }
  })
</script>
<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
