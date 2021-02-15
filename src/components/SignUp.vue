<template>
  <div class="sign-up">
    <div class="content">
      <h1>Get early access today</h1>
      <p>
        It only takes a minute to sign up and our free starter tier is extremely
        generous. If you have any questions, our support team would be happy to
        help you.
      </p>
      <div>
        <input type="text" />
        <button class="btn">Get Started For Free</button>
      </div>
    </div>
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
.sign-up {
  background: #1b2330;
  box-shadow: 5px 5px 8px rgba(0, 0, 0, 0.25);
  position: absolute;
  z-index: 100;
  width: 863px;
  height: 275px;
  border-radius: 9px;
  left: 50%;
  transform: translate(-50%, -50%);
  color: #ffffff;
}

.content {
  position: relative;
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  text-align: center;
  width: 709px;
  height: 192px;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}

h1 {
  font-size: 32px;
}

p {
  color: #ffffff;
  font-family: 'Open Sans';
  font-size: 14px;
  font-weight: 400;
  line-height: 21px;
  margin: 0 80px;
}

input {
  width: 480px;
  height: 48px;
  border-radius: 24px;
  background: #ffffff;
  box-shadow: 2px 3px 6px rgba(7, 4, 59, 0.16);
  color: #c0c0c0;
  font-family: 'Open Sans';
  font-size: 12px;
  font-weight: 400;
  line-height: 16px;
  margin-right: 20px;
}

button {
  width: 200px;
  height: 48px;
  border-radius: 24px;
  color: #ffffff;
  font-family: Raleway;
  font-size: 14px;
  font-weight: 700;
  line-height: 16px;
  text-align: center;
}

@media (max-width: 700px) {
  .sign-up {
    max-width: 336px;
    min-height: 353px;
  }

  .content {
    width: 280px;
    height: 276px;
  }

  h1 {
    font-size: 18px;
  }

  p {
    margin: 0;
  }

  input {
    width: 280px;
    height: 48px;
    font-size: 10px;
    line-height: 14px;
  }

  button {
    width: 280px;
    height: 48px;
    font-size: 14px;
    margin-top: 24px;
  }
}
</style>
