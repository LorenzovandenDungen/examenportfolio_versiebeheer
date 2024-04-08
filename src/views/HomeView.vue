<template>
  <div class="container">
    <header class="header">
      <div class="logo">YOUR LOGO</div>
      <nav class="nav">
        <a href="#home">Home</a>
        <a href="#websites">Websites</a>
        <a href="#tarieven">Tarieven</a>
        <a href="#contact">Contact</a>
        <a href="#offerte">Offerte</a>
      </nav>
    </header>

    <div class="main-banner">
      <button class="main-button">Button</button>
    </div>

    <div class="content">
      <div class="content-block" v-for="i in 3" :key="`content-${i}`">
        <div class="image-placeholder"></div>
        <div class="text-placeholder"></div>
        <button>Button</button>
      </div>
    </div>

    <div class="features">
      <div class="feature-block" v-for="i in 3" :key="`feature-${i}`">
        <div class="text-placeholder"></div>
        <button>Button</button>
      </div>
    </div>

    <footer class="footer">
      Footer
    </footer>
  </div>
</template>

<script>
export default {
  name: 'HomeView'
  // No router used here, so you can remove the import and setup
};
</script>

<style scoped>
.container {
  display: flex;
  flex-direction: column;
  height: 100vh; /* Make the container fill the full viewport height */
}

.header {
  background-color: #FFC107;
  display: flex;
  justify-content: space-between;
  padding: 1rem;
  align-items: center;
}

.logo {
  width: 150px; /* You can adjust this as per your logo's dimensions */
  height: auto;
}

.nav {
  display: flex;
  gap: 1rem;
}

.main-banner {
  background-color: #FFEB3B;
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 2rem;
  flex-grow: 1; /* Take up available space */
}

.content {
  display: flex;
  justify-content: space-around;
  flex-grow: 1; /* Take up available space */
}

.content-block {
  border: 1px solid #000;
  padding: 1rem;
  width: 30%;
}

.image-placeholder {
  background-color: #ddd;
  height: 150px;
  margin-bottom: 1rem;
}

.text-placeholder {
  background-color: #eee;
  height: 2rem;
  margin-bottom: 1rem;
  width: 100%;
}

.features {
  background-color: #90CAF9;
  display: flex;
  justify-content: space-around;
  flex-grow: 1; /* Take up available space */
}

.feature-block {
  background-color: #fff;
  padding: 1rem;
}

.main-button, button {
  background-color: #000;
  color: #fff;
  border: none;
  padding: 0.5rem 1rem;
  cursor: pointer;
}

.footer {
  background-color: #757575;
  color: #fff;
  text-align: center;
  padding: 1rem;
}
</style>
