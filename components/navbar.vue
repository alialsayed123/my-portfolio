<template>
  <div class="navbar">
    <nav>
      <router-link class="href" to="/" exact active-class="active-link">Home</router-link>
      <router-link class="href" to="/about" exact active-class="active-link"
        >About</router-link
      >
      <router-link class="href" to="/skills" exact active-class="active-link"
        >Skills</router-link
      >
      <router-link class="href" to="/portfolio" exact active-class="active-link"
        >Portfolio</router-link
      >
      <router-link class="href" to="/contactMy" exact active-class="active-link"
        >Contact</router-link
      >
      <div class="animation start-home"></div>
    </nav>
  </div>
</template>

<style scoped>
/* @import url('https://fonts.googleapis.com/css?family=Open+Sans&display=swap'); */
body {
  font-family: "Open Sans", sans-serif;
  margin: 0;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh; /* Center vertically in the viewport */
  background-color: #f2f2f2; /* Set a background color for the entire page */
}


.navbar {
  display: flex;
  justify-content: center;
  align-items: center;
  position: fixed;
  z-index: 99;
  width: 100%;
  margin: 15px 0;
 /* Apply a blur effect */
}

nav {
  position: relative;
  width: 50%;
  height: 80px;
  background-color: rgb(125 130 133 / 17%);

  border-radius: 12px;
  font-size: 0;
  box-shadow: 0 2px 3px 0 rgba(0, 0, 0, 0.1);
  z-index: 99;
  display: flex;
  justify-content: center;
  border: 1px solid #e5e7eb;
  opacity: 1;
  box-sizing: border-box;
  backdrop-filter: blur(10px);
}

nav a {
  font-size: 15px;
  text-transform: uppercase;
  color: white;
  text-decoration: none;
  line-height: 80px;
  position: relative;
  z-index: 1;
  display: inline-block;
  cursor: pointer;
  text-align: center;
  margin: 0 2%; /* Add some horizontal margin between navigation items */
  padding: 0 2%;
  flex-grow: 1; /* Make navigation items evenly spaced */
  transition: all 0.5s ease 0s; /* Apply transition to all properties */
}

.active-link {
  color: #fff;
  position: relative;

  
  /* Change the text color for active link */
}

.active-link::after {
  content: "";
  position: absolute;
  height: 5px;
  width: 100%;
  top: 0;
  left: 0;
  z-index: -1;
  background-color: #32a39b;
  border-radius: 8px;
  transition: all 0.5s ease 0s; /* Apply transition to all properties */
}

.href{
	position: relative;
}
.href::before {
  content: "";
  position: absolute;
  height: 5px;
  width: 0;
  top: 0;
  left: 0;
  z-index: -1;
  
  background-color: #32a39b;
  backdrop-filter: blur(10px);
  border-radius: 8px;
  transition: width 1s ease 0s; /* Apply transition to all properties */
}

.href:hover::before {
	width: 100%; 
	

}







@media screen and (max-width: 700px) {
  /* nav {
    position: relative;
    width: 95%;
    height: 50px;
    background: #13151600;
    border-radius: 8px;
    font-size: 0;
    box-shadow: 0 2px 3px 0 rgba(0, 0, 0, 0.1);
    z-index: 99;
    display: flex;
    justify-content: center;
  } */
  nav {
  position: relative;
  width: 95%;
  height: 60px;
  background-color: rgb(125 130 133 / 17%);

  border-radius: 12px;
  font-size: 0;
  box-shadow: 0 2px 3px 0 rgba(0, 0, 0, 0.1);
  z-index: 99;
  display: flex;
  justify-content: center;
  border: 1px solid #e5e7eb;
  opacity: 1;
  box-sizing: border-box;
  backdrop-filter: blur(10px);
}

  nav a {
    font-size: 13px;
    text-transform: uppercase;
    color: white;
    text-decoration: none;
    line-height: 60px;
    position: relative;
    z-index: 1;
    display: inline-block;
    text-align: center;
    margin: 0; /* Add some horizontal margin between navigation items */
    padding: 0;
    width: 100%;
  }
}

/* Add a media query for smaller screens */
@media screen and (max-width: 500px) {
  nav {
  position: relative;
  width: 95%;
  height: 60px;
  background-color: rgb(125 130 133 / 17%);

  border-radius: 12px;
  font-size: 0;
  box-shadow: 0 2px 3px 0 rgba(0, 0, 0, 0.1);
  z-index: 99;
  display: flex;
  justify-content: center;
  border: 1px solid #e5e7eb;
  opacity: 1;
  box-sizing: border-box;
  backdrop-filter: blur(10px);
}
  /* nav {
    position: relative;
  
    height: 50px;
    background: #34495e;
    border-radius: 8px;
    font-size: 0;
    box-shadow: 0 2px 3px 0 rgba(0, 0, 0, 0.1);
    z-index: 99;
    display: flex;
    justify-content: center;
  } */
  .navbar {
    display: flex;
    justify-content: center;
    align-items: center;
    position: fixed;
    z-index: 99;
    width: 100%;
    margin: 15px 0;
    bottom: 0;
    width: 100%;
  }
  nav a {
    font-size: 13px;
    text-transform: uppercase;
    color: white;
    text-decoration: none;
    line-height: 60px;
    position: relative;
    z-index: 1;
    display: inline-block;
    text-align: center;
    margin: 0; /* Add some horizontal margin between navigation items */
    padding: 0;
    width: 100%;
  }
}
</style>
