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
    <v-dialog
      v-model="dialog"
      persistent
      max-width="290"
    >
      <template v-slot:activator="{ on, attrs }">
        <v-btn
          color="primary"
          dark
          v-bind="attrs"
          v-on="on"
        >
          Open Dialog
        </v-btn>
      </template>
      <v-card>
        <v-card-title class="text-h5">
          Use Google's location service?
        </v-card-title>
        <v-card-text>Let Google help apps determine location. This means sending anonymous location data to Google, even when no apps are running.</v-card-text>
        <v-card-actions>
          <v-spacer></v-spacer>
          <v-btn
            color="green darken-1"
            text
            @click="dialog = false"
          >
            Disagree
          </v-btn>
          <v-btn
            color="green darken-1"
            text
            @click="dialog = false"
          >
            Agree
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-dialog>
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