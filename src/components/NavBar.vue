<template>
  <div>
    <div id="navbar">
      <div class="leftNavbox">
        <h1>Hemmings</h1>
        <p>est 1954</p>
      </div>
      <div class="middleNavbox">
        <form class="searchForm">
          <font-awesome-icon
            class="searchIcon"
            icon="fa-solid fa-magnifying-glass"
          />
          <input
            class="searchInput"
            type="text"
            placeholder="Search for vehicles, parts, service"
          />
          <button class="searchButton">Search</button>
        </form>
        <a href="#" class="middleNavboxLink">Auctions</a>
        |
      </div>
      <div class="rightNavBox">
        <font-awesome-icon class="navIcon" icon="fa-solid fa-user" />
        <h2>Sign In</h2>
      </div>
    </div>

    <div id="navBarLinks">
      <li>
        <a href="#">Buy</a>
        <ul class="dropDown_Menu">
          <li><a href="#">Cars for Sale</a></li>
          <li><a href="#">Hemmings Auctions</a></li>
          <li><a href="#">Dealers</a></li>
          <li><a href="#">Upcoming Live Auctions</a></li>
          <li><a href="#">Car parts for Sale</a></li>
          <li><a href="#">Cars Service for Sale</a></li>
        </ul>
      </li>
      <li>
        <a href="#">Sell</a>
        <ul class="dropDown_Menu">
          <li><a href="#">Sell A Car</a></li>
          <li><a href="#">Find Cars Value</a></li>
          <li><a href="#">Sell Car Parts</a></li>
          <li><a href="#">Sell Car Services</a></li>
          <li><a href="#">Sell Real Estate</a></li>
          <li><a href="#">Sell Other</a></li>
        </ul>
      </li>
      <li>
        <a href="#">Research</a>
        <ul class="dropDown_Menu">
          <li><a href="#">Tech 101</a></li>
          <li><a href="#">Find Car's Value</a></li>
          <li><a href="#">Price Guide</a></li>
          <li><a href="#">Buyers Guide</a></li>
          <li><a href="#">Engine Guide</a></li>
        </ul>
      </li>
      <li>
        <a href="#">Entertainment</a>
        <ul class="dropDown_Menu">
          <li><a href="#">Latest</a></li>
          <li><a href="#">Car Culture</a></li>
          <li><a href="#">News</a></li>
          <li><a href="#">How To</a></li>
          <li><a href="#">Builds</a></li>
        </ul>
      </li>
      <li>
        <a href="#">Magazine</a>
        <ul class="dropDown_Menu">
          <li><a href="#">Cars for Sale</a></li>
          <li><a href="#">Hemmings Auctions</a></li>
          <li><a href="#">Dealers</a></li>
          <li><a href="#">Upcoming Live Auctions</a></li>
          <li><a href="#">Car parts for Sale</a></li>
          <li><a href="#">Cars Service for Sale</a></li>
        </ul>
      </li>
      <li>
        <a href="#">Community</a>
        <ul class="dropDown_Menu">
          <li><a href="#">Cars for Sale</a></li>
          <li><a href="#">Hemmings Auctions</a></li>
          <li><a href="#">Dealers</a></li>
          <li><a href="#">Upcoming Live Auctions</a></li>
          <li><a href="#">Car parts for Sale</a></li>
          <li><a href="#">Cars Service for Sale</a></li>
        </ul>
      </li>
      <li>
        <a href="/about">About Us</a>
        <ul class="dropDown_Menu">
          <li><a href="#">Cars for Sale</a></li>
          <li><a href="#">Hemmings Auctions</a></li>
          <li><a href="#">Dealers</a></li>
          <li><a href="#">Upcoming Live Auctions</a></li>
          <li><a href="#">Car parts for Sale</a></li>
          <li><a href="#">Cars Service for Sale</a></li>
        </ul>
      </li>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
#navbar {
  display: flex;
  justify-content: space-around;
  gap: 30px;
  align-items: center;
  padding: 2rem 1rem;
}
.leftNavbox {
  color: #0a6321;
  display: flex;
  justify-content: center;
  flex-direction: column;
  text-align: center;
  gap: 0.5rem;
}

.middleNavbox {
  display: flex;
  gap: 20px;
  align-items: center;
  flex-direction: row;
}
.searchForm {
  flex: 1 1 300px;
  position: relative;
  border-radius: 5px;
  overflow: hidden;
}

.searchInput {
  border: none;
  border: 1px solid black;
  padding: 0 0rem 0 2rem;
  font-size: 19px;
  color: #0a6321;
  border-radius: inherit;
  width: 360px;
  height: 40px;
}

.middleNavboxLink {
  color: black;
  text-decoration: none;
  font-size: 20px;
  font-weight: bold;
}

.searchButton {
  position: absolute;
  left: 330px;
  top: 4px;
  padding: 0.5rem;
  border: 1px solid black;
  background-color: #06456a;
  color: white;
  border-radius: inherit;
  cursor: pointer;
}

.searchIcon {
  position: absolute;
  background: transparent;
  top: 12px;
  padding: 0 5px;
}

.link {
  font-size: 20px;
}

.navIcon {
  display: flex;
  border: 2px solid black;
  border-radius: 50%;
  padding: 7px 7px 0px 7px;
}

.rightNavBox {
  display: flex;
  align-items: center;
  gap: 20px;
  margin-right: 40px;
}

#navBarLinks {
  margin-top: -12px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #0a6321;
  height: 10px;
  padding: 1.5rem 3rem;
  list-style-type: none;
}

#navBarLinks > li > a {
  list-style-type: none;
  color: white;
  font-size: 20px;
  font-weight: bold;
  text-decoration: none;
}

.dropDown_Menu {
  display: none;
}

#navBarLinks li:hover .dropDown_Menu {
  display: block;
  position: absolute;
  left: 0;
  top: 12%;
  background-color: whitesmoke;
}
#navBarLinks li:hover .dropDown_Menu li {
  display: block;
  list-style: none;
  margin: 10px;
}

#navBarLinks li:hover .dropDown_Menu li a {
  text-decoration: none;
}

#navBarLinks li:hover .dropDown_Menu li:hover {
  text-decoration: underline;
  color: #0a6321;
}

#navBarLinks li:hover .dropDown_Menu li:hover {
  color: #0a6321;
}
</style>
