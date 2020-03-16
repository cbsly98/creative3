<template>
<div class="character">
  <h1>{{ character.name }}</h1>
  <p class="quote">"{{ character.quote }}"</p>
  <p class="objective">Objective: {{ character.objective }}</p>
  <img :src="'../../images/characters/'+character.character">
  <p>Realm:</p>
  <img class="board" :src="'../../images/boards/'+character.board">
</div>
</template>

<script>
export default {
  name: 'Character',
  data() {
    return {
      id: 0
    }
  },
  created() {
    this.id = this.$route.params.id;
  },
  computed: {
    character() {
      return this.$root.$data.characters[this.id - 1];
    }
  }
}
</script>

<style scoped>
.board {
  width: 90%;
  margin: auto;
  margin-bottom: 20px;
}

p.quote {
  font-style: italic;
}
</style>
