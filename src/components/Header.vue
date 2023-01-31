<template>
    <div class="headerContainer">
        <v-img
              src="https://picsum.photos/350/165?random"
              height="125"
              cover
              class="bg-grey-lighten-2"
            ></v-img>
        <v-avatar
            size="80"
        >
        <v-img
              src="https://picsum.photos/350/165?random"
              height="125"
              cover
              class="bg-grey-lighten-2"
            ></v-img>    
        </v-avatar>  
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

</style>