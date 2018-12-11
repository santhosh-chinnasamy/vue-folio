<template>
  <v-container fluid>
    <h2 class="heading">Skills</h2>
    <div class="table">
           <ul  class="tech">
            <h2 class="topic">Languages & Frameworks</h2>
            <li v-for="item in tech" :key="item"> {{item}}</li>
            <h2 class="topic">Tools</h2>
            <li v-for="tool in tools" :key="tool">{{tool}}</li>
            <h2 class="topic">Database</h2>
            <li v-for="db in database" :key="db">{{db}}</li>
            <h2 class="topic">Multimedia</h2>
            <li v-for="software in multimedia" :key="software">{{software}}</li>
            <h2 class="topic">Cloud</h2>
            <li v-for="vendor in cloud" :key="vendor">{{vendor}}</li>
            <h2 class="topic">Others</h2>
            <li v-for="other in others" :key="other">{{other}}</li>
      </ul>
    </div>
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      tech: [
        "HTML5,",
        "CSS3,",
        "SASS/SCSS,",
        "Bootstrap, Materialize,",
        "Javascript,",
        "VueJs,",
        "PHP,",
        "Flutter,",
        "Embedded C"
      ],
      database: ["MySQL,", "MongoDB"],
      tools: ["VS Code,", "Android Studio,", "Git,", "CPanel"],
      multimedia: ["Gravit,", "GIMP,", "Adobe Photoshop"],
      cloud: ["Amazon Web Services,", "Google Cloud Platform"],
      OS: ["Ubuntu"],
      others: ["Internet of Things,","Wordpress Developer"]
    };
  }
};
</script>

<style scoped>
.heading {
  font-size: 15vmin;
  font-family: "Finger Paint", cursive;
  font-weight: lighter;
  color: #0d1b2a;
}
.topic {
  margin-top: 5%;
  font-size: 9vmin;
  text-decoration: underline;
}
li {
  display: inline;
  padding: 2px;
  font-weight: bold;
  font-size: 7.2vmin;
  color: #42b883;
  font-family: "Roboto", sans-serif;
}
</style>
