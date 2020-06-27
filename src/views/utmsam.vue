<template>
  <v-row class="d-flex justify-center">
    <v-col cols="12" sm="8" md="6" class="d-flex justify-center">
      <img :height="900" :width="500" src="../assets/img/utmsam.png" />
    </v-col>
    <v-col cols="12" sm="8" md="6" class="d-flex justify-center">
      <span>
        <br>
        <br>
        <br>
        <h3 class="mt-5"> I founded the Society for Algorithmic Modelling (SAM) with the hope of creating a safe place for students to learn from each other regardless of their program.   </h3>
        <h3 class="mt-5"> SAM is a student- run society that discover the application of machine learning, artificial intelligence, data science, algorithm development and mathematical modelling. We encourage STEM students to constantly apply what they learnt in lecture to some cool real-life applications. SAM is also dedicated to bringing talents from the technological aspect and the business aspect together. Cool projects could be created by cross-discipline collaborations. SAM executives are from different program but all have one single goal of exploring every single interesting aspect that come up in their mind, and we would love to share the coolest ideas and concepts that we found with others! We are here to support the students in variety of ways.</h3>
        <h3 class="mt-5"> To me, SAM is not a club, but a family. Throughout my years at University of Toronto, I have learnt how to be a better member, leader and mentor. By actively working with students coming from a technical background, I have gained technical skills and perspective. I hope that SAM will continue to spread its positive influence to a bigger community for the years to come given the culture that we have built within the organization. </h3>
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