<template>
  <div class="bodyContainer">
    <div class="align">
    <span>{{ content }}</span>
    <v-btn class="websiteButton" @click="websiteButtonClicked"> Website </v-btn>
    </div>
    <div class="gridCointainer">
        <div class="gridBox"><font-awesome-icon icon="fa-brands fa-linkedin" class="icons" /></div>
        <div class="gridBox"><font-awesome-icon icon="fa-brands fa-github" class="icons" /></div>
        <div class="gridBox"><font-awesome-icon icon="fa-brands fa-facebook" class="icons" /></div>
        <div class="gridBox"><font-awesome-icon icon="fa-brands fa-twitter" class="icons" /></div>
        <div class="gridBox"><font-awesome-icon icon="fa-brands fa-facebook" class="icons" /></div>
        <div class="gridBox"><font-awesome-icon icon="fa-brands fa-facebook" class="icons" /></div>
        <div class="gridBox"><font-awesome-icon icon="fa-brands fa-facebook" class="icons" /></div>
        <div class="gridBox"><font-awesome-icon icon="fa-brands fa-facebook" class="icons" /></div>
        <div class="gridBox"><font-awesome-icon icon="fa-solid fa-user-secret" class="icons" /></div>
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
  methods: {
    websiteButtonClicked() {
      console.log("Button Clicked!");
    }
  }
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
  background-color: black;
  color: yellow;
}
.gridCointainer{
  margin: 2rem 0;
    height: auto;
    width: auto;
    display: grid;
    grid-template: 1fr 1fr 1fr / 1fr 1fr 1fr;
    gap: 20px;
    justify-items: center;
    align-items: center;
}

.gridBox{
    height: 50px;
    width: 50px;
    display: flex;
    align-items: center;
    justify-content: center;
}
.icons{
  height: 30px;
}
</style>