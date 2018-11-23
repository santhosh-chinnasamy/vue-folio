<template>
  <v-card height="200px" flat>
    
    <v-bottom-nav
      :value="true"
      fixed
      color="transparent"
    >
    
      <v-btn color="teal" flat to="/"
        router>
        <span>Home</span>
        <v-icon>home</v-icon>
      </v-btn>
      
<!-- <router-link to="/about"></router-link> -->
      <v-btn
        color="teal"
        flat
        to="/about"
        router
      >
        <span>About</span>
        <v-icon>info</v-icon>
      </v-btn>

      <v-btn
        color="teal"
        flat
        to="/skills"
        router
      >
        <span>Skills</span>
        <v-icon>book</v-icon>
      </v-btn>

      <v-btn
        color="teal"
        flat
        to="/contact"
        router
      >
        <span>Contact</span>
        <v-icon>explore</v-icon>
      </v-btn>
    </v-bottom-nav>
  </v-card>
</template>