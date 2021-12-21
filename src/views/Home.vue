<template>
  <div>
    <ProjectSelection />
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import ProjectSelection from "@/components/ProjectSelection.vue"

@Component({
  components: { ProjectSelection }
})
export default class Home extends Vue {}
</script>
