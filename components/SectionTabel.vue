<template>
  <div class="tes-project">
    <div class="container" style="margin-top: 50px">
      <table class="table table-bordered">
        <thead>
          <tr>
            <th scope="col"></th>
            <th scope="col">kd_artis</th>
            <th scope="col">nm_artis</th>
            <th scope="col">jk</th>
            <th scope="col">bayaran</th>
            <th scope="col">award</th>
            <th scope="col">negara</th>
          </tr>
        </thead>
        <tbody>
          <tr v-for="item in dataArtis" :key="item.dataArtis">
            <th scope="row">{{ item.id }}</th>
            <td>{{ item.kd_artis }}</td>
            <td>{{ item.nm_artis }}</td>
            <td>{{ item.jk }}</td>
            <td>{{ item.bayaran }}</td>
            <td>{{ item.award }}</td>
            <td>{{ item.negara }}</td>
          </tr>
        </tbody>
      </table>
    </div>
    <div class="container" style="margin-top: 50px">
      <table class="table table-bordered">
        <thead>
          <tr>
            <th scope="col"></th>
            <th scope="col">kd_film</th>
            <th scope="col">nm_film</th>
            <th scope="col">genre</th>
            <th scope="col">artis</th>
            <th scope="col">produser</th>
            <th scope="col">pendapatan</th>
            <th scope="col">nominasi</th>
          </tr>
        </thead>
        <tbody>
          <tr v-for="item in dataFilm" :key="item.dataFilm">
            <th scope="row">{{ item.id }}</th>
            <td>{{ item.kd_film }}</td>
            <td>{{ item.nm_film }}</td>
            <td>{{ item.genre }}</td>
            <td>{{ item.artis }}</td>
            <td>{{ item.produser }}</td>
            <td>{{ item.pendapatan }}</td>
            <td>{{ item.nominasi }}</td>
          </tr>
        </tbody>
      </table>
    </div>
    <div class="container" style="margin-top: 50px">
      <table class="table table-bordered">
        <thead>
          <tr>
            <th scope="col"></th>
            <th scope="col">kd_genre</th>
            <th scope="col">nm_genre</th>
          </tr>
        </thead>
        <tbody>
          <tr v-for="item in dataGenre" :key="item.dataGenre">
            <th scope="row">{{ item.id }}</th>
            <td>{{ item.kd_genre }}</td>
            <td>{{ item.nm_genre }}</td>
          </tr>
        </tbody>
      </table>
    </div>
    <div class="container" style="margin-top: 50px">
      <table class="table table-bordered">
        <thead>
          <tr>
            <th scope="col"></th>
            <th scope="col">kd_negara</th>
            <th scope="col">nm_negara</th>
          </tr>
        </thead>
        <tbody>
          <tr v-for="item in dataRegion" :key="item.dataRegion">
            <th scope="row">{{ item.id }}</th>
            <td>{{ item.kd_negara }}</td>
            <td>{{ item.nm_negara }}</td>
          </tr>
        </tbody>
      </table>
    </div>
    <div class="container" style="margin-top: 50px">
      <table class="table table-bordered">
        <thead>
          <tr>
            <th scope="col"></th>
            <th scope="col">kd_negara</th>
            <th scope="col">nm_negara</th>
          </tr>
        </thead>
        <tbody>
          <tr v-for="item in dataRegion" :key="item.dataRegion">
            <th scope="row">{{ item.id }}</th>
            <td>{{ item.kd_negara }}</td>
            <td>{{ item.nm_negara }}</td>
          </tr>
        </tbody>
      </table>
    </div>
    <div class="container" style="margin-top: 50px">
      <table class="table table-bordered">
        <thead>
          <tr>
            <th scope="col"></th>
            <th scope="col">kd_produser</th>
            <th scope="col">nm_produser</th>
            <th scope="col">international</th>
          </tr>
        </thead>
        <tbody>
          <tr v-for="item in dataProduser" :key="item.dataProduser">
            <th scope="row">{{ item.id }}</th>
            <td>{{ item.kd_produser }}</td>
            <td>{{ item.nm_produser }}</td>
            <td>{{ item.international }}</td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
</template>

<script>
import genreData from "~/static/genre.json";
import artisData from "~/static/artis.json";
import filmData from "~/static/film.json";
import regionData from "~/static/region.json";
import produserData from "~/static/produser.json";

export default {
  data() {
    return {
      dataGenre: genreData,
      dataArtis: artisData,
      dataFilm: filmData,
      dataRegion: regionData,
      dataProduser: produserData,
    };
  },
};
</script>
