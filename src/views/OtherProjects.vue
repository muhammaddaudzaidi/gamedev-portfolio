<template>
  <div>
    <h1>Game Jam Submissions</h1>

    <div style="margin-bottom: 30px;">
      And here are the submissions from the two game jams that I have participated in. More to follow soon ; ).
    </div>
    <ProjectsList v-bind:projects="projects" />
  </div>
</template>

<script lang="ts">
import Vue from "vue";
import ProjectsList from "@/components/ProjectsList.vue";
import otherProjectsData from "@/data/OtherProjectsData.ts";

export default Vue.extend({
  name: "OtherProjects",
  components: {
    ProjectsList,
  },
  data: function () {
    return {
      projects: otherProjectsData,
    };
  },
});
</script>
