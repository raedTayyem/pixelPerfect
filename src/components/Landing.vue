<template>
  <div class="landing">
    <div class="second-background" />
    <div class="landing-inner">
      <img class="inner-image" src="../assets/images/main.png" />
      <h1>All your files in one secure location, accessible anywhere.</h1>
      <p>
        Fylo stores all your most important files in one secure location. Access
        them wherever you need, share and collaborate with friends family, and
        co-workers.
      </p>
      <button class="btn">Get Started</button>
    </div>

    <Cards />

    <Productive />

    <Reviews />

    <SignUp />
  </div>
</template>

<script>
import Productive from './Productive.vue';
import Reviews from './Reviews';
import Cards from './Cards';
import SignUp from './SignUp';

export default {
  name: 'Landing',
  props: {},
  components: {
    Productive,
    Reviews,
    Cards,
    SignUp,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.second-background {
  width: 100%;
  height: 100%;
  position: absolute;
  overflow: hidden;
  background: url(../assets/images/second-bc.png) no-repeat center center /
    cover;
  background-position-y: 78vh;
}

.landing {
  z-index: 2;
  position: relative;
  top: 200px;
  /* display: contents; */
}

.landing-inner {
  position: relative;
  display: flex;
  flex-direction: column;
  margin: 0 25vw;
  align-items: center;
  justify-content: center;
  color: #fff;
}

.landing-inner h1 {
  width: 710px;
  height: 120px;
  color: #ffffff;
  font-family: 'Raleway-Bold';
  font-size: 40px;
  font-weight: 400;
  line-height: 60px;
  text-align: center;
  margin: 30px 0;
}

.landing-inner p {
  width: 520px;
  height: 90px;
  color: #ffffff;
  font-family: 'OpenSans-Regular';
  font-size: 20px;
  font-weight: 400;
  line-height: 30px;
  text-align: center;
}

.landing-inner button {
  margin-top: 30px;
  width: 280px;
  height: 56px;
  font-size: 16px;
}

.sign-up {
  position: absolute;
  z-index: 100;
  width: 863px;
  height: 275px;
  left: 50%;
  transform: translate(-50%, -50%);
}

/* Mobile Styles */
@media (max-width: 700px) {
  .landing-inner {
    margin: 0 5vw;
  }

  h3 {
    font-size: 18px;
  }

  .landing-inner h1 {
    width: 280px;
    font-size: 24px;
    line-height: 36px;
    height: 108px;
  }

  .landing-inner p {
    width: 250px;
    font-size: 14px;
    line-height: 21px;
    height: 84px;
  }
}
</style>
