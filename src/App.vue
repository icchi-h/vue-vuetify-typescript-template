<template>
  <v-app>
    <Header />
    <Content />
    <Footer />
  </v-app>
</template>

<script lang="ts">
import { Vue, Component } from "vue-property-decorator";
import Header from "./components/Header.vue";
import Content from "./components/Content.vue";
import Footer from "./components/Footer.vue";

@Component({
  components: {
    Header,
    Content,
    Footer
  }
})
export default class App extends Vue {}
</script>
