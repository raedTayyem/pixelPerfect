<template
  ><div class="reviews">
    <img class="review" src="../assets/images/card1.png" />
    <img class="review" src="../assets/images/card2.png" />
    <img class="review" src="../assets/images/card3.png" />
  </div>
</template>

<script>
export default {
  name: 'Reviews',
  props: {},
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.reviews {
  position: relative;
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(360px, 1fr));
  padding-bottom: 360px;
  justify-items: center;
  align-items: baseline;
  grid-gap: 39px;
  max-width: 1180px;
  margin: auto;
}

.review {
  width: 360px;
  height: 200px;
}

.review:first-child {
  width: 380px;
  height: 259px;
}
@media (max-width: 700px) {
  .review {
    width: 280px;
    height: 160px;
  }

  .review:first-child {
    margin-right: 20px;
    width: 290px;
    height: 219px;
  }

  .reviews {
    grid-gap: 24px;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  }
}
</style>
