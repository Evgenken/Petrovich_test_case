<template>
  <div id="app">
    <Petrovich />
  </div>
</template>

<script>
import Petrovich from "@/components/Petrovich/petrovich";
export default {
  name: 'App',
  components: {Petrovich}
}
</script>
<style lang="scss">
@font-face {
  font-family: "Graphik Cy";
  src: url("/src/assets/Graphik Cy.ttf") format("truetype");
}
</style>

