<template>
  <div class="container">
    <GlobalHeader />
    <div class="header">
      <nav>
        <ul>
          <li>Home</li>
          <li>Websites</li>
          <li class="active">Tarieven</li>
          <li>Contact</li>
          <li>Offerte</li>
        </ul>
      </nav>
    </div>
    <div class="main-content">
      <h1>Tarieven</h1>
      <p class="intro">Korte inleiding</p>
      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
      <div class="prices">
        <!-- Add your pricing details here -->
        <div class="price-box">
          <h2>Prijs</h2>
          <button>Kopen</button>
        </div>
        <div class="price-box">
          <h2>Prijs</h2>
          <button>Kopen</button>
        </div>
        <div class="price-box">
          <h2>Prijs</h2>
          <button>Kopen</button>
        </div>
      </div>
    </div>
    <footer>
      <p>Footer</p>
    </footer>
  </div>
</template>

<script setup>
import GlobalHeader from '../components/GlobalHeader.vue'
</script>

<style scoped>
.container {
  width: 100%;
  max-width: 1200px;
  margin: 0 auto;
}
.header nav ul {
  list-style: none;
  padding: 0;
  display: flex;
  justify-content: space-between;
}
.header nav ul li {
  display: inline;
}
.header nav ul li.active {
  font-weight: bold;
}
.main-content {
  text-align: center;
}
.intro {
  font-style: italic;
}
.prices {
  display: flex;
  justify-content: space-around;
}
.price-box {
  border: 1px solid #000;
  padding: 20px;
  margin: 20px;
  text-align: center;
}
footer {
  text-align: center;
  padding: 20px 0;
}
</style>
