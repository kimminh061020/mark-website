<template>
<div id="site-wrapper">
<AppHeader />
<Nuxt />
<AppFooter />
</div>
</template>

<script>
import AppHeader from "../components/AppHeader.vue"
import AppFooter from "../components/AppFooter.vue"
export default {
  components: {
    AppHeader,
    AppFooter
  }
}
</script>
<style scoped>
@import "../assets/default.css";

#site-wrapper {
    min-height: 100vh;
        display: flex;
        flex-direction: column;
    }
</style>