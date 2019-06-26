<template>
  <v-layout column justify-center align-center>
    <v-flex xs12 sm8 md6>
      <v-card>
        <v-card-title class="headline">Health Receipt Tracking</v-card-title>
        <v-card-text>
          <p>
            Welcome to my app for tracking receipts. This application is designed with
            a specific goal in mind, to track my health related expenditures that will qualify
            as deductions from an HSA later in life.
          </p>
          <p>
            With this knowledge, understand that this may not be the most well-suited app for general
            receipt tracking. I will, however, try to develop it in such a way that allows for more
            general use in the future.
          </p>
        </v-card-text>
        <v-card-actions>
          <v-spacer/>
          <v-btn color="primary" flat nuxt to="/receipts">View Receipts</v-btn>
          <v-btn color="primary" flat nuxt to="/add-receipt">Add Receipt</v-btn>
          <v-spacer/>
        </v-card-actions>
      </v-card>
    </v-flex>
  </v-layout>
</template>
<script>
export default {}
</script>
