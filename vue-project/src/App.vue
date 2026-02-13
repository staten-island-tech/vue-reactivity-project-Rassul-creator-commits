
<template>
  <div>
     <div class="container">
      <div v-for="northAmericanCountry in northAmericanCountries : key"northAmericanCountries.name">
  </div>
</div>
</div>
  <h1></h1>
  <p>
    
    Visit <a href="https://vuejs.org/" target="_blank" rel="noopener">vuejs.org</a> to read the
    documentation
  </p>
</template>
<script setup>
const northAmericanCountries = [
  {
    name: "United States",
    population: 342000000,
    educationRate: "50.1% (Tertiary)",
    lifeExpectancy: 79.8,
    infantMortality: 5.2,
    medianAge: 38.9
  },
  {
    name: "Mexico",
    population: 129500000,
    educationRate: "24.0% (Tertiary)",
    lifeExpectancy: 75.4,
    infantMortality: 11.5,
    medianAge: 30.5
  },
  {
    name: "Canada",
    population: 40100000,
    educationRate: "62.7% (Tertiary)",
    lifeExpectancy: 83.1,
    infantMortality: 4.1,
    medianAge: 41.2
  },
  {
    name: "Guatemala",
    population: 18400000,
    educationRate: "18.5% (Tertiary)",
    lifeExpectancy: 72.5,
    infantMortality: 21.0,
    medianAge: 24.1
  },
  {
    name: "Haiti",
    population: 11900000,
    educationRate: "12.0% (Tertiary)",
    lifeExpectancy: 64.5,
    infantMortality: 43.2,
    medianAge: 24.8
  },
  {
    name: "Cuba",
    population: 11100000,
    educationRate: "41.0% (Tertiary)",
    lifeExpectancy: 78.5,
    infantMortality: 4.0,
    medianAge: 42.5
  },
  {
    name: "Dominican Republic",
    population: 11400000,
    educationRate: "25.0% (Tertiary)",
    lifeExpectancy: 74.2,
    infantMortality: 22.0,
    medianAge: 28.5
  },
  {
    name: "Honduras",
    population: 10700000,
    educationRate: "16.0% (Tertiary)",
    lifeExpectancy: 72.8,
    infantMortality: 14.5,
    medianAge: 25.1
  },
  {
    name: "Nicaragua",
    population: 7100000,
    educationRate: "19.0% (Tertiary)",
    lifeExpectancy: 75.2,
    infantMortality: 15.0,
    medianAge: 28.1
  },
  {
    name: "El Salvador",
    population: 6400000,
    educationRate: "20.5% (Tertiary)",
    lifeExpectancy: 74.5,
    infantMortality: 11.0,
    medianAge: 28.9
  },
  {
    name: "Costa Rica",
    population: 5200000,
    educationRate: "33.5% (Tertiary)",
    lifeExpectancy: 80.9,
    infantMortality: 7.2,
    medianAge: 34.2
  },
  {
    name: "Panama",
    population: 4500000,
    educationRate: "29.0% (Tertiary)",
    lifeExpectancy: 79.5,
    infantMortality: 11.2,
    medianAge: 30.5
  },
  {
    name: "Jamaica",
    population: 2800000,
    educationRate: "27.0% (Tertiary)",
    lifeExpectancy: 75.8,
    infantMortality: 11.5,
    medianAge: 29.8
  },
  {
    name: "Trinidad and Tobago",
    population: 1500000,
    educationRate: "15.5% (Tertiary)",
    lifeExpectancy: 76.5,
    infantMortality: 10.8,
    medianAge: 37.5
  },
  {
    name: "Bahamas",
    population: 410000,
    educationRate: "22.0% (Tertiary)",
    lifeExpectancy: 74.1,
    infantMortality: 9.2,
    medianAge: 33.2
  },
  {
    name: "Belize",
    population: 415000,
    educationRate: "14.0% (Tertiary)",
    lifeExpectancy: 75.6,
    infantMortality: 11.0,
    medianAge: 25.8
  },
  {
    name: "Barbados",
    population: 282000,
    educationRate: "35.0% (Tertiary)",
    lifeExpectancy: 78.1,
    infantMortality: 8.5,
    medianAge: 40.5
  }
];
const southAmericanCountries = [
  {
    name: "Brazil",
    population: 213562000,
    educationRate: "20.5% (Tertiary)",
    lifeExpectancy: 76.5,
    infantMortality: 10.4,
    medianAge: 35.3
  },
  {
    name: "Colombia",
    population: 53425000,
    educationRate: "30.1% (Tertiary)",
    lifeExpectancy: 78.3,
    infantMortality: 10.5,
    medianAge: 33.0
  },
  {
    name: "Argentina",
    population: 45851000,
    educationRate: "39.5% (Tertiary)",
    lifeExpectancy: 77.8,
    infantMortality: 8.5,
    medianAge: 33.3
  },
  {
    name: "Peru",
    population: 34576000,
    educationRate: "28.0% (Tertiary)",
    lifeExpectancy: 77.9,
    infantMortality: 10.1,
    medianAge: 31.8
  },
  {
    name: "Venezuela",
    population: 28516000,
    educationRate: "15.0% (Tertiary/Est)",
    lifeExpectancy: 72.8,
    infantMortality: 22.9,
    medianAge: 30.5
  },
  {
    name: "Chile",
    population: 19859000,
    educationRate: "41.5% (Tertiary)",
    lifeExpectancy: 81.4,
    infantMortality: 5.6,
    medianAge: 37.1
  },
  {
    name: "Ecuador",
    population: 18289000,
    educationRate: "19.8% (Tertiary)",
    lifeExpectancy: 77.6,
    infantMortality: 11.0,
    medianAge: 29.5
  },
  {
    name: "Bolivia",
    population: 12581000,
    educationRate: "22.0% (Tertiary)",
    lifeExpectancy: 68.6,
    infantMortality: 23.8,
    medianAge: 26.5
  },
  {
    name: "Paraguay",
    population: 7013000,
    educationRate: "18.5% (Tertiary)",
    lifeExpectancy: 73.8,
    infantMortality: 16.9,
    medianAge: 27.2
  },
  {
    name: "Uruguay",
    population: 3384000,
    educationRate: "24.5% (Tertiary)",
    lifeExpectancy: 78.3,
    infantMortality: 7.4,
    medianAge: 36.2
  },
  {
    name: "Guyana",
    population: 835000,
    educationRate: "10.0% (Tertiary)",
    lifeExpectancy: 70.2,
    infantMortality: 24.0,
    medianAge: 28.1
  },
  {
    name: "Suriname",
    population: 639000,
    educationRate: "11.5% (Tertiary)",
    lifeExpectancy: 73.6,
    infantMortality: 14.7,
    medianAge: 30.1
  },
  {
    name: "French Guiana",
    population: 313000,
    educationRate: "16.0% (Tertiary)",
    lifeExpectancy: 77.2,
    infantMortality: 8.1,
    medianAge: 25.8
  },
  {
    name: "Falkland Islands",
    population: 3469,
    educationRate: "99% (Lit)",
    lifeExpectancy: 79.4,
    infantMortality: 4.5,
    medianAge: 46.5
  }
];
</script>
<style scoped></style>
