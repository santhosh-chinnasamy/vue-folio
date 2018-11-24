<template>
  <v-container fluid>
    <h2 class="heading">Skills</h2>
    <div class="table">
           <ul v-for="(item,index) in lists" :key="index" class="tech">
        <v-table>
            <tr>{{item}}</tr>
        </v-table>
      </ul>
    </div>
  </v-container>
</template>

<script>
  export default {
    data() {
      return {
        color: "#42b883",
        lists: ["html", "javascript", "css3", "Vuejs", "PHP", 'MySQL','Git']
      };
    }
  };

</script>

<style scoped>
  .heading {
    font-size: 15vmin;
    font-family: "Finger Paint", cursive;
    font-weight: lighter;
  }

</style>
