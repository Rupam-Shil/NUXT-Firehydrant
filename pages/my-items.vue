<template>
  <div class="container">
    <MyItems v-for="rental in myRentals" :key="rental.id" :item="rental" />
  </div>
</template>

<script>
import { mapState } from "vuex";
export default {
  layout: "no-nav",
  computed: {
    ...mapState(["myRentals"])
  }
};
</script>

<style></style>
