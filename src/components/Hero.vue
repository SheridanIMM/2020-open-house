<template>
  <section class="container align-items-center hero">
    <div class="row">
      <div class="col">
        <h1> Meet </h1>
        <h1> Your Sheridan </h1>
        <h1 class="outline"> IMM2020 Grads </h1>
        <p class="hero__text">& see what they can do for you </p>
      </div>
    </div>
  </section>
</template>

<script>
export default {
	name: "Hero",
	data: function(){
    return {};
  }
};
</script>
<style scoped lang="scss">
@import "@/styles/mixins/typography";
@import "@/styles/mixins/breakpoints";

h1 {
  margin-bottom: -8px;
}

.outline {
  -webkit-text-stroke-width: 2px;
  -webkit-text-stroke-color: $color-purple;
  color: rgba(0, 0, 0, 0);
  margin-bottom: 3rem;
}

.hero__text {
  @include text-body-lg();
}

@include media-breakpoint-up(xs) {
  .outline {
    -webkit-text-stroke-width: 1.5px;
  }
}

// @include media-breakpoint-up(lg) {
//     h1 {
//       margin-bottom: -20px;
//     }
//   .outline {
//     -webkit-text-stroke-width: 1.2px;
//   }
//   .hero__text {
//     margin-top: 10px;
//   }
// }
</style>
