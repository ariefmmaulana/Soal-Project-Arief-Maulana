<template>
  <section class="section-blog">
    <div class="container container-top">
      <img class="center" src="../assets/img/ecolify-blog.png" alt="" />
      <div class="row row-button-category">
        <div class="col-2">Eco-Acts</div>
        <div class="col-2">Eco-News</div>
        <div class="col-2">Eco-Project</div>
        <div class="col-2">Eco-Edu</div>
        <div class="col-2">Eco-Tips</div>
        <div class="col-2">Eco-Feature</div>
      </div>
      <h6 class="title-top">Artikel Pilihan</h6>
      <div class="grid-artikel">
        <div class="row">
          <div class="col-8">
            <div v-for="item in dataBlog1" :key="item.id" class="list-blog">
              <template>
                <div class="list-artikel">
                  <div class="container box-blog-content-1">
                    <div class="content-blog">
                      <img
                        :src="`https://api.ecolify.com/image/blog/small/${item.img}`"
                      />
                      <div class="row row-category">
                        <div class="col-2">
                          <img
                            src="data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNCIgaGVpZ2h0PSIxNSIgdmlld0JveD0iMCAwIDQgMTUiIGZpbGw9Im5vbmUiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+CjxyZWN0IHdpZHRoPSI0IiBoZWlnaHQ9IjE1IiBmaWxsPSIjNjdDMERFIi8+Cjwvc3ZnPgo="
                            alt=""
                          />
                        </div>
                        <div class="col-10">
                          <span v-html="item.category"></span>
                        </div>
                      </div>
                      <div class="title">
                        <h5 v-html="item.title"></h5>
                      </div>
                      <p class="desc" v-html="item.desc"></p>
                      <p v-html="item.posted"></p>
                    </div>
                  </div>
                </div>
              </template>
            </div>
          </div>
          <div class="col-4">
            <div v-for="item in dataBlog2" :key="item.id" class="list-blog">
              <template>
                <div class="list-artikel">
                  <div class="container box-blog-content-2">
                    <div class="content-blog">
                      <img
                        :src="`https://api.ecolify.com/image/blog/small/${item.img}`"
                      />
                      <div class="row row-category">
                        <div class="col-2">
                          <img
                            src="data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNCIgaGVpZ2h0PSIxNSIgdmlld0JveD0iMCAwIDQgMTUiIGZpbGw9Im5vbmUiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+CjxyZWN0IHdpZHRoPSI0IiBoZWlnaHQ9IjE1IiBmaWxsPSIjNjdDMERFIi8+Cjwvc3ZnPgo="
                            alt=""
                          />
                        </div>
                        <div class="col-10">
                          <span v-html="item.category"></span>
                        </div>
                      </div>
                      <div class="title">
                        <h5 v-html="item.title"></h5>
                      </div>
                      <p class="desc" v-html="item.desc"></p>
                      <p v-html="item.posted"></p>
                    </div>
                  </div>
                </div>
              </template>
            </div>
          </div>
        </div>
      </div>
      <div class="grid-artikel">
        <div v-for="item in dataBlog" :key="item.id" class="list-blog">
          <template>
            <div class="list-artikel">
              <div class="container box-blog">
                <!-- <img
                class="w-100"
                v-if="item.img"
                :src="require(`~/assets/${item.img}`)"
                alt=""
              /> -->
                <div class="content-blog">
                  <img
                    :src="`https://api.ecolify.com/image/blog/small/${item.img}`"
                  />
                  <div class="row row-category">
                    <div class="col-2">
                      <img
                        src="data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNCIgaGVpZ2h0PSIxNSIgdmlld0JveD0iMCAwIDQgMTUiIGZpbGw9Im5vbmUiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+CjxyZWN0IHdpZHRoPSI0IiBoZWlnaHQ9IjE1IiBmaWxsPSIjNjdDMERFIi8+Cjwvc3ZnPgo="
                        alt=""
                      />
                    </div>
                    <div class="col-10">
                      <span v-html="item.category"></span>
                    </div>
                  </div>
                  <div class="title">
                    <h5 v-html="item.title"></h5>
                  </div>
                  <p class="desc" v-html="item.desc"></p>
                  <p v-html="item.posted"></p>
                </div>
              </div>
            </div>
          </template>
        </div>
      </div>
      <div class="center-button">
        <b-button variant="success">Lanjut Baca</b-button>
      </div>
    </div>
  </section>
</template>

<script>
import blogData from "~/static/blog.json";

export default {
  data() {
    return {
      dataBlog: blogData,
      dataBlog2: [
        {
          id: 2,
          img: "CSR%20Sebagai%20Strategi%20Penghijauan-GkJlH-1641452313yHmED.jpg",
          category: "Eco-Act",
          title: "Environmental CSR as a Nature Conservation Strategy",
          desc: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
          posted: "6 Jan 2022 / Miftachur Robani",
        },
      ],
      dataBlog1: [
        {
          id: 1,
          img: "CSR%20Lingkungan%20Hidup%20untuk%20Hijaukan%20Bumi-nCCFD-1642398939kWjBf.jpg",
          category: "Eco-Act",
          title: "Environmental CSR Greening the Mother Earth",
          desc: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
          posted: "17 Jan 2022 / Miftachur Robani",
        },
      ],
    };
  },
};
</script>


<style>
.section-blog .container-top {
  margin-top: 100px;
  margin-bottom: 180px;
}
.section-blog .center {
  display: block;
  margin-left: auto;
  margin-right: auto;
}
.section-blog .center-button {
    text-align: center; 
    margin-top: 40px
}
.section-blog h6 {
  font-size: 48px;
}
.section-blog .grid-artikel {
  display: flex;
  flex-wrap: wrap;
  width: 100%;
  height: auto;
  gap: 15px;
}
.section-blog .box-blog {
  width: 358px;
  height: 460px;
}
.section-blog .box-blog-content-2 {
  width: 300px;
  height: 520px;
  margin-left: 45px;
}
.section-blog .box-blog-content-1 {
  width: 690px;
  height: 540px;
}
.section-blog .box-blog-content-2 img {
  width: 300px;
  height: 300px;
  background-size: cover;
}
.section-blog .box-blog-content-1 img {
  width: 670px;
  height: 300px;
  background-size: cover;
}
.section-blog .box-blog-content-1 span {
  margin-left: -100px;
}
.section-blog .box-blog-content-2 span {
  margin-left: -35px;
}
.section-blog .box-blog-content-2 .desc {
  margin-bottom: 15px;
}
.section-blog .box-blog-content-1 .desc {
  margin-bottom: 55px;
}
.section-blog h5 {
  font-size: 14px;
  color: #212322;
  font-family: "Poppins-Bold";
}
.section-blog p {
  font-size: 14px;
  font-family: "Poppins-Light";
  color: #96a59d;
}
.section-blog .box-blog img {
  width: 328px;
  height: 246px;
}
.section-blog .desc {
  margin-bottom: 30px;
}
.section-blog .title {
  height: 40px;
}
.section-blog .title-top {
  padding: 20px 20px 40px 20px;
}
.section-blog span {
  font-size: 16px;
  color: #67c0de;
  font-family: "Poppins-Medium";
  margin-left: -45px;
}
.section-blog .row-category img {
  width: 5px;
  height: 20px;
}
.section-blog .row-category {
  margin-bottom: 10px;
  margin-top: 10px;
}
.section-blog .row-button-category {
  padding-left: 40px;
  margin-top: 40px;
  margin-bottom: 90px;
}
</style>