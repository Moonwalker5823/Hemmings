<template>
  <div id="popularCat">
    <h2 class="popularCatHeading">Browse Popular Catagories</h2>
    <div class="catagories">
      <button><font-awesome-icon icon="fa-solid fa-car" /> Classics</button>
      <button>
        <font-awesome-icon icon="fa-solid fa-truck-monster" /> Truck & SUV
      </button>
      <button><font-awesome-icon icon="fa-solid fa-car" /> Muscle Cars</button>
      <button>
        <font-awesome-icon icon="fa-solid fa-gauge" /> Sports & Exotics
      </button>
      <button>
        <font-awesome-icon icon="fa-solid fa-motorcycle" /> Motorycycles
      </button>
      <button>
        <font-awesome-icon icon="fa-solid fa-car-side" /> Restomods & Customs
      </button>
    </div>
    <h2 class="popularCatHeading">Popular Makes</h2>
    <div class="popswipper">
      <img src="../assets/bmw.jpeg" />
      <img src="../assets/jag.jpeg" />
      <img src="../assets/Mer.jpeg" />
      <img src="../assets/ferrarri.png" />
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
#popularCat {
  display: block;
  height: 90%;
  width: 100%;
}

.popularCatHeading {
  font-size: 35px;
  padding: 3rem;
}

.popswipper {
  display: flex;
  justify-content: space-evenly;
}

.popswipper img {
  height: 100px;
}

.catagories {
  display: grid;
  gap: 5px;
  grid-template-columns: repeat(3, 1fr);
  padding: 0 5rem;
}

.catagories button {
  padding: 2rem;
  font-size: 20px;
}
</style>
