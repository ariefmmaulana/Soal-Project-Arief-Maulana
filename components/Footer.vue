<template>
  <div class="section-footer">
    <div class="container-footer-wave">
      <div class="wave">
        <img :src="`https://ecolify.org/_nuxt/img/gelombang-footer2.b6e2f25.svg`" />
      </div>
    </div>
    <div class="container-footer">
      <div class="row">
        <div class="col-sm-12 col-md-3 col-lg-3">
          <div class="logo">
            <img src="../assets/img/ecolify-logo.png" alt="" />
          </div>
          <h5>lindungihutan</h5>
          <p class="bold">
            <span>Ecofly</span> adalah platform yang memudahkan organisasi instansi dan
            perusahaan untuk menjalankan projek sosial penanaman pohon secara
            transparan dan berkelanjutan
          </p>
        </div>
        <div class="col-sm-12 col-md-2 col-lg-2">
          <div class="row">
            <h4>Peta Situs</h4>
          </div>
          <div class="row">
            <a>Beranda</a>
          </div>
          <div class="row">
            <a>Blog</a>
          </div>
          <div class="row">
            <a>Kenapa?</a>
          </div>
          <div class="row">
            <a>Lokasi</a>
          </div>
          <div class="row">
            <a>Layanan</a>
          </div>
        </div>
        <div class="col-sm-12 col-md-2 col-lg-2">
          <div class="row">
            <h4>Resources</h4>
          </div>
          <div class="row">
            <a>FAQ</a>
          </div>
          <div class="row">
            <a>Kebijakan Privasi</a>
          </div>
        </div>
        <div class="col-sm-12 col-md-3 col-lg-3 row-hubungikami">
          <div class="row">
            <h4>Hubungi Kami</h4>
          </div>
          <div class="row">
            <p>
              email:
              <br />
              <span>kartika@lindungihutan.com</span>
            </p>
            <p>
              wa / phone:
              <br />
              <span>+62 813 2918 1389</span>
            </p>
            <p>
              location:
              <br />
              <span>Jalan Lempongsari 1 No. 405,<br />Semarang, Indonesia</span>
            </p>
            <p>
              legal info:
              <br />
              <span
                >Keputusan MENKUMHAM NOMOR AHU-<br />0003033.AHA.01.04.</span
              >
            </p>
          </div>
        </div>
        <div class="col-sm-12 col-md-2 col-lg-2">
          <div class="row">
            <h4>Ikuti Kami</h4>
          </div>
        </div>
      </div>
      <p style="margin-top: 20px">
        LindungiHutan c 2020 - made with conscience "for a future worth living"
      </p>
    </div>
  </div>
</template>

<style>
.section-footer .container-footer {
  padding: 20px 100px;
  background-color: #47baa6;
}
.section-footer h4 {
  font-size: 18px;
  font-family: "Poppins-Bold";
  color: #ffffff;
}
.section-footer p {
  margin-bottom: 0px;
  font-family: "Poppins-Light";
  color: #ffffff;
  font-size: 14px;
  width: 85%;
}
.section-footer a {
  font-size: 16px;
  color: #ffffff !important;
}
.section-footer h6 {
  font-size: 12px;
  color: #ffffff;
}
.section-footer .logo img {
  width: 140px;
  height: 50px;
}
.section-footer h5 {
  font-size: 24px;
  color: #ffffff;
}
.section-footer .row-hubungikami p {
  font-family: "Poppins-Medium";
  font-size: 14px;
}
.section-footer .row-hubungikami span {
  font-family: "Poppins-Light";
  font-size: 14px;
}
.section-footer .wave img {
  background-size: cover;
  height: 170px;
  margin-top: -130px;
}
.section-footer .bold span {
  font-family: "Poppins-Bold";
}
</style>