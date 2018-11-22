<template>
  <v-card height="200px" flat>
    <div class="headline text-xs-center pa-5">
      Active: {{ bottomNav }}
    </div>
    <v-bottom-nav
      :active.sync="bottomNav"
      :value="true"
      fixed
      color="transparent"
    >
      <v-btn
        color="teal"
        flat
        value="recent"
      >
        <span>Home</span>
        <v-icon>home</v-icon>
      </v-btn>

      <v-btn
        color="teal"
        flat
        value="favorites"
      >
        <span>About</span>
        <v-icon>info</v-icon>
      </v-btn>

      <v-btn
        color="teal"
        flat
        value="nearby"
      >
        <span>Skills</span>
        <v-icon>book</v-icon>
      </v-btn>

      <v-btn
        color="teal"
        flat
        value="contact"
      >
        <span>Contact</span>
        <v-icon>explore</v-icon>
      </v-btn>
    </v-bottom-nav>
  </v-card>
</template>

<script>
  export default {
    data () {
      return {
        bottomNav: 'recent'
      }
    }
  }
</script>