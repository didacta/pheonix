<template>

<div>
  <div class="layout">
    <link href="https://fonts.googleapis.com/css?family=Alfa+Slab+One" rel="stylesheet"> 
    <header class="header">
      <strong>
        <g-link :to="{ name: 'home' }">Gridsome</g-link>
      </strong>
      <nav class="nav">
        <g-link class="nav__link" :to="{ name: 'home' }">Home</g-link>
        <g-link class="nav__link" :to="{ name: 'about' }">About</g-link>
      </nav>
    </header>
    
  </div>
    <card/>  
    

</div>
</template>
<script>
// @ is an alias to /src
import Card from "@/components/Card.vue";
export default {
  name: "home",
  components: {
    Card
  }
};
</script>
<style>
body {
  font-family: "Alfa Slab One", cursive;
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
  width: 100%;
  font-size: 30px;
  background-color: rgba(167, 179, 247, 0.726);
  box-shadow: 2px 2px 5px black;
  color: #6b78cd;
  padding: 15px;
  margin: 10px;
  font-family: "Alfa Slab One", cursive;
}

a:link {
  text-decoration: none;
  color: #4158d0;
}

a:visited {
  text-decoration: none;
  color: #6b78cd;
}

a:hover {
  text-decoration: underline;
  color: rgb(65, 84, 207);
}

a:active {
  text-decoration: underline;
  color: rgb(61, 82, 214);
}
.nav__link {
  margin-left: 20px;
  font-size: 20px;
}
</style>
