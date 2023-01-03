<template>
  <div id="mainListing">
    <div class="carBox">
      <img src="../assets/Eleanor.jpeg" alt="Eleanor" />
      <h2 class="carBoxHeading">
        1,290-Mile, 760 Horsepower 2021 Ford Mustang Shelby GT500
      </h2>
      <div class="cbContext">
        <p class="cbText">Price</p>
        <p class="cbPrice">$82,000</p>
      </div>
    </div>
    <div class="carBox">
      <img src="../assets/Eleanor.jpeg" alt="Eleanor" />
      <h2 class="carBoxHeading">
        1,290-Mile, 760 Horsepower 2021 Ford Mustang Shelby GT500
      </h2>
      <div class="cbContext">
        <p class="cbText">Price</p>
        <p class="cbPrice">$82,000</p>
      </div>
    </div>
    <div class="carBox">
      <img src="../assets/Eleanor.jpeg" alt="Eleanor" />
      <h2 class="carBoxHeading">
        1,290-Mile, 760 Horsepower 2021 Ford Mustang Shelby GT500
      </h2>
      <div class="cbContext">
        <p class="cbText">Price</p>
        <p class="cbPrice">$82,000</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
#mainListing {
  display: flex;
  justify-content: center;
  background-color: whitesmoke;
  height: 50vh;
  padding: 2rem 5rem;
  gap: 3rem;
}

.carBox {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  border: 1px solid grey;
  border-radius: 10px;
}

.carBox > img {
  height: 60%;
  width: 100%;
  border-radius: inherit;
}

.carBoxHeading {
  font-size: 25px;
  inline-size: 550px;
  overflow-wrap: break-word;
  padding: 1rem;
}

.cbText {
  font-size: 25px;
  color: gray;
}

.cbPrice {
  font-size: 32px;
  font-weight: bold;
}
.cbContext {
  padding: 1rem;
}
</style>
