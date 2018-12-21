<template>
  <section class="container">
    <div>
      <organisms-common-header />
      <div>
        {{ otenki }}
      </div>

    </div>
  </section>
</template>

<script>
import axios from 'axios'
import OrganismsCommonHeader from "~/components/Organisms/Common/OrganismsCommonHeader";

export default {
  components: {
    OrganismsCommonHeader
  },
  asyncData ({ params }) {
    return axios.get(`https://api.openweathermap.org/data/2.5/weather?id=1850147&appid=79c471b00fcecc60ff2b9a3edf0ba66b`)
      .then((res) => {
        return { otenki: res.data }
      })
  }
}
</script>

<style>
</style>
