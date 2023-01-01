<template>
<div class="bodyContainer">
<span>{{content}}</span>
<v-btn variant="tonal">
  Button
</v-btn>
</div>
</template>

<script>
export default {
  name: 'Body_1',
  props: {
    content: {
        default: ""
    },
  }
}
</script>

<style scoped>
.bodyContainer {
  padding: 4vh 8vw;
}
</style>