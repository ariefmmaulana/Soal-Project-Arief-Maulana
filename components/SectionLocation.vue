<template>
  <section class="section-location">
    <div class="location" v-for="item in dataLocation" :key="item.id">
      <div class="container container-top">
        <h3 v-html="item.title"></h3>
        <div class="row">
          <div class="col-6">
            <p v-html="item.desc"></p>
          </div>
          <div class="col-6">
            <div style="text-align: right">
              <b-dropdown
                id="dropdown-1"
                text="Pick based on area"
                class="m-md-2"
              >
                <b-dropdown-item>First Action</b-dropdown-item>
                <b-dropdown-item>Second Action</b-dropdown-item>
                <b-dropdown-item>Third Action</b-dropdown-item>
              </b-dropdown>
            </div>
          </div>
        </div>
        <div class="location">
          <p v-html="item.location"></p>
        </div>
        <div class="row row-location">
          <div class="col-2">
            <div class="grid-artikel" v-for="(value) in item.value" :key="value.id">
            <div class="list-artikel">
              <div class="container box-venue">
                <div class="content-value">
                  <div class="image-venue">
                    <img
                    :src="`https://api.ecolify.com/image/site/large/${value.img}`"
                  />
                  </div>
                  <h6 v-html="value.venue"></h6>
                  <p v-html="value.location"></p>
                </div>
              </div>
            </div>
          </div>
          </div>
          <div class="col-10">
            <iframe
              :src="`https://www.google.com/maps/${item.map}`"
              alt=""
            ></iframe>
          </div>
        </div>
        <h6 v-html="item.question"></h6>
        <div class="center d-flex justify-content-center">
          <b-button variant="success" v-html="item.button"></b-button>
        </div>
      </div>
      <div class="container-fluid container-bottom">
        <div class="row">
          <div class="col-6">
            <h4 v-html="item.titlebottom"></h4>
            <p v-html="item.descbottom">
            </p>
          </div>
          <div class="col-6">
            <div style="text-align: right; margin-right: 100px">
              <b-button variant="primary" v-html="item.buttonbottom"></b-button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import locationData from "~/static/location.json";

export default {
  data() {
    return {
      dataLocation: locationData,
    };
  },
};
</script>

<style>
.section-location .container-top {
  margin-top: 100px;
}
.section-location .container-top .btn-group {
  width: 340px;
  height: 30px;
}
.section-location .container-top .btn-group .show{
  width: 340px;
}
.section-location .container-bottom .btn-primary {
  width: 153px;
}
.section-location .container-top .btn-secondary {
  padding-top: 2px;
  text-align: left;
  background-color: #E5E5E5;
  color: #000000;
}
.section-location iframe {
  width: 910px;
  height: 400px;
}
.section-location h3 {
  font-size: 48px;
  font-family: "Poppins-Medium";
  margin-bottom: 25px;
}
.section-location .container-top p {
  font-size: 24px;
  font-family: "Poppins-Light";
}
.section-location h6 {
  text-align: center;
  font-family: "Poppins-Medium";
  font-size: 24px;
  margin-top: 33px;
  margin-bottom: 22px;
}
.section-location .container-bottom {
  background-color: #f5f5f5;
  margin-top: 40px;
  padding: 70px 200px 140px 200px;
}
.section-location h4 {
  font-size: 24px;
  font-family: "Poppins-Bold";
}
.section-location .container-bottom p {
  font-size: 14px;
  font-family: "Poppins-Light";
}
.section-location .row-location {
  margin-top: 20px;
}
.section-location .location {
  margin-top: 60px;
}
.section-location .container-top .location p {
  font-family: "Poppins-Medium";
  font-size: 18px;
}
.section-location .dropdown-toggle::after {
  margin-left: 9.255em;
}
.section-location span {
  color: #2dc48d;
}
.section-location .grid-artikel {
  display: flex;
  flex-wrap: wrap;
  width: 100%;
  height: auto;
  gap: 30px;
}
.section-location .container-top .grid-artikel h6 {
  font-size: 12px;
  margin-bottom: 5px;
  margin-top: 5px;
}
.section-location .container-top .grid-artikel p {
  font-size: 12px;
  text-align: center;
}
.section-location .container-top .grid-artikel img {
  width: 146px;
  height: 73px;
}
.section-location .image-venue {
  margin-left: -15px;
}
.section-location .box-venue {
  box-shadow: 0 5px 5px 0 rgba(165, 173, 187, 0.05),
    0 -5px 5px 0 rgba(165, 173, 187, 0.05),
    -5px 0 5px 0 rgba(165, 173, 187, 0.05),
    5px 0 5px 0 rgba(165, 173, 187, 0.05);
  width: 146px;
  height: 140px;
}
</style>
