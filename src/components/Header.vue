<template>
    <div class="headerContainer">
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
.headerContainer {
    display: flex;
    flex-direction: column;
    justify-content: center;
}
.profilePic {
    height: 200px;
    width: 200px;
    align-self: center;
    margin-top: -110px;
    border-radius: 100px;
}
.backgroundImage {
    height: auto;
    width: auto;
}
</style>