<script setup>
import {ref} from 'vue'
const Props = defineProps({
  northCountries: Array,
  southCountries: Array
})


const selectedCountry= ref(null)

function countryValue(country){
  selectedCountry.value = country
}

function goBack(){
  selectedCountry.value = null 
}


</script>
<template>
  <div class="container">
    <button
      class="northAmericanCountries"
      v-for="country in northCountries"
      :key="country.name"
      @clicked = countryValue(country)
      >
        {{ northCountry.name }}
    </button>

    <button
      class="SouthAmericanCountries"
      v-for="country in southCountries"
      :key="southCountry.name"
      >
        {{ southCountry.name }}
      </button>
  </div>
</template>

<style scoped>

</style>
