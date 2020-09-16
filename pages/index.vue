<template>
  <div class="container">
    Home
    <slice-zone type="home" queryType="single" />
  </div>
</template>

<script>
import SliceZone from "vue-slicezone";

export default {
  name: "Home",
  components: { SliceZone }
};
</script>

<style></style>
