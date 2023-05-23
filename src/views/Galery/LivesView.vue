<script>
  export default {
    data() {
      return {
        logo_bendera: [
          {
            rating: "rating1.png",
            bendera: "bendera.png",
            negara: "indonesia",
          },
        ],
        data_live_liga_one: [
          {
            club_logo: "bola1.png",
            club_name: "FOTBALL FC",
            scores: 3,
            session_liga: 1,
          },
          {
            club_logo: "bola2.png",
            club_name: "LIVERPOOL",
            scores: 1,
            session_liga: 1,
          },
        ],
        data_live_liga_two: [
          {
            club_logo: "bola3.jpeg",
            club_name: "HANOVER",
            scores: 4,
            session_liga: 1,
          },
          {
            club_logo: "bola4.jpeg",
            club_name: "BROCELLE",
            scores: 2,
            session_liga: 1,
          },
        ],
        data_live_liga_three: [
          {
            club_logo: "bola5.png",
            club_name: "CLUB BRUGEN KV",
            scores: 1,
            session_liga: 1,
          },
          {
            club_logo: "bola6.jpeg",
            club_name: "CHAMPION TEAM",
            scores: 1,
            session_liga: 1,
          },
        ],
        data_live_liga_four: [
          {
            club_logo: "bola7.png",
            club_name: "SOCCER CLUB",
            scores: 0,
            session_liga: 1,
          },
          {
            club_logo: "bola8.png",
            club_name: "REAL MADRID",
            scores: 3,
            session_liga: 1,
          },
        ],
      };
    },
  };
