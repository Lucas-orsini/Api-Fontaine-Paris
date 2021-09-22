<template>
  <!-- Site footer -->
  <footer class="site-footer">
    <div class="container">
      <div class="row">
        <div class="about">
          <h6>About</h6>
          <p class="text-justify">The Walks and refresh platform is a customizable and extensible open source information gathering platform that brings together all the different drinking fountains in Paris. You
            can easily add features to extend the platform and make part of the project.</p>
        </div>

        <div>
          <h6>Categories</h6>
          <ul class="footer-links">
            <li><a href="#">Fontaine_bois</a></li>
            <li><a href="#">Fontaine_arceau</a></li>
            <li><a href="#">Fontaine_totem</a></li>
          </ul>
        </div>

        <div>
          <h6>Quick Links</h6>
          <ul class="footer-links">
            <li><a href="#">Contact Us</a></li>
            <li><a href="https://opendata.paris.fr/api/v1/console/datasets/1.0/search/">API</a></li>
            <li><a href="https://github.com/Lucas-orsini/Api-Fontaine-Paris">GitHub</a></li>
          </ul>
        </div>
      </div>
      <hr>
    </div>
    <div class="container">
      <div class="row">
        <div>
          <p class="copyright-text">Copyright &copy; 2021 All Rights Reserved by
            <a href="#">API-Fontaine-Paris</a>.
          </p>
        </div>


      </div>
    </div>
  </footer>
</template>
<style>

body{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
.site-footer {
  background-color: #26272b;
  padding: 45px 0 20px;
  font-size: 15px;
  line-height: 24px;
  color: #737373;
}

.site-footer h6 {
  color: #fff;
  font-size: 16px;
  text-transform: uppercase;
  margin-top: 5px;
  letter-spacing: 2px;
}

.site-footer a {
  color: #737373;
  text-decoration: none;

}

.site-footer a:hover {
  color: white;
  text-decoration: none;
}
.footer-links a:hover {
  color: white !important;
  text-decoration: none;
}

.footer-links {
  padding-left: 0;
  list-style: none;
}

.footer-links li {
  display: block;
}

.footer-links a {
  color: #737373;
  list-style: none;
  text-decoration: none;
}

.footer-links a:active, .footer-links a:focus, .footer-links a:hover {
  color: #3366cc;
  text-decoration: none;
}

.footer-links.inline li {
  display: inline-block
}

.site-footer .social-icons {
  text-align: right
}

.site-footer .social-icons a {
  width: 40px;
  height: 40px;
  line-height: 40px;
  margin-left: 6px;
  margin-right: 0;
  border-radius: 100%;
  background-color: #33353d
}

.copyright-text {
  margin: 0
}
.about{
  display: table;
}
.row{
  justify-content: center;
  display: flex;
}
.text-justify{
  max-width: 90vh;
}
.row div{
  margin-right: 35px;
}

</style>
