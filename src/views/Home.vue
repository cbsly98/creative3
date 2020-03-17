<template>
<div class="home">
  <img class="banner" src="../../public/images/banner.jpg">
  <!-- <img class="poster" src="../../public/images/poster.jpeg"> -->
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
  /* display: grid;
  grid-columns: 100%;
  grid-rows: 50% 50%; */
}

.banner {
  border-radius: 500px;
  /* grid-row-start: 1;
  grid-row-end: 2; */
  /* margin: auto;
  width: 80%;
  vertical-align: center; */
  max-height: 100%;
  max-width: 100%;
  position: absolute;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  margin: auto;
}

/* .poster {
  display: inline-block;
  grid-row-start: 2;
  grid-row-end: 3;
  margin: auto;
  margin-top: 20px;
  width: 70%;
} */
</style>
