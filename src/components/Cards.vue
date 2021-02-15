<template>
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
          Whether you're sharing holidays photos or work documents, Fylo has you
          covered allowing for all file types to be securely stored and shared.
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Cards',
  props: {},
};
</script>

<style scoped>
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

@media (max-width: 500px) {
  .cards {
    width: 320px;
    margin: auto;
  }

  .card-preview p {
    width: 270px;
  }
}
</style>
