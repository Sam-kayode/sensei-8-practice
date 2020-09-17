<template>
  <div class="landing-page">
    <div class="content">
      <h1 class="display">
        Lorem ipsum
        <br />dolor sit amet
      </h1>
     <a href=""><div class="button">MEET A SENSEI</div></a>
    </div>
    <!-- ellipse shapes -->
    <svg
      class="ellipse-6"
      width="100"
      height="100"
      viewBox="0 0 100 100"
      fill="none"
      xmlns="http://www.w3.org/2000/svg"
    >
      <circle cx="50" cy="50" r="49.5" stroke="url(#paint0_linear)" />
      <defs>
        <linearGradient
          id="paint0_linear"
          x1="0"
          y1="0"
          x2="100.44"
          y2="6.66045"
          gradientUnits="userSpaceOnUse"
        >
          <stop stop-color="#6441A5" />
          <stop offset="0.0001" stop-color="#1D2B64" />
          <stop offset="1" stop-color="#F39D83" />
        </linearGradient>
      </defs>
    </svg>

    <svg
      class="group-4"
      width="378"
      height="470"
      viewBox="0 0 378 470"
      fill="none"
      xmlns="http://www.w3.org/2000/svg"
    >
      <circle opacity="0.5" cx="300" cy="170" r="299.5" stroke="url(#paint0_linear)" />
      <circle opacity="0.5" cx="300" cy="170" r="249.5" stroke="url(#paint1_linear)" />
      <circle opacity="0.5" cx="300" cy="170" r="199.5" stroke="url(#paint2_linear)" />
      <defs>
        <linearGradient
          id="paint0_linear"
          x1="0"
          y1="-130"
          x2="602.638"
          y2="-90.0373"
          gradientUnits="userSpaceOnUse"
        >
          <stop stop-color="#6441A5" />
          <stop offset="0.0001" stop-color="#1D2B64" />
          <stop offset="1" stop-color="#F39D83" />
        </linearGradient>
        <linearGradient
          id="paint1_linear"
          x1="50"
          y1="-80"
          x2="552.198"
          y2="-46.6977"
          gradientUnits="userSpaceOnUse"
        >
          <stop stop-color="#6441A5" />
          <stop offset="0.0001" stop-color="#1D2B64" />
          <stop offset="1" stop-color="#F39D83" />
        </linearGradient>
        <linearGradient
          id="paint2_linear"
          x1="100"
          y1="-30"
          x2="501.759"
          y2="-3.35819"
          gradientUnits="userSpaceOnUse"
        >
          <stop stop-color="#6441A5" />
          <stop offset="0.0001" stop-color="#1D2B64" />
          <stop offset="1" stop-color="#F39D83" />
        </linearGradient>
      </defs>
    </svg>

    <svg class="group-5" viewBox="0 0 69 69" fill="none" xmlns="http://www.w3.org/2000/svg">
      <g opacity="0.5">
        <circle cx="34.5" cy="34.5" r="23" stroke="url(#paint0_linear)" />
        <circle cx="34.5" cy="34.5" r="34" stroke="url(#paint1_linear)" />
      </g>
      <defs>
        <linearGradient
          id="paint0_linear"
          x1="11"
          y1="11"
          x2="58.2066"
          y2="14.1304"
          gradientUnits="userSpaceOnUse"
        >
          <stop stop-color="#6441A5" />
          <stop offset="0.0001" stop-color="#1D2B64" />
          <stop offset="1" stop-color="#F39D83" />
        </linearGradient>
        <linearGradient
          id="paint1_linear"
          x1="0"
          y1="0"
          x2="69.3033"
          y2="4.59571"
          gradientUnits="userSpaceOnUse"
        >
          <stop stop-color="#6441A5" />
          <stop offset="0.0001" stop-color="#1D2B64" />
          <stop offset="1" stop-color="#F39D83" />
        </linearGradient>
      </defs>
    </svg>

    <svg class="group-3" height="110px" widt="110px" viewBox="0 0 100 100" fill="none" xmlns="http://www.w3.org/2000/svg">
      <circle cx="50" cy="50" r="50" fill="#F39D83" fill-opacity="0.2" />
      <circle cx="50" cy="50" r="40" fill="#F39D83" fill-opacity="0.2" />
      <circle cx="50" cy="50" r="25" fill="#F39D83" />
      <path
        d="M61.5698 48.2752C62.8866 49.0481 62.8866 50.9519 61.5698 51.7248L45.3896 61.2222C44.0563 62.0048 42.3772 61.0433 42.3772 59.4974L42.3772 40.5026C42.3772 38.9567 44.0563 37.9952 45.3896 38.7778L61.5698 48.2752Z"
        fill="#1D203F"
      />
    </svg>

    <div class="social">
      <a class="terms" href="">Terms and privacy</a>
      <div class="icons">
        <a href="">
          <i class="fab fa-facebook-f"></i>
        </a>
        <a href="">
          <i class="fab fa-twitter"></i>
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Home",
  components: {},
};
</script>
  
