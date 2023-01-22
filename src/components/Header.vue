<template>
    <div class="headerContainer">
        <img src="../assets/tree-736885__480.jpg" class="backgroundImage">
        <div class="profilePicContainer">
        <img src="../assets/profile_pic.webp" class="profilePic">
        <font-awesome-icon icon="fa-solid fa-user-secret" />
        </div>
    </div>
</template>

<script>
export default {
  name: 'Header_1'
}
</script>

<style scoped>
html{
    font-size: 10px;
    
}
.headerContainer {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-content: center;
}
.profilePicContainer{
    display: flex;
    align-content: center;
    justify-content: center;
    padding: 0.5rem;
    margin-top: -7rem;
}
.profilePic {
    height: 12rem;
    width: auto;
    border-radius: 10rem;
    border: 0.5rem solid rgb(255, 255, 255);
}
.backgroundImage {
    height: auto;
    width: auto;
    border-radius: 5px;
    max-height: 400px;
}
</style>