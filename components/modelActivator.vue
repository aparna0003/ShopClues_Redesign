<template>
  <v-row justify="center">
    <v-dialog v-model="dialog" persistent max-width="290">  <!-- persistent means to maintain their memory when they are called-->
      <template v-slot:activator="{ on, attrs }">  <!-- declaring the attributes-->
        <v-btn
          color="primary"
          dark
          v-bind="attrs"
          v-on="on"
        >
          Open Dialog
        </v-btn>
      </template>
      <v-card>
        <v-card-title class="headline">Use Google's location service?</v-card-title>
        <v-card-text>Let Google help apps determine location. This means sending anonymous location data to Google, even when no apps are running.</v-card-text>
        <v-card-actions>
          <v-spacer></v-spacer>
          <v-btn color="green darken-1" text @click="dialog = false">Disagree</v-btn> <!--to show the appearence and dissapearence of the dialoge box-->
          <v-btn color="green darken-1" text @click="dialog = false">Agree</v-btn>
        </v-card-actions>
      </v-card>
    </v-dialog>
  </v-row>
</template>

<script>
  export default {
    data () {
      return {
        dialog: false, // to know when it has to dropdown or not
      }
    },
  }
</script>