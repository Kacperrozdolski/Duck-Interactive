<template>
  <section>
    <div>
      <h1>Our Work</h1>
    </div>
    <div class="work-container">
      <div class="work-card">
        <div class="card-image">
          <img src="../assets/workImage_01.png" alt="" srcset="" />
        </div>
        <div class="card-content">
          <h2>Brand Name</h2>
          <h3>iOS | ANDROID | WEB DEVELOPMENT</h3>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
            eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim
            ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut
            aliquip ex ea commodo consequat.
          </p>
        </div>
      </div>
      <div class="work-card">
        <div class="card-image">
          <img src="../assets/workImage_02.png" alt="" srcset="" />
        </div>
        <div class="card-content">
          <h2>Brand Name</h2>
          <h3>iOS | ANDROID | WEB DEVELOPMENT</h3>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
            eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim
            ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut
            aliquip ex ea commodo consequat.
          </p>
        </div>
      </div>
      <div class="work-card">
        <div class="card-image">
          <img src="../assets/workImage_03.png" alt="" srcset="" />
        </div>
        <div class="card-content">
          <h2>Brand Name</h2>
          <h3>iOS | ANDROID | WEB DEVELOPMENT</h3>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
            eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim
            ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut
            aliquip ex ea commodo consequat.
          </p>
        </div>
      </div>
      <div class="work-card">
        <div class="card-image">
          <img src="../assets/workImage_04.png" alt="" srcset="" />
        </div>
        <div class="card-content">
          <h2>Brand Name</h2>
          <h3>iOS | ANDROID | WEB DEVELOPMENT</h3>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
            eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim
            ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut
            aliquip ex ea commodo consequat.
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
section {
  width: 100%;
  min-height: 100vh;
  display: flex;
  align-items: center;
  flex-direction: column;
  background: #020e35;
  padding-bottom: 100px;
  h1 {
    margin: 0 0 50px 0;
    color: #ffffff;
    font-family: Yeseva One;
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
  .work-container {
    width: 90%;
    min-height: 100vh;
    display: flex;
    gap: 50px;
    flex-direction: column;
    .work-card {
      min-height: 55vh;
      width: 100%;
      display: flex;
      gap: 30px;
      .card-content {
        width: 50%;
        height: 100%;
        color: white;
        p {
          font-size: 1.25rem;
        }
      }
      .card-image {
        width: 50%;
        min-height: 100%;
        display: flex;
        align-items: center;
        justify-content: center;
        img {
          width: 60%;
        }
      }
    }
    .work-card:nth-child(1) > .card-image {
      background: #f09532;
    }
    .work-card:nth-child(2) {
      flex-direction: row-reverse;
      text-align: right;
    }
    .work-card:nth-child(2) > .card-image {
      background: #8c32f0;
    }
    .work-card:nth-child(3) > .card-image {
      background: #e73587;
    }
    .work-card:nth-child(4) {
      flex-direction: row-reverse;
      text-align: right;
    }
    .work-card:nth-child(4) > .card-image {
      background: #32d6f0;
    }
  }
}
@media only screen and (max-width: 700px) {
  section {
    .work-container {
      .work-card {
        flex-direction: column !important;
        .card-content {
          width: 100%;
          text-align: center;
        }
        .card-image {
          width: 100%;
          height: 100%;
        }
      }
    }
  }
}
</style>
