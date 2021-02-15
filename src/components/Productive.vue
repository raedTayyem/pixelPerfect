<template>
  <div class="productive">
    <img src="../assets/images/stayProductive.png" />
    <div class="productive-content">
      <h3>Stay productive, wherever you are</h3>
      <p>
        Never let location be an issue when accessing your files. Fylo has you
        covered for all of your file storage needs.
      </p>
      <p>
        Securely share files and folders with friends, family and colleagues for
        live collaboration. No email attachments required.
      </p>
      <div class="see">
        <a>
          See how Fylo works
        </a>
        <img class="see-how" src="../assets/images/seeHowIcon.png" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Productive',
  props: {},
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.productive {
  margin: 100px 5vw;
  position: relative;
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(305px, 1fr));
  grid-gap: 50px;
  justify-items: center;
  align-items: center;
  text-align: left;
  color: #fff;
}
.productive * {
  margin-bottom: 20px;
}

.productive p {
  width: 500px;
  height: 48px;
  color: #ffffff;
  font-family: 'OpenSans-Regular';
  font-size: 16px;
  font-weight: 400;
  line-height: 24px;
}

.productive h3 {
  font-family: 'Raleway', sans-serif;
  width: 350px;
  height: 100px;
  color: #ffffff;
  font-size: 40px;
  font-weight: 400;
  line-height: 50px;
}

.see {
  display: flex;
  width: 166px;
  height: 27px;
  border-bottom: 1px solid #62e0d9;
  justify-content: space-between;
  align-items: baseline;
}

.productive a {
  color: #62e0d9;
  font-family: 'OpenSans-Regular';
  font-size: 16px;
  font-weight: 400;
  line-height: 21px;
  margin: 0;
  cursor: pointer;
}

.productive-content {
  display: flex;
  height: 282px;
  flex-direction: column;
  justify-content: space-between;
}

.see-how {
  width: 12px;
  height: 12px;
  margin: 0;
}

@media (max-width: 700px) {
  .productive {
    margin: 160px auto;
    width: 320px;
    height: 499px;
  }

  .productive p {
    width: 320px;
    height: 63px;
    font-size: 14px;
  }

  .productive h3 {
    width: 296px;
    height: 24px;
    font-size: 18px;
  }
}
</style>
