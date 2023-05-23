<script>
  export default {
    props: ["id"],
    data() {
      return {
        data_images: [
          {
            id: 1,
            logo_name: "FOTBALL FC",
            logo_file: "bola1.png",
            palyed: 8,
            scores: 4,
            lose: 0,
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
            logo_name: "HANOVER",
            logo_file: "bola3.jpeg",
            palyed: 6,
            scores: 2,
            lose: 2,
            rating: 3,
          },
          {
            id: 4,
            logo_name: "BROCELLE",
            logo_file: "bola4.jpeg",
            palyed: 6,
            scores: 2,
            lose: 2,
            rating: 3,
          },
          {
            id: 5,
            logo_name: "CLUB BRUGEN KV",
            logo_file: "bola5.png",
            palyed: 6,
            scores: 2,
            lose: 2,
            rating: 3,
          },
          {
            id: 6,
            logo_name: "CHAMPION TEAM",
            logo_file: "bola6.jpeg",
            palyed: 6,
            scores: 2,
            lose: 2,
            rating: 3,
          },
          {
            id: 7,
            logo_name: "SOCCER CLUB",
            logo_file: "bola7.png",
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
            logo_name: "ALMERIA",
            logo_file: "bola9.png",
            palyed: 6,
            scores: 2,
            lose: 2,
            rating: 3,
          },
          {
            id: 10,
            logo_name: "FC BAZENHEID",
            logo_file: "bola10.png",
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
