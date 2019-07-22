<template>
  <v-footer app dark class="footer">
    <span>ver. {{ packageJson.version }}</span>
  </v-footer>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import packageJson from "../../package.json";

@Component
export default class Footer extends Vue {
  private packageJson = packageJson;
}
</script>

<style lang="scss" scoped>
.footer {
  justify-content: flex-end;
  padding: 8px;
}
</style>
