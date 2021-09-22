<template>
<nav>
  <div class="container">
      <ul class="navbar-nav ml-auto">
        <li class="nav-item ">
          <a class="nav-link" href="#">Home</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">About</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Portfolio</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Services</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Contact</a>
        </li>
      </ul>
    </div>
</nav>


</template>
<script>

</script>
<style scoped>
    li, a{
        list-style: none;
        text-decoration: none;
        color: black;
        padding: 5px
    }
    ul {
    display: flex;
    align-content: center;
    justify-content: space-around;
    }
    nav{
        padding: 10px;
        background-color: white;
        position: fixed;
        width: 100%;
        top : 0;
        
    }

a {
  position: relative;
}
a::after {
  content: '';
  transform-origin: 0 0; 
  transform: scaleX(0);
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  height: .1em; 
  background: black;
  z-index: -1;
  opacity: 0.8;
  transition: transform .3s;
}
a:hover::after {
  transform: scaleX(1);
}
</style>
