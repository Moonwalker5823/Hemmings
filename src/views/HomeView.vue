<script setup>
import NavBar from "../components/NavBar.vue";
import MainSearch from "../components/MainSearch.vue";
import MainListings from "../components/MainListings.vue";
import PopularCatagory from "../components/PopularCatagory.vue";
import AuctionList from "../components/AuctionsList.vue";
</script>

<template>
  <nav>
    <NavBar />
  </nav>
  <header>
    <MainSearch />
  </header>
  <main>
    <MainListings />
    <PopularCatagory />
    <AuctionList />
  </main>
</template>
