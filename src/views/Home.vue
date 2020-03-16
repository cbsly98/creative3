<template>
<div class="home">

</div>
</template>

<script>
export default {
  name: 'Home',
  computed: {
    characters() {
      return this.$root.$data.characters;
    }
  }
}
</script>

<style scoped>
.home {
  height: 100%;
  width: 100%;
}

.character {
  margin: 10px;
}
</style>
