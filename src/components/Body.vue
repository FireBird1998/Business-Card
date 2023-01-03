<template>
  <div class="bodyContainer">
    <div class="align">
    <span>{{ content }}</span>
    <v-btn class="websiteButton"> Website </v-btn>
    </div>
  </div>
</template>

<script>
export default {
  name: "Body_1",
  props: {
    content: {
      default: "",
    },
  },
};
</script>

<style scoped>
.bodyContainer {
  padding: 4vh 8vw;
}
.align {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
.websiteButton {
  margin-top: 20px;
  width: 120px;
  height: 32px;
}
</style>