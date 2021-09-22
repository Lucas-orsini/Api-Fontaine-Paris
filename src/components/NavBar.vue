<template>
<nav>
  <div class="container">
      <ul class="navbar-nav ml-auto">
        <li class="nav-item ">
          <a class="nav-link" href="#">API</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Water point</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">GitHub</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Contact Us</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Support Us </a>
        </li>
      </ul>
    </div>
</nav>


</template>
<script>

</script>
<style scoped>

  .navbar-nav li, .navbar-nav a{
        list-style: none;
        text-decoration: none;
        color: white;
        padding: 5px
    }
    .navbar-nav {
    display: flex;
    align-content: center;
    justify-content: space-around;
    }
    nav{
        padding: 10px;
        background-color: #26272b;
        position: fixed;
        width: 100%;
        top : 0;
        font-family: Avenir, Helvetica, Arial, sans-serif;
        
    }

.navbar-nav a {
  position: relative;
}
.navbar-nav a::after {
  content: '';
  transform-origin: 0 0; 
  transform: scaleX(0);
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  height: .1em; 
  background: white;
  z-index: -1;
  opacity: 0.8;
  transition: transform .3s;
}
.navbar-nav a:hover::after {
  transform: scaleX(1);
}
</style>
