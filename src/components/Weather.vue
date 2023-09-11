<template>
  <div class="container p-0">
    <div class="d-flex">
      <div class="card main-div w-100">
        <div class="p-3">
          <h2 class="mb-1 day">Monday</h2>
          <p class="text-light date mb-0">date</p>
          <small>time</small>
          <h2 class="place">
            <i class="fa fa-location">Rio <small>country</small></i>
          </h2>
          <div class="temp">
            <h1 class="weather-temp">18&deg;</h1>
            <h2 class="text-light">description</h2>
          </div>
        </div>
      </div>
      <div class="card card-2 w-100">
        <table class="m-4">
          <tbody>
            <tr>
              <th>Sea Level</th>
              <td>100</td>
            </tr>

            <tr>
              <th>Sea Level</th>
              <td>100</td>
            </tr>

            <tr>
              <th>Sea Level</th>
              <td>100</td>
            </tr>
          </tbody>
        </table>

        <DaysWeather></DaysWeather>
        <div id="div_Form" class="d-flex m-3 justify-content-center">
          <form action="">
            <input
              type="button"
              value="Change location"
              class="btn change-btn btn-primary"
            />
          </form>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import DaysWeather from "./DaysWeather.vue";

export default (await import("vue")).defineComponent({
  name: "myWeather",
  components: { DaysWeather },
  props: {
    city: String,
  },
  data() {
    return;
  },
});
</script>

<style>
body {
  background-color: #343d4b;
}

.weather-temp {
  margin: 0;
  font-weight: 700;
  font-size: 4em;
}

h2.mb-1.day {
  font-size: 3rem;
  font-weight: 400;
}

.main-div {
  border-radius: 20px;
  color: #fff;
  background-image: ;
  background-size: cover;
  background-position: center;
  background-blend-mode: overlay;
  background-color: rgba(0, 0, 0, 0.5);
  background-repeat: no-repeat;
}

.temp {
  position: absolute;
  bottom: 0;
}

.main-div:hover {
  transform: scale(1.1);
  transition: transform 0.5s ease;
  z-index: 1;
}

.card-2 {
  background-color: #212730;
  border-radius: 20px;
}

.card-details {
  margin-left: 19px;
}

.h1_left {
  position: absolute;
  bottom: 25px;
  left: 16px;
  font-size: 3vw;
  line-height: 1.2;
}

.h3_left {
  position: absolute;
  left: 16px;
  font-size: 2vw;
  line-height: 0.5;
}

.h3_left small {
  font-size: 1rem;
}

table {
  position: relative;
  left: 15px;
  border-collapse: separate;
  border-spacing: 15px;
  width: 85%;
  text-align: left;
  max-width: 600px;
  margin: 0 auto;
}

th,
td {
  font-size: 18px;
  color: #fff;
}

td {
  text-align: right;
}

table,
tr:hover {
  color: red;
}

.change_btn {
  background-image: liner-gradient(to right, cyan, magenta);
}

.change_btn {
  transform: scale(0.9);
  transition: transform 0.1 ease;
}
</style>
