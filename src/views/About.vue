<template>
  <div class="about">
    <h1>{{ title }}</h1>
    <TsTesting />
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import TsTesting from "@/components/TsTesting.vue";

@Options({
  components: {
    TsTesting
  }
})
export default class About extends Vue {
  private title = "This is an about page";
}
</script>
