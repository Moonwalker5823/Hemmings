<template>
  <div id="mainSearch">
    <h1 class="mainHeading">
      Find the perfect classic car or classic car part
    </h1>
    <form
      @click.prevent="searching('search.make', 'year1', 'year2')"
      class="mainSearch"
    >
      <select v-model="search.make">
        <option value="">Make</option>
        <option value="abarth">Abarth</option>
        <option value="Acura">Acura</option>
        <option value="Benz">Benz</option>
        <option value="Chevy">Chevy</option>
        <option value="Ducati">Ducati</option>
        <option value="Fisker">Fisker</option>
        <option value="Ford">Ford</option>
        <option value="Mayback">Mayback</option>
        <option value="Nissan">Nissan</option>
        <option value="Toyota">Toyota</option>
      </select>
      <select v-model="search.year1">
        <option value="">Year</option>
        <option value="2023">2023</option>
        <option value="2022">2022</option>
        <option value="2021">2021</option>
        <option value="2020">2020</option>
        <option value="2019">2019</option>
        <option value="2018">2018</option>
        <option value="2017">2017</option>
        <option value="2016">2016</option>
      </select>
      to
      <select v-model="search.year2">
        <option value="">Year</option>
        <option value="2023">2023</option>
        <option value="2022">2022</option>
        <option value="2021">2021</option>
        <option value="2020">2020</option>
        <option value="2019">2019</option>
        <option value="2018">2018</option>
        <option value="2017">2017</option>
        <option value="2016">2016</option>
      </select>
      <button>Find it</button>
    </form>
    <a id="mainLink" href="#">Advanced Search</a>
  </div>
</template>

<script>
export default {
  data() {
    return {
      search: {
        make: "",
        year1: 0,
        year2: 0,
      },
      searchValue: {
        value: "",
      },
    };
  },
  methods: {
    searching(payload) {
      console.log(this.search);
      console.log(payload);
      this.searchValue.value = `${this.search.make} ${this.search.year1} - ${this.search.year2}`;
      console.log(this.searchValue);
    },
  },
};
</script>

<style scoped>
#mainSearch {
  background-image: url("../assets/search-bar-mustang-bg.png");
  background-size: cover;
  background-color: #00193a;
  opacity: 1;
  width: 94%;
  height: 10vh;
  border: 2px solid black;
  padding: 3rem 2rem;
}
.mainHeading {
  text-align: center;
  color: white;
  margin-bottom: 15px;
}
.mainSearch {
  display: flex;
  justify-content: center;
  align-items: center;
  color: white;
  gap: 5px;
  font-size: 25px;
}
.mainSearch > select:first-of-type {
  height: 50px;
  width: 180px;
  border-radius: 5px;
}
.mainSearch > select {
  height: 50px;
  width: 80px;
  border-radius: 5px;
  font-size: 16px;
  color: gray;
}
.mainSearch > button {
  padding: 0.5rem 5rem;
  background-color: red;
  border-radius: 10px;
  color: white;
  border: 2px solid red;
}
#mainLink {
  display: flex;
  justify-content: center;
  margin-top: 2rem;
  color: white;
  font-size: 16px;
}
#mainListing {
  display: flex;
  justify-content: center;
  background-color: whitesmoke;
  height: 50vh;
  padding: 2rem 5rem;
  gap: 3rem;
}
</style>
