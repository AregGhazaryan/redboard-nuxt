<template>
<welcome/>
</template>

<script>
import Welcome from '~/components/Welcome.vue';

export default {
  components: {
    Welcome
  },
  head() {
    return {
      title: 'Redboard'
    }
  }
}
</script>
