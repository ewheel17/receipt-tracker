<template>
  <v-app dark>
    <Toolbar :tabs="tabs"/>
    <v-content>
      <v-container>
        <nuxt/>
      </v-container>
    </v-content>
    <BottomToolbar :tabs="tabs"/>
    <!-- <Footer /> -->
  </v-app>
</template>

<script>
import Toolbar from '@/components/layout_components/Toolbar'
import BottomToolbar from '@/components/layout_components/BottomToolbar'
// import Footer from '@/components/layout_components/Footer';

export default {
  components: {
    Toolbar,
    BottomToolbar
    // Footer
  },
  data() {
    return {
      title: 'Receipt Tracker',
      tabs: [
        {
          name: 'Dashboard',
          route: '/',
          icon: 'dashboard'
        },
        {
          name: 'Receipts',
          route: 'receipts',
          icon: 'folder'
        },
        {
          name: 'Add Receipt',
          route: 'add-receipt',
          icon: 'add_circle'
        }
      ]
    }
  }
}
</script>