</script>
<template>
  <div class="container">
    <h2 class="text-center">In live</h2>

    <!-- dropdown pertama -->
    <div
      class="row btn-lg text-bg-warning p-2"
      data-bs-toggle="dropdown"
      aria-expanded="false"
    >
      <div v-for="logo_bendera in logo_bendera">
        <div id="bendera" class="col-2 d-flex justify-content-between">
          <div>
            <img :src="'/src/assets/bendera/' + logo_bendera.rating" />
          </div>
          <div>
            <img :src="'/src/assets/bendera/' + logo_bendera.bendera" />
          </div>
          <div>
            <span>{{ logo_bendera.negara }}</span>
          </div>
        </div>
      </div>
    </div>
    <ul class="dropdown-menu container">
      <div class="container d-flex">
        <div class="col-2 mt-2">
          <div v-for="logo_bendera in logo_bendera">
            <div id="bendera" class="col-4 d-flex justify-content-between">
              <div class="col-2 ml-2">
                <img :src="'/src/assets/bendera/' + logo_bendera.rating" />
              </div>
              <div class="col-6">
                <span>{{ logo_bendera.negara }}</span>
              </div>
            </div>
          </div>
        </div>
        <div class="col-5">
          <div v-for="data_live_liga_one in data_live_liga_one">
            <div class="col-12 d-flex">
              <div id="clubLogo" class="col-1">
                <img
                  :src="'/src/assets/logo_bola/' + data_live_liga_one.club_logo"
                />
              </div>
              <div class="col">
                {{ data_live_liga_one.club_name }}
              </div>
            </div>
          </div>
        </div>
        <div class="col-1">
          <div v-for="data_live_liga_one in data_live_liga_one">
            <div class="col">{{ data_live_liga_one.scores }}</div>
          </div>
        </div>
        <div class="col-1">
          <div v-for="data_live_liga_one in data_live_liga_one">
            <div class="col">
              {{ "(" + data_live_liga_one.session_liga + ")" }}
            </div>
          </div>
        </div>
      </div>
    </ul>
    <!-- end dropdown pertama -->

    <!-- dropdown kedua -->
    <div class="mt-1">
      <div
        class="row btn-lg text-bg-warning p-2"
        data-bs-toggle="dropdown"
        aria-expanded="false"
      >
        <div v-for="logo_bendera in logo_bendera">
          <div id="bendera" class="col-2 d-flex justify-content-between">
            <div>
              <img :src="'/src/assets/bendera/' + logo_bendera.rating" />
            </div>
            <div>
              <img :src="'/src/assets/bendera/' + logo_bendera.bendera" />
            </div>
            <div>
              <span>{{ logo_bendera.negara }}</span>
            </div>
          </div>
        </div>
      </div>
      <ul class="dropdown-menu container">
        <div class="container d-flex">
          <div class="col-2 mt-2">
            <div v-for="logo_bendera in logo_bendera">
              <div id="bendera" class="col-4 d-flex justify-content-between">
                <div class="col-2 ml-2">
                  <img :src="'/src/assets/bendera/' + logo_bendera.rating" />
                </div>
                <div class="col-6">
                  <span>{{ logo_bendera.negara }}</span>
                </div>
              </div>
            </div>
          </div>
          <div class="col-5">
            <div v-for="data_live_liga_two in data_live_liga_two">
              <div class="col-12 d-flex">
                <div id="clubLogo" class="col-1">
                  <img
                    :src="
                      '/src/assets/logo_bola/' + data_live_liga_two.club_logo
                    "
                  />
                </div>
                <div class="col">
                  {{ data_live_liga_two.club_name }}
                </div>
              </div>
            </div>
          </div>
          <div class="col-1">
            <div v-for="data_live_liga_two in data_live_liga_two">
              <div class="col">{{ data_live_liga_two.scores }}</div>
            </div>
          </div>
          <div class="col-1">
            <div v-for="data_live_liga_two in data_live_liga_two">
              <div class="col">
                {{ "(" + data_live_liga_two.session_liga + ")" }}
              </div>
            </div>
          </div>
        </div>
      </ul>
      <!-- end dropdown kedua -->

      <!-- dropdown kedua -->
      <div class="mt-1">
        <div
          class="row btn-lg text-bg-warning p-2"
          data-bs-toggle="dropdown"
          aria-expanded="false"
        >
          <div v-for="logo_bendera in logo_bendera">
            <div id="bendera" class="col-2 d-flex justify-content-between">
              <div>
                <img :src="'/src/assets/bendera/' + logo_bendera.rating" />
              </div>
              <div>
                <img :src="'/src/assets/bendera/' + logo_bendera.bendera" />
              </div>
              <div>
                <span>{{ logo_bendera.negara }}</span>
              </div>
            </div>
          </div>
        </div>
        <ul class="dropdown-menu container">
          <div class="container d-flex">
            <div class="col-2 mt-2">
              <div v-for="logo_bendera in logo_bendera">
                <div id="bendera" class="col-4 d-flex justify-content-between">
                  <div class="col-2 ml-2">
                    <img :src="'/src/assets/bendera/' + logo_bendera.rating" />
                  </div>
                  <div class="col-6">
                    <span>{{ logo_bendera.negara }}</span>
                  </div>
                </div>
              </div>
            </div>
            <div class="col-5">
              <div v-for="data_live_liga_three in data_live_liga_three">
                <div class="col-12 d-flex">
                  <div id="clubLogo" class="col-1">
                    <img
                      :src="
                        '/src/assets/logo_bola/' +
                        data_live_liga_three.club_logo
                      "
                    />
                  </div>
                  <div class="col">
                    {{ data_live_liga_three.club_name }}
                  </div>
                </div>
              </div>
            </div>
            <div class="col-1">
              <div v-for="data_live_liga_three in data_live_liga_three">
                <div class="col">{{ data_live_liga_three.scores }}</div>
              </div>
            </div>
            <div class="col-1">
              <div v-for="data_live_liga_three in data_live_liga_three">
                <div class="col">
                  {{ "(" + data_live_liga_three.session_liga + ")" }}
                </div>
              </div>
            </div>
          </div>
          <div class="container d-flex">
            <div class="col-2 mt-2">
              <div v-for="logo_bendera in logo_bendera">
                <div id="bendera" class="col-4 d-flex justify-content-between">
                  <div class="col-2 ml-2">
                    <img :src="'/src/assets/bendera/' + logo_bendera.rating" />
                  </div>
                  <div class="col-6">
                    <span>{{ logo_bendera.negara }}</span>
                  </div>
                </div>
              </div>
            </div>
            <div class="col-5">
              <div v-for="data_live_liga_four in data_live_liga_four">
                <div class="col-12 d-flex">
                  <div id="clubLogo" class="col-1">
                    <img
                      :src="
                        '/src/assets/logo_bola/' + data_live_liga_four.club_logo
                      "
                    />
                  </div>
                  <div class="col">
                    {{ data_live_liga_four.club_name }}
                  </div>
                </div>
              </div>
            </div>
            <div class="col-1">
              <div v-for="data_live_liga_four in data_live_liga_four">
                <div class="col">{{ data_live_liga_four.scores }}</div>
              </div>
            </div>
            <div class="col-1">
              <div v-for="data_live_liga_four in data_live_liga_four">
                <div class="col">
                  {{ "(" + data_live_liga_four.session_liga + ")" }}
                </div>
              </div>
            </div>
          </div>
        </ul>
        <!-- end dropdown kedua -->
      </div>
    </div>
  </div>
</template>
<style>
  #bendera img,
  #clubLogo img {
    width: 15px;
    height: 10px;
  }
</style>