<style scoped>
@import url("https://fonts.googleapis.com/css2?family=IBM+Plex+Serif:wght@400;600&display=swap");

.landing-page {
  height: 100vh;
  padding: 0;
  background-image: url(../assets/landing-background1.jpg);
  background-size: cover;
  margin: 0px;
  position: relative;
  overflow: hidden;
}
.content a{
  text-decoration: none;
  color:#ffffff;
}
.social {
  width: 70px;
  height: inherit;
  border-right: 1px solid #808080;
  box-sizing: border-box;
}
.terms {
  font-family: Montserrat;
  font-style: normal;
  font-weight: lighter;
  font-size: 10px;
  line-height: 20px;
  color: rgba(255, 255, 255, 0.8);
  transform: rotate(-90deg);
  height: 50px;
  position: absolute;
  bottom: 200px;
  text-decoration: none;
}
.icons {
  position: absolute;
bottom:60px;
  text-align: center;

  width: inherit;
}

.icons i {
  color: white;
  display:flex;
  margin: 15px auto;
  width:13px;
}
/* .icons svg{
  color: white;
  display: block;
  margin: 15px auto;
} */

.icons a {
  text-decoration: none;
}

/* ellipse 6 */
.ellipse-6 {
  position: absolute;
  width: 90px;
  left: calc(75vw / 2);
  top: 90px;
}

.group-4 {
  position: absolute;
  width: 350px;
  right: 0px;
  top: 0px;
  z-index: 1;
}
.group-5 {
  position: absolute;
  width: 90px;
  left: 156px;
  top: 220px;
}

.group-3 {
  position:absolute;
  right:20px !important;
  top:62vh !important;
  z-index: 1000;
  opacity: 0.7;
  transition:0.4s ease-out;
    cursor: pointer;
}

.group-3:hover {
   opacity: 1;
  transform: scale(1.1);
  transition: 0.4s ease-out;
}

.content {
  position: absolute;
  text-align: center;
  width:100%;
  margin:auto;
    z-index:500;
  transform: translateY(-50%);
    top: 50%;

}
.content h1 {
  font-family: IBM Plex Serif;
  font-style: normal;
  font-size: 50px;
  font-weight: 600;
  color: #ffffff; 
margin-left:auto;
}


.button  {
  font-family: Montserrat;
  font-style: normal;
  font-weight: lighter;
  font-size: 14px;
  line-height: 20px;
  color: #ffffff;
  background: linear-gradient(
    93.79deg,
    #1d203f 0%,
    #6b4d58 37.45%,
    #f39d83 94.61%
  );
  box-shadow: 0px 5px 20px rgba(0, 0, 0, 0.25);
  border-radius: 30px;
  width: fit-content;
  padding: 10px 40px;
  margin: auto;
  transition:0.3s ease-out;

}
.button:hover{
cursor: pointer;
padding:10px 45px;
  transition:0.3s ease-out;

}

/* media-query */

@media (max-width: 992px) {
  .topnav {
    display: none;
  }

  .content h1{
    font-size: 30px;
  }

  .group-3{
    top:430px;
    right:10px;
  }
}
</style>


