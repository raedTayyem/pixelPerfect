<template
  ><div className="footer">
    <div className="footer-content">
      <div>
        <a to="/"> <img src="../assets/images/Logo.png" /> </a>
        <p>
          orem ipsum dolor sit amet, consectetur adipiscing elit. Nunc et
          convallis ante, at suscipit sem.
        </p>
      </div>
      <div>
        <p>+1-543-123-4567</p>
        <p>example@fylo.com</p>
      </div>
      <div>
        <p>About Us</p>
        <p>Jobs</p>
        <p>Press</p>
        <p>Blog</p>
      </div>
      <div>
        <p>Contact Us</p>
        <p>Terms</p>
        <p>Privacy</p>
      </div>
      <div><p></p></div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Footer',
  props: {},
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.footer {
  background-color: #0b1524;
  position: absolute;
  z-index: 5;
  left: 0;
  bottom: 0;
  height: 517px;
  width: 100%;
  position: relative;
  display: grid;
  justify-items: center;
  align-items: center;
  text-align: center;
}

.footer-content {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  grid-auto-rows: auto;
  grid-gap: 5vw;
  align-items: center;
  justify-items: center;
  width: 1200px;
  margin: 0 19vw;
  margin-top: 60px;
}

.footer div img {
  height: 100%;
  width: auto;
}
</style>
