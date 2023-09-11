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
export default (await import("vue")).defineComponent({
  name: "myWeather",
  components: {},
});
</script>

<style></style>
