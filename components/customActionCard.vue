<template>
  <v-card
    class="mx-auto"
    max-width="344"
  >
    <v-img                <!---link for the picture to be added--->
      src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"   
      height="200px"
    ></v-img>

    <v-card-title>
      Top western road trips
    </v-card-title>

    <v-card-subtitle>
      1,000 miles of wonder
    </v-card-subtitle>

    <v-card-actions>                 <!--to show the button most probably-->
      <v-btn text>Share</v-btn>

      <v-btn
        color="purple"
        text
      >
        Explore
      </v-btn>

      <v-spacer></v-spacer>

      <v-btn             <!when clicked what to happen-->
        icon
        @click="show = !show"  
      >
        <v-icon>{{ show ? 'mdi-chevron-up' : 'mdi-chevron-down' }}</v-icon>
      </v-btn>
    </v-card-actions>

    <v-expand-transition>  <!--the starting of expansion-->
      <div v-show="show">
        <v-divider></v-divider>

        <v-card-text>
          I'm a thing. But, like most politicians, he promised more than he could deliver. You won't have time for sleeping, soldier, not with all the bed making you'll be doing. Then we'll go with that data file! Hey, you add a one and two zeros to that or we walk! You're going to do his laundry? I've got to find a way to escape.
        </v-card-text>
      </div>
    </v-expand-transition>  <!--the closing of expansion-->
  </v-card>
</template>

<script>
  export default {      // boolean condition about when to show
    data: () => ({
      show: false,
    }),
  }
</script>