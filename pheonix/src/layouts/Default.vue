<template>
  <div class="layout">
    <header class="header">
      <strong>
        <g-link :to="{ name: 'home' }">Gridsome</g-link>
      </strong>
      <nav class="nav">
        <g-link class="nav__link" :to="{ name: 'home' }">Home</g-link>
        <g-link class="nav__link" :to="{ name: 'about' }">About</g-link>
      </nav>
    </header>
    <slot/>
  </div>
</template>

<style>
body {
  background-color:rgba(167, 179, 247, 0.726);
  box-shadow: 2px 2px 5px black;
  font-family: -apple-system, system-ui, BlinkMacSystemFont, "Segoe UI", Roboto,
    "Helvetica Neue", Arial, sans-serif;
  margin: 0;
  padding: 0;
  line-height: 1.5;
}

.layout {
  max-width: 600px;
  margin: 0 auto;
  padding-left: 20px;
  padding-right: 20px;
}

.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
  height: 80px;
  font-size: 30px;
  
  color:#6B78CD;
  
  font-family: "Alfa Slab One", cursive;
}

a:link {
    text-decoration: none;
    color:#4158D0;
}

a:visited {
    text-decoration: none;
      color:#6B78CD;
}

a:hover {
    text-decoration: underline;
    color:rgb(65, 84, 207);
    
}

a:active {
    text-decoration: underline;
    color:rgb(61, 82, 214);
}
.nav__link {
  margin-left: 20px;
  font-size: 20px;
}
</style>
