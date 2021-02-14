<template>
  <div class="landing">
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

    <div class="cards">
      <div class="card-preview">
        <img src="../assets/images/1.png" />
        <div>
          <h3>Access your files, anywhere</h3>
          <p>
            The ability to use a smartphone, tablet, or computer to access your
            account means your files follow you everywhere.
          </p>
        </div>
      </div>

      <div class="card-preview">
        <img src="../assets/images/2.png" />
        <div>
          <h3>Security you can trust</h3>
          <p>
            2-factor authentication and user-controlled encryption are just a
            couple of the security features we allow to help secure your files.
          </p>
        </div>
      </div>

      <div class="card-preview">
        <img src="../assets/images/3.png" />
        <div>
          <h3>Real-time collaboration</h3>
          <p>
            Securely share files and folders with friends, family and colleagues
            for live collaboration. No email attachments required.
          </p>
        </div>
      </div>

      <div class="card-preview">
        <img src="../assets/images/4.png" />
        <div>
          <h3>Store any type of file</h3>
          <p>
            Whether you're sharing holidays photos or work documents, Fylo has
            you covered allowing for all file types to be securely stored and
            shared.
          </p>
        </div>
      </div>
    </div>
    <div class="productive">
      <img src="../assets/images/stayProductive.png" />
      <div class="productive-content">
        <h3>Stay productive, wherever you are</h3>
        <p>
          Never let location be an issue when accessing your files. Fylo has you
          covered for all of your file storage needs.
        </p>
        <p>
          Securely share files and folders with friends, family and colleagues
          for live collaboration. No email attachments required.
        </p>
        <div class="see">
          <a>
            See how Fylo works
          </a>
          <img class="see-how" src="../assets/images/seeHowIcon.png" />
        </div>
      </div>
    </div>

    <div class="reviews">
      <img class="review" src="../assets/images/card1.png" />
      <img class="review" src="../assets/images/card2.png" />
      <img class="review" src="../assets/images/card3.png" />
    </div>
  </div>

  <img class="second-background" src="../assets/images/second-bc.png" />
</template>

<script>
export default {
  name: 'Landing',
  props: {},
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.second-background {
  z-index: 1;
  top: 848px;
  position: absolute;
}

.landing {
  z-index: 2;
  position: relative;
  top: 200px;
}

.landing-inner {
  position: relative;
  display:flex;
  flex-direction:column;
  margin: 0 25vw;
  align-items: center;
  justify-content: center;
  color: #fff;
}

.landing-inner h1 {
  width: 710px;
  height: 120px;
  color: #ffffff;
  font-family: "Raleway-Bold";
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
  font-family: "OpenSans-Regular";
  font-size: 20px;
  font-weight: 400;
  line-height: 30px;
  text-align: center;
}

.landing-inner button {
  margin-top: 30px;
  width: 280px;
  height: 56px;
  border-radius: 28px;
  background: linear-gradient(152deg, hsl(176, 68%, 64%), hsl(198, 60%, 50%));
  box-shadow: 2px 3px 6px rgba(0, 0, 0, 0.16);
  color: #fff;
  font-size: 16px;
  font-weight: 700;
}

.cards {
  position: relative;
  margin: 0 19vw;
  margin-top: 60px;
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(305px, 1fr));
  grid-auto-rows: auto;
  grid-gap: 8.5vw;
  justify-items: center;
  align-items: center;
  text-align: center;
}

.card-preview {
  height: 215px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-between;
}

.card-preview img {
  width: 104px;
  padding: 10px;
  color: #9a1f40;
  transition: border-bottom 0.5s;
}

.card-preview h3 {
  color: #fff;
}

.card-preview p {
  color: #fff;
  width: 330px;
  font-size: 14px;
  font-weight: 400;
  line-height: 21px;
  font-family: 'Open Sans';
}

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


.productive p{
  width: 520px;
  height: 48px;
  color: #ffffff;
  font-family: "OpenSans-Regular";
  font-size: 16px;
  font-weight: 400;
  line-height: 24px;
}


.productive h3{
 font-family: [Raleway](https://fonts.google.com/specimen/Raleway);
  width: 350px;
  height: 100px;
  color: #ffffff;
  font-size: 40px;
  font-weight: 400;
  line-height: 50px;

}

.see{
  display:flex;
  width: 166px;
  height: 27px;
  border-bottom: 1px solid #62e0d9;
  justify-content: space-between;
  align-items: baseline;
}

.productive a{
  color: #62e0d9;
  font-family: "OpenSans-Regular";
  font-size: 16px;
  font-weight: 400;
  line-height: 21px;
  margin: 0;
}

.productive-content{
display: flex;
height: 282px;
flex-direction: column;
justify-content: space-between;
}

.see-how{
  width: 12px;
  height: 12px;
  margin: 0;
}

.reviews{
  position: relative;
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(370px, 1fr));
  margin: 100px 5vw;
  justify-items: center;
  align-items: baseline;
  grid-gap: 50px;
}

.review{
width: 360px;
height: 200px;
}

.review:first-child{
width: 380px;
height: 259px;
}
/* Mobile Styles */
@media (max-width: 700px) {
  .landing-inner {
    margin: 0 5vw;
  }
  .cards {
    margin: 0 10vw;
  }


.productive p{
  width: 300px;
  height: 48px;
}


 h3{
  font-size:18px
}

.landing-inner h1 {
  width: 300px;
  font-size:18px
}
.landing-inner p {
  width: 300px;
}
}
</style>
