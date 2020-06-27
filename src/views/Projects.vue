<template>
  <v-row>
    <v-col cols="12" class="d-flex justify-center">
      <h1 :class="{'small-h1': getMobile, 'med-h1': this.$vuetify.breakpoint.sm}">Projects and Achievements</h1>
    </v-col>
    <v-col cols="12" sm="6" md="4" v-for="(p, i) in projects" :key="i">
      <app-card
        :desc="p.desc"
        :projectName="p.projectName"
        :descriptionOne="p.descriptionOne"
        :descriptionTwo="p.descriptionTwo"
        :website="p.website"
      />
    </v-col>
  </v-row>
</template>

<script>
import AppCard from "../components/AppCard.vue";

export default {
  computed: {
    getMobile() {
      if (this.$vuetify.breakpoint.xs) {
        return true;
      }
      return false;
    }
  },
  data() {
    return {
      projects: [
        {
          desc: "Third place",
          projectName: "Big Data & AI Competition",
          descriptionOne:
            "In an effort to tackle the issue of human traﬃcking and money laundering using techniques in machine learning, my team and I eﬀectively applied the OPTICS algorithm to identify outliers that could be categorized as suspicious transactions.",
          descriptionTwo:
            "During the competition, I then integrated such techniques into real-life solutions and apply the applicable business model and pipeline to our strategy."
        },
        {
          desc: "Amazon Web Services AI/ ML Services winner",
          projectName: "Hack the Six Competition",
          descriptionOne:
            " We created an AI investment solution called Resonance that analyses personal and investment traits to make the best matches between those who want to invest and those who know how to. I asist my team by using basic information provided by ﬁnancial institutions about their clients' ﬁnancial assets as well as past interactions to create a deep and objective measure of interaction quality and maximize it through optimal matches.",
          
        },
        {
          desc: "Innovation Through Education Certificate",
          projectName: "InnovatED",
          descriptionOne: "I did research on ESL students' experience in learning English to collect information concerning what areas ESL students should improve on and how to do so. After analyzing the data, I built an app prototype with interactive tools such as interpersonal language games to ensure ESL students' engagement in class",
        },
        {
          desc: "Project implementation",
          projectName: "AlgoTrade",
          descriptionOne: "Project AlgoTrade is initialized to create a community of students with a passion for quantitative analysis and data science research. Throughout the project, I curated a workﬂow that enhances members’ learning experience and project completeness as well as diversiﬁed teams into Reinforcement Learning, Multi-Factor Investing, and Option Hedging by eﬀectively assess members’ resources, strengths and competencies. As a project leader, as well as a part of the implementation team, I provided ﬁnancial insights to the team and guided members to essential resources whenever help is needed."
       
          
        }
      ]
    };
  },
  components: {
    AppCard
  }
};
</script>

<style scoped>
h1 {
  font-size: 80px;
}
.med-h1 {
  font-size: 60px;
}
.small-h1 {
  font-size: 45px;
}
</style>