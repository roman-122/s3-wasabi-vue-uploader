<template>
  <v-app-bar
    :clipped-left="primaryDrawer.clipped"
    app
    color="background"
  >
    <v-app-bar-nav-icon
      v-if="primaryDrawer.type !== 'permanent'"
      @click.stop="primaryDrawer.model = !primaryDrawer.model">
    </v-app-bar-nav-icon>
    <v-spacer></v-spacer>
    <v-toolbar-title>LotBlok Blockchain Link</v-toolbar-title>
    <v-spacer></v-spacer>
  </v-app-bar>
</template>

<script>
  export default {
    name: 'Header',
    props: {
      primaryDrawer: {
        type: Object,
        default: () => {},
      }
    }
  }
</script>

<style scoped>

</style>