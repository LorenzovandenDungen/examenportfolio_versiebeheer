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
  // You can add your script content here if needed
};
</script>

<style scoped>
.container {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}

.header {
  background-color: #FFC107;
  display: flex;
  justify-content: space-between;
  padding: 1rem;
  align-items: center;
}

.logo {
  /* Adjust this as necessary */
  width: 150px;
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
  flex-grow: 1;
}

.content {
  display: flex;
  justify-content: space-between;
  flex-grow: 2; /* Allows this section to take up more space */
}

.content-block {
  display: flex;
  flex-direction: column;
  align-items: center;
  flex-basis: calc(33.333% - 2rem);
  margin: 1rem;
}

.image-placeholder {
  width: 100%;
  height: 150px;
  background-color: #ddd;
  margin-bottom: 1rem;
}

.text-placeholder {
  width: 100%;
  height: 2rem;
  background-color: #eee;
  margin-bottom: 1rem;
}

.features {
  background-color: #90CAF9;
  display: flex;
  justify-content: space-between;
  flex-grow: 1;
}

.feature-block {
  background-color: #fff;
  padding: 1rem;
  flex-basis: calc(33.333% - 2rem);
  margin: 1rem;
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
  margin-top: auto; /* Pushes footer to the bottom */
}
</style>
