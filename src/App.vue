<template>
  <div>
    <Header></Header>
    <Body :content="about"></Body>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Body from "./components/Body.vue";

export default {
  name: "App",
  components: {
    Header,
    Body,
  },
  data() {
    return {
      about:
        "The reservoir water level continued to lower while we enjoyed our long shower. His thought process was on so many levels that he gave himself a phobia of heights. The lake is a long way from here. The worst thing about being at the top of the career ladder is that there's a long way to fall.",
    };
  },
};
</script>

<style>

</style>
