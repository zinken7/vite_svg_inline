<template>
  <component :is="currentIcon" />
</template>
<script lang="ts">
  import { computed, defineComponent, defineAsyncComponent } from 'vue'
  export default defineComponent({
    props: {
      name: {
        type: String,
        required: true
      },
    },
    setup(props) {
      const currentIcon = computed(() => defineAsyncComponent(() => import(`../icons/${props.name}.svg?component`))).value
      return {
        currentIcon
      }
    }
  })
</script>