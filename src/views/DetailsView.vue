<script>
  export default {
    props: ["id"],
    data() {
      return {
        data_images: [
          {
            id: 1,
            logo_name: "ARSENAL",
            logo_file: "arsenal.jpg",
            palyed: 8,
            scores: 4,
            lose: 1,
            rating: 5,
          },
          {
            id: 2,
            logo_name: "LIVERPOOL",
            logo_file: "bola2.png",
            palyed: 6,
            scores: 2,
            lose: 2,
            rating: 3,
          },
          {
            id: 3,
            logo_name: "AC MILAN",
            logo_file: "milan.jpg",
            palyed: 6,
            scores: 2,
            lose: 2,
            rating: 3,
          },
          {
            id: 4,
            logo_name: "INTER MILAN",
            logo_file: "inter.jpg",
            palyed: 6,
            scores: 2,
            lose: 2,
            rating: 3,
          },
          {
            id: 5,
            logo_name: "MANCESTER UNITED",
            logo_file: "MUI.png",
            palyed: 6,
            scores: 2,
            lose: 2,
            rating: 3,
          },
          {
            id: 6,
            logo_name: "VALENCIA",
            logo_file: "valencia.jpg",
            palyed: 6,
            scores: 2,
            lose: 2,
            rating: 3,
          },
          {
            id: 7,
            logo_name: "PARIS",
            logo_file: "paris.jpg",
            palyed: 6,
            scores: 2,
            lose: 2,
            rating: 3,
          },
          {
            id: 8,
            logo_name: "REAL MADRID",
            logo_file: "bola8.png",
            palyed: 6,
            scores: 2,
            lose: 2,
            rating: 3,
          },
          {
            id: 9,
            logo_name: "BORUSSIA DORTMUND",
            logo_file: "OIP.jpg",
            palyed: 6,
            scores: 2,
            lose: 2,
            rating: 3,
          },
          {
            id: 10,
            logo_name: "BAYER MUCHEN",
            logo_file: "bayer.jpg",
            palyed: 6,
            scores: 2,
            lose: 2,
            rating: 3,
          },
        ],
      };
    },
  };
</script>
<template>
  <div class="container">
    <div v-for="data_images in data_images" class="col">
      <div v-if="data_images.id == id">
        <div class="mt-2 mx-auto" style="width: 18rem">
          <img
            :src="'/src/assets/logo_bola/' + data_images.logo_file"
            class="rounded mx-auto d-block"
            alt="404"
          />
          <div class="card-body">
            <h5 class="text-center mt-2">{{ data_images.logo_name }}</h5>
          </div>
        </div>

        <div class="row row-cols-1 row-cols-md-4 g-4 mt-3">
          <div class="col">
            <div class="card shadow-sm">
              <div class="card-body">
                <h5 class="card-title">
                  Played <br />
                  {{ data_images.palyed }}
                </h5>
              </div>
            </div>
          </div>
          <div class="col">
            <div class="card shadow-sm">
              <div class="card-body">
                <h5 class="card-title">
                  Scores <br />
                  {{ data_images.scores }}
                </h5>
              </div>
            </div>
          </div>
          <div class="col">
            <div class="card shadow-sm">
              <div class="card-body">
                <h5 class="card-title">
                  Lose <br />
                  {{ data_images.lose }}
                </h5>
              </div>
            </div>
          </div>
          <div class="col">
            <div class="card shadow-sm">
              <div class="card-body">
                <h5 class="card-title">
                  Rating <br />
                  {{ data_images.rating }}
                </h5>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<style>
  img {
    width: 160px;
    height: 160px;
  }
  h5 {
    text-align: center;
  }
</style>
