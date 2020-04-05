<template>
<div class="flex flex-col h-screen bg-gray-200">
  <navbar />
  <nuxt />
  <appFooter />
</div>
</template>
<script>
import navbar from '~/components/Navbar.vue';
import appFooter from '~/components/AppFooter.vue';

export default {
  components: {
    navbar,
    appFooter
  }
}
</script>
