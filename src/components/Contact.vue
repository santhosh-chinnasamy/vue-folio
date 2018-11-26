<template>
  <div>
    <h2 class="heading">Contact</h2>
    <div>
      <ul class="links">
        <li class="social" v-for="item in social" :key="item.id">
          <a :href="item.url" target="_blank">{{item.title}}</a>
        </li>
      </ul>


    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      break1: "<br/>",
      social: [
        {
          id: 1,
          title: "LinkedIn",
          url: "https://www.linkedin.com/in/santhosh-chinnasamy/",
          icon: "fab fa-twitter"
        },
        {
          id: 2,
          title: "Github",
          url: "https://github.com/santhosh-chinnasamy"
        },
        {
          id: 3,
          title: "Twitter",
          url: "https://twitter.com/santhosh_in_dev"
        },
        {
          id: 4,
          title: "Blog",
          url: "https://bleedbytes.in"
        },
        {
          id: 5,
          title: "Email",
          url: "mailto:csesanthosh15@gmail.com?subject=from portfolio"
        },{
          id:6,
          title:"Instagram",
          url:"https://www.instagram.com/santh0.sh/"
        }
      ]
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
a {
  color: #42b883;
}

.social {
  font-weight: bold;
  display: inline-flex;
  padding: 10px;
  font-size: 13vmin;
  font-family: "Roboto", Tahoma, Geneva, Verdana, sans-serif;
}
li {
  list-style: none;
}
</style>
