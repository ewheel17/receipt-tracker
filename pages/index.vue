<template>
  <v-layout column justify-center align-center>
    <v-flex xs12 sm8 md6>
      <div class="text-xs-center">
        <!-- <logo />
        <vuetify-logo /> -->
      </div>
      <v-card>
        <v-card-title class="headline"
          >Welcome to the receipt-reader app.</v-card-title
        >
        <v-card-text></v-card-text>
        <v-card-actions>
          <v-btn color="primary" flat nuxt to="/receipts"
            >View Receipts</v-btn
          >
          <v-spacer />
          <v-btn color="primary" flat nuxt to="/add-receipt">Add Receipt</v-btn>
        </v-card-actions>
      </v-card>
    </v-flex>
  </v-layout>
</template>
<script>
export default {}
</script>
