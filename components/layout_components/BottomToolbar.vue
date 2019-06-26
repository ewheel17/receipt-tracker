<template>
  <v-bottom-nav :value="true" class="hidden-md-and-up">
    <v-btn
      v-for="tab in tabs"
      :key="tab.name"
      nuxt
      :to="tab.route"
      color="teal"
      flat
      value="recent"
    >
      <span>{{ tab.name }}</span>
      <v-icon>{{ tab.icon }}</v-icon>
    </v-btn>
  </v-bottom-nav>
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
