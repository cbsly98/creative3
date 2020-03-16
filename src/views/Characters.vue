<template>
<div>
  <h1>Characters</h1>
  <div class="home">

    <div class="character" v-for="character in characters" :key="character.id">
      <router-link :to="{name: 'Character', params: {id: character.id}}"><img :src="'images/characters/'+character.character"></router-link>
    </div>
  </div>
</div>
</template>

<script>
export default {
  name: 'Characters',
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
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}

.character {
  margin: 10px;
  transition: all 0.6s cubic-bezier(0.165, 0.84, 0.44, 1);
}

.character:hover {
  transform: scale(1.05, 1.05);
  box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
}
</style>
