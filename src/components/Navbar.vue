<template>
  <nav className="navbar">
    <div>
      <a to="/"> <img src="../assets/images/Logo.png" /> </a>
    </div>
    <ul>
      <li>
        <a to="/">Features</a>
      </li>
      <li>
        <a to="/register">Team</a>
      </li>
      <li>
        <a to="/login">Sign In</a>
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: 'Navbar',
  props: {},
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
/* Navbar */
.navbar {
  margin: 74px 0;
  padding: 0 6vw;
  display: flex;
  justify-content: space-between;
  align-items: center;
  position: absolute;
  z-index: 5;
  width: 100%;
  height: 52px;
  top: 0;
  opacity: 0.9;
}

.navbar div {
  display: flex;
  align-items: center;
}

.navbar div h1 {
  font-size: 45px;
}

.navbar div img {
  height: 100%;
  width: auto;
  margin-right: 84px;
}
.navbar ul {
  display: flex;
}

.navbar a {
  font-family: Raleway;
  color: #fff;
  padding: 0.45rem;
  margin: 0 0.25rem;
}

.navbar .welcome span {
  margin-right: 0.6rem;
}

@media (max-width: 500px) {
  .navbar div img {
    width: 80px;
    height: 24px;
    margin-right: 84px;
  }

  ul {
    width: 166px;
  }

  li {
    width: 47.29px;
    height: 28px;
    color: #ffffff;
    font-family: Raleway;
    font-size: 12px;
    font-weight: 100;
    line-height: 14px;
    word-break: break-all;
    text-align: center;
  }
}
</style>
