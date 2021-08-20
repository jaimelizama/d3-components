<template>
  <div class="container mt-5 list">
    <ul>
      <li v-for="(character, $index) in characters" :key="$index">
        <img class="character-img my-3" :src="character.src" />
        <p class="character-name ml-5">{{ character.name }}</p>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'List',

  data: () => ({
    characters: [
      {
        name: 'Rick Sanchez',
        src: 'https://rickandmortyapi.com/api/character/avatar/1.jpeg'
      },
      {
        name: 'Morty Smith',
        src: 'https://rickandmortyapi.com/api/character/avatar/2.jpeg'
      }
    ]
  })
}
</script>

<style>
.list li p {
  display: inline-block;
}

.character-img {
  height: 150px;
  width: 150px;
  border-radius: 50%;
}
.character-name {
  color: green;
  font-size: 24px;
  font-weight: 700;
  font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande',
    'Lucida Sans', Arial, sans-serif;
}
</style>
