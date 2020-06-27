<template>
  <v-row class="d-flex justify-center">
    <v-col cols="12" sm="8" md="6" class="d-flex justify-center">
      <img :height="800" :width="500" src="../assets/img/aboutMe.png">
    </v-col>
    <v-col cols="12" sm="8" md="6" class="d-flex justify-center">
      <span>
        <br>
        <br>
        <br>
        <h3>My name is Scarlett Tran.</h3>
        <h3 class="mt-5"> I am a third year student at the University of Toronto Mississauga, pursuing Finance specialist and Economics major.   </h3>
        <h3 class="mt-5">I have always been motivated to research the principle of behaviors and ideologies, whether it is from a movies or theories in lectures. I am always eager to learn more and go beyond textbooks themselves. I am passionate in pursuing innovations that are backed by a true technological or social leap. During my journey, I started to learn how to apply what I learned in lectures into my daily life. Therefore, I created the society for Algorithmic Modeling as a place for people to break their boundaries and find the encouragement to unleash their wildest ideas .</h3>
        <h3 class="mt-5">I often see myself as the bridge connecting people from different programs and backgrounds during groupwork, especially between technology and business. Coming from a business background, I constantly worked with a group of talented programmers, mathematicians and statisticians to help them apply their extraordinary knowledge into something applicable. </h3>
        <h3 class="mt-5">I hope you enjoy browsing through my website and learn a bit more about me.</h3>
      </span>
    </v-col>
  </v-row>
</template>

<script>
export default {
  computed: {
    imageSize() {
      switch (this.$vuetify.breakpoint.name) {
        case "xs":
          return "300px";
      }
      return "550px";
    }
  }
};
</script>

<style scoped>
</style>