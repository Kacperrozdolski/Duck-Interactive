<template>
  <section>
    <div>
      <h1>Our Valuable Services</h1>
    </div>
    <div class="services-container">
      <div class="service-card">
        <img src="../assets/mobileService.png" alt="" srcset="" />
        <h2>App Development</h2>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
          eiusmod tempor incididunt ut labore et dolore magna aliqua.
        </p>
        <button>READ MORE</button>
      </div>
      <div class="service-card">
        <img src="../assets/webService.png" alt="" srcset="" />
        <h2>Web Development</h2>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
          eiusmod tempor incididunt ut labore et dolore magna aliqua.
        </p>
        <button>READ MORE</button>
      </div>
      <div class="service-card">
        <img src="../assets/designService.png" alt="" srcset="" />
        <h2>UI/UX Development</h2>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
          eiusmod tempor incididunt ut labore et dolore magna aliqua.
        </p>
        <button>READ MORE</button>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "MainServices",
};
</script>

<style lang="scss" scoped>
section {
  min-height: 100vh;
  width: 100%;
  background: linear-gradient(#fff 50%, #020e35 50% 100%);
  display: flex;
  align-items: center;
  flex-direction: column;
  h1 {
    margin: 0;
    color: #020e35;
    font-size: 3rem;
    position: relative;
  }
  h1::before {
    position: absolute;
    bottom: 0;
    left: 25%;
    width: 50%;
    height: 5px;
    border-radius: 5rem;
    background: #e73587;
    content: "";
  }
  .services-container {
    width: 90%;
    display: flex;
    align-items: center;
    justify-content: space-between;
    height: 90vh;
    .service-card {
      width: 350px;
      height: 75%;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      text-align: center;
      gap: 10px;
      img {
        width: 90%;
      }
      h2 {
        margin: 0;
      }
      p {
        margin: 0;
        font-size: 0.9rem;
      }
      button {
        width: 140px;
        height: 40px;
        margin: 0;
        border: none;
        outline: none;
        font-family: Poppins;
        color: white;
        cursor: pointer;
        background: linear-gradient(to left, #d332f0, #e73587);
      }
    }
    .service-card:nth-child(1) {
      background: #fdf8e3;
    }
    .service-card:nth-child(2) {
      background: #f0f3fa;
    }
    .service-card:nth-child(3) {
      background: #feeff0;
    }
  }
}
</style>
