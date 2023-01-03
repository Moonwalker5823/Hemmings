<template>
  <div id="auctions">
    <h2 class="auctionHeading">
      Live on Hemmings Auctions <a href="#">View All</a>
    </h2>
    <div class="carBidContainer">
      <div class="carBidBox">
        <img src="../assets/Eleanor.jpeg" alt="Eleanor" />
        <h2>1965 Ford Mustang</h2>
        <div class="auctionInfo">
          <p class="auctionBid">Current Bid: $82,000</p>
          <p class="auctionTime">Ends IN: <span>12h:22m:30sec</span></p>
        </div>
      </div>
      <div class="carBidBox">
        <img src="../assets/Eleanor.jpeg" alt="Eleanor" />
        <h2>1965 Ford Mustang</h2>
        <div class="auctionInfo">
          <p class="auctionBid">Current Bid: $82,000</p>
          <p class="auctionTime">Ends IN: <span>12h:22m:30sec</span></p>
        </div>
      </div>
      <div class="carBidBox">
        <img src="../assets/Eleanor.jpeg" alt="Eleanor" />
        <h2>1965 Ford Mustang</h2>
        <div class="auctionInfo">
          <p class="auctionBid">Current Bid: $82,000</p>
          <p class="auctionTime">Ends IN: <span>12h:22m:30sec</span></p>
        </div>
      </div>
    </div>

    <h2 class="auctionHeading">
      Popular Cars For Sale <a href="#">View All</a>
    </h2>
    <div class="popularCarContainer">
      <div class="carBox">
        <img src="../assets/Eleanor.jpeg" alt="Eleanor" />
        <h2 class="carBoxHeading">2021 Ford Mustang Shelby GT500</h2>
        <div class="cbContext">
          <p class="cbText">Price</p>
          <p class="cbPrice">$82,000</p>
        </div>
      </div>
      <div class="carBox">
        <img src="../assets/Eleanor.jpeg" alt="Eleanor" />
        <h2 class="carBoxHeading">2021 Ford Mustang Shelby GT500</h2>
        <div class="cbContext">
          <p class="cbText">Price</p>
          <p class="cbPrice">$82,000</p>
        </div>
      </div>
      <div class="carBox">
        <img src="../assets/Eleanor.jpeg" alt="Eleanor" />
        <h2 class="carBoxHeading">2021 Ford Mustang Shelby GT500</h2>
        <div class="cbContext">
          <p class="cbText">Price</p>
          <p class="cbPrice">$82,000</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
#auctions {
  margin-top: 2rem;
  height: 70vh;
  padding: 2rem 4rem;
  background-color: whitesmoke;
}

.auctionHeading {
  font-size: 30px;
  font-weight: 300;
}

.auctionHeading a {
  font-size: 16px;
  color: green;
}

.auctionTime span {
  color: red;
}

.carBidContainer {
  display: flex;
  justify-content: center;
  padding: 2rem;
  gap: 1rem;
  font-size: 18px;
}

.auctionInfo {
  display: flex;
  padding: 0.2rem;
}

.carBidContainer h2 {
  font-size: 18px;
}
.carBidBox {
  align-items: flex-start;
  border: 1px solid grey;
  border-radius: 5px;
}

.carBox {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  border: 1px solid grey;
  border-radius: 10px;
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

.popularCarContainer {
  display: flex;
  justify-content: center;
  padding: 2rem;
  gap: 1rem;
  padding: 2rem;
}

.popularCarContainer h2 {
  font-size: 18px;
}

.popularCarContainer .cbContext p {
  font-size: 18px;
}
</style>
