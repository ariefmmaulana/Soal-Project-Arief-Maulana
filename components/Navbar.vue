<template>
  <section class="section-navbar">
    <div class="container">
      <nav class="navbar navbar-expand-lg">
        <ul class="navbar-nav">
          <li>Beranda</li>
          <li>Blog</li>
          <li>Kenapa?</li>
          <li>Layanan</li>
          <li>Lokasi</li>
          <div class="button" style="margin-left: 630px; margin-top: -10px;">
            <b-button variant="success">Hubungi</b-button>
          </div>
        </ul>
      </nav>
    </div>
  </section>
</template>

<style>
.section-navbar {
  margin: 0px;
  width: 100%;
  box-shadow: none;
  -webkit-box-shadow: none;
  position: fixed;
  z-index: 99;
  transition: background-color 200ms linear;
  background-color: #ffffff;
  height: 50px;
  margin-top: -100px;
  padding-top: 10px;
  padding-bottom: 10px;
}
.section-navbar li {
  color: darkgray;
  font-family: "Poppins-Light";
  margin-right: 16px;
}
</style>