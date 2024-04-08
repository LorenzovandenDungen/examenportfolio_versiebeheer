<template>
  <div class="tarieven-view">
    <header>
      <!-- Navigation goes here -->
    </header>

    <main class="content">
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
    </main>

    <footer>
      <p class="footer-content">Footer</p>
    </footer>
  </div>
</template>

<script setup>
// Import your components or any scripts if needed
</script>

<style scoped>
.tarieven-view {
  font-family: 'Arial', sans-serif;
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}

header {
  /* Add header styles here */
}

.content {
  flex: 1;
  text-align: center;
  padding: 40px 20px;
  max-width: 1200px;
  margin: auto;
}

.title {
  margin-bottom: 1em;
}

.introduction {
  font-size: 20px;
  font-weight: bold;
  margin-bottom: 2em;
}

.description {
  margin-bottom: 3em;
}

.price-container {
  display: flex;
  justify-content: space-evenly;
  flex-wrap: wrap;
  gap: 30px;
}

.price-box {
  border: 1px solid #ccc;
  padding: 2em;
  width: 300px;
  min-height: 150px;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.2);
}

.price {
  font-size: 1.5em;
  font-weight: bold;
}

.buy-button {
  background-color: #fff;
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
  border-top: 1px solid #ccc;
  padding: 1em 0;
  text-align: center;
}

.footer-content {
  margin: 0;
}
</style>
