<template>
  <div>
    <!-- harmburger -->
    <div class="navbar">
      <button
        class="harmburger"
        :class="[
        {'opened':toggled}]"
        @click="toggle"
        aria-label="Main Menu"
      >
        <svg width="100" height="100" viewBox="0 0 100 100">
          <path
            class="line line1"
            d="M 20,29.000046 H 80.000231 C 80.000231,29.000046 94.498839,28.817352 94.532987,66.711331 94.543142,77.980673 90.966081,81.670246 85.259173,81.668997 79.552261,81.667751 75.000211,74.999942 75.000211,74.999942 L 25.000021,25.000058"
          />
          <path class="line line2" d="M 40,50 H 80" />
          <path
            class="line line3"
            d="M 20,70.999954 H 80.000231 C 80.000231,70.999954 94.498839,71.182648 94.532987,33.288669 94.543142,22.019327 90.966081,18.329754 85.259173,18.331003 79.552261,18.332249 75.000211,25.000058 75.000211,25.000058 L 25.000021,74.999942"
          />
        </svg>
      </button>
    </div>

    <!-- logo -->

    <div class="logo">
      <img src="../assets/sensei-8-logo.png" alt />
    </div>

    <!-- top navigation -->

    <div class="topnav">
      <ul>
        <li class="navlink">
          <router-link to="/">Home</router-link>
        </li>
        <li class="navlink">
          <router-link to="/about">About</router-link>
        </li>
        <li class="navlink">
          <router-link to="/sensei">Sensei</router-link>
        </li>
        <li class="navlink">
          <router-link to="/contact">Contact</router-link>
        </li>
        <li class="navlink">
          <router-link to="/pricing">Pricing</router-link>
        </li>
      </ul>
    </div>

    <!-- side nav-->

    <div class="side-nav" :class="[
        {'slide': !toggled}]">
<!-- <div class="paatern">  <img src="../assets/Taieri.png" alt=""></div> -->
      
      <ul>
        <li class="side-link" @click="toggle">
          <router-link to="/">Home</router-link>
        </li>
        <li class="side-link" @click="toggle">
          <router-link to="/about">About</router-link>
        </li>
        <li class="side-link" @click="toggle">
          <router-link to="/sensei">Sensei</router-link>
        </li>
        <li class="side-link" @click="toggle">
          <router-link to="/contact">Contact</router-link>
        </li>
        <li class="side-link" @click="toggle">
          <router-link to="/pricing">Pricing</router-link>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "navabar",
  data() {
    return { toggled: false };
  },
  methods: {
    toggle() {
      this.toggled = !this.toggled;
    },
  },
};
</script>

<style scoped>
.navbar {
  position: relative;
  z-index: 5000;
}
.harmburger {
  background-color: #1d203f;
  border: none;
  cursor: pointer;
  padding: 0;
  position: fixed;
  top: 0;
  left: 0;
}
.line {
  fill: none;
  stroke: black;
  stroke-width: 6;
  transition: stroke-dasharray 200ms cubic-bezier(0.4, 0, 0.2, 1),
    stroke-dashoffset 200ms cubic-bezier(0.4, 0, 0.2, 1);
}
.line1 {
  stroke-dasharray: 60 207;
  stroke-width: 6;
}
.line2 {
  stroke-dasharray: 60 60;
  stroke-width: 6;
}
.line3 {
  stroke-dasharray: 60 207;
  stroke-width: 6;
}
.opened .line1 {
  stroke-dasharray: 90 207;
  stroke-dashoffset: -134;
  stroke-width: 6;
}
.opened .line2 {
  stroke-dasharray: 1 90;
  stroke-dashoffset: -90;
  stroke-width: 6;
}
.opened .line3 {
  stroke-dasharray: 90 207;
  stroke-dashoffset: -134;
  stroke-width: 6;
}
button {
  outline: none;
}

svg {
  height: 60px;
  width: 70px;
}

/* logo image */
.logo {
  position: fixed;
  top: 0px;
  left: 100px;
  z-index: 300;
}
.logo img {
  width: 150px;
  top: 0;
}

/* topnav */

.topnav {
  display: flex;
  flex-direction: column;
  padding: 0px;
  width: calc(100% - 270px);
  position: absolute;
  height: 49px;
  top: 10px;
  margin-left: 200px;
  z-index: 2000;
}
.topnav ul {
  display: flex;
  flex-direction: row;
  padding: 0px;
  position: static;
  max-width: 605px;
  height: 20px;
  left: 0px;
  top: 0px;
  margin: auto;
}

.topnav li {
  flex: none;
  order: 0;
  align-self: center;
  margin: 0px 29px;
  list-style: none;
  position: relative;
  font-family: Montserrat;
  font-style: normal;
}

.navlink::before {
  content: "";
  position: absolute;
  left: 0;
  bottom: -13px;
  background-color: #e6947b;
  width: 100%;
  height: 2px;
  transform: scaleX(0);
  transform-origin: center;
  transition: transform 650ms;
}
.navlink:hover::before {
  transform: scaleX(1);
}

.topnav a {
  color: #ffffff;
  text-decoration: none;
}
/* side-nav */
.side-nav {
  width: 70vw;
  height: 100vh;
  position: absolute;
  z-index: 4000;
  background-color: #14162b;
  display: flex;
  justify-content: center;
  align-items: center;
  transition: 0.3s ease-out;
}
 .side-nav li{
   list-style:none;
   text-decoration: none;
   padding:20px;
    transition:0.2s ease-out;

 }

  .side-nav a{
    text-decoration: none;
       color:#ffff; 
       position:relative;
          z-index:50;

  }

  .side-nav li:hover{
    transform: scale(1.2);
    transition:0.3s ease-out;
  }
  .slide {
  margin-left: -70vw;
  transition: 0.3s ease-out;
}

/* .paatern{
  position:absolute;
  height:100%;
   z-index:10;
right:0;     
opacity: 0.9;

}

.paatern img{
opacity: 0.04;
width:100%;

} */
/* media-query */

@media (max-width: 992px) {
  .topnav {
    display: none;
  }
}
</style>