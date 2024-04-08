<template>

    <div class="content">
      <h1 class="title">Tarieven</h1>
      <p class="introduction">Korte inleiding</p>
      <p class="description">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
      </p>
      <div class="price-container">
        <div class="price-box">
          <p class="price">Prijs</p>
          <button class="buy-button">Kopen</button>
        </div>
        <div class="price-box">
          <p class="price">Prijs</p>
          <button class="buy-button">Kopen</button>
        </div>
        <div class="price-box">
          <p class="price">Prijs</p>
          <button class="buy-button">Kopen</button>
        </div>
      </div>
    </div>
    <footer>
      <p class="footer-content">Footer</p>
    </footer>

</template>

<script setup>

</script>

<style scoped>
/* Adjusted the layout, colors, and typography to match the new design */
.container {
  font-family: 'Arial', sans-serif;
  max-width: 1200px;
  margin: 0 auto;
  padding: 20px;
}
.navigation .nav-list {
  list-style: none;
  padding: 0;
  display: flex;
  justify-content: center;
  gap: 40px;
}
.nav-list li {
  cursor: pointer;
}
.nav-list li.active {
  border-bottom: 3px solid #000;
  padding-bottom: 5px;
}
.content {
  text-align: center;
  margin-top: 20px;
}
.title {
  margin-bottom: 10px;
}
.introduction {
  font-size: 18px;
  font-weight: bold;
  margin-bottom: 15px;
}
.description {
  margin-bottom: 30px;
}
.price-container {
  display: flex;
  justify-content: space-around;
  align-items: center;
}
.price-box {
  border: 2px solid #000;
  padding: 20px;
  width: 200px;
  height: 100px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-between;
}
.buy-button {
  background-color: transparent;
  padding: 10px 20px;
  cursor: pointer;
  border: 2px solid #000;
  transition: background-color 0.3s ease;
}
.buy-button:hover {
  background-color: #000;
  color: #fff;
}
footer {
  border-top: 2px solid #000;
  padding: 10px 0;
  margin-top: 30px;
}
.footer-content {
  text-align: center;
}
</style>
