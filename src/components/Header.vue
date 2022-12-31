<template>
    <div class="backgroundContainer">
        <img src="../assets/tree-736885__480.jpg" class="backgroundImage">
        <img src="../assets/profile_pic.webp" class="profilePic">
    </div>
</template>

<script>
export default {
  name: 'Header_1'
}
</script>

<style scoped>
.backgroundImage {
    height: auto;
    width: 402px;
}
.backgroundContainer {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-content: top;
    padding: 0px;
    margin-left: -4px;
    margin-top: -4px;
}
.profilePic {
    height: 200px;
    width: 200px;
    align-self: center;
    margin-top: -110px;
    border-radius: 100px;
}
</style>