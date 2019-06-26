<template>
  <v-toolbar fixed app>
    <v-toolbar-title v-text="title"/>
    <v-spacer/>
    <v-toolbar-items class="hidden-sm-and-down">
      <v-btn v-for="tab in tabs" :key="tab.name" nuxt :to="tab.route" flat>{{ tab.name }}</v-btn>
    </v-toolbar-items>
  </v-toolbar>
</template>

<script>
export default {
  props: {
    tabs: Array
  },
  data() {
    return {
      fixed: false,
      title: 'Receipt Tracker'
    }
  }
}
</script>


<style lang="stylus" scoped></style>
