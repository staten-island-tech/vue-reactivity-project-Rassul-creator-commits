<script setup>
import { ref } from 'vue'

const props = defineProps({
  northCountries: Array,
  southCountries: Array
})

const selectedCountry = ref(null)

function countryClicked(country) {
  selectedCountry.value = country
}

function goBack() {
  selectedCountry.value = null
}
</script>

<template>
  <div class="container">
    <div v-if="!selectedCountry">
      <h2>North America</h2>
      <button
        v-for="country in props.northCountries"
        :key="country.name"
        @click="countryClicked(country)"
      >
        {{ country.name }}
      </button>

      <h2>South America</h2>
      <button
        v-for="country in props.southCountries"
        :key="country.name"
        @click="countryClicked(country)"
      >
        {{ country.name }}
      </button>
    </div>

    <div v-if="selectedCountry">
      <h2>{{ selectedCountry.name }}</h2>
      <p>Population: {{ selectedCountry.population }}</p>
      <p>Education Rate: {{ selectedCountry.educationRate }}</p>
      <p>Life Expectancy: {{ selectedCountry.lifeExpectancy }}</p>
      <p>Infant Mortality: {{ selectedCountry.infantMortality }}</p>
      <p>Median Age: {{ selectedCountry.medianAge }}</p>
      <button @click="goBack">Go Back</button>
    </div>
  </div>
</template>