<template >
    <v-container >
   <Contact />
 </v-container>
</template>

<script>
import Contact from '@/components/Contact'
export default {
 components: {
   Contact,
 
 },
 data() {
   return {
     showMenu: false
   }
 }
}
</script>

<style lang="scss" scoped>
.navigation {
 background-color: #232020;
}
.portfolio-content {
 background-color: #232020;
 height: 100vh;
}
.wrapper {
 position: relative;
}
</style>