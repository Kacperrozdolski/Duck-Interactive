<template>
  <section class="hero">
    <nav>
      <div class="logo">
        <img src="@/assets/logo.png" alt="" />
      </div>
      <div class="menu">
        <p>HOME</p>
        <p>ABOUT</p>
        <p>SERVICES</p>
        <p>PORTFOLIO</p>
        <p>CONTACT US</p>
      </div>
    </nav>
    <div class="hero-container">
      <div class="hero-content">
        <h1>We Create Content that ranks</h1>
        <button>SEE OUR WORK</button>
      </div>
      <div class="hero-image">
        <img src="@/assets/heroImage.png" alt="" />
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "MainHero",
};
</script>

<style lang="scss" scoped>
.hero {
  width: 100%;
  height: 95vh;
  display: flex;
  align-items: center;
  flex-direction: column;
  nav {
    height: 10vh;
    width: 90%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    font-size: 1.25rem;
    .logo {
      height: 100%;
      position: relative;
      img {
        position: absolute;
        height: 140%;
      }
    }
    .menu {
      width: 50%;
      display: flex;
      justify-content: center;
      align-items: center;
      p {
        display: flex;
        justify-content: center;
        align-items: center;
        font-size: 1.25rem;
        width: 20%;
        text-align: center;
        height: 50px;
        color: #2b2b2b;
        font-weight: 500;
      }
      p:nth-child(5) {
        background: linear-gradient(to left, #d332f0, #e73587);
        color: white;
        height: 50px;
      }
    }
  }
  .hero-container {
    height: 80vh;
    width: 90%;
    display: flex;
    .hero-content {
      width: 40%;
      height: 100%;
      h1 {
        font-size: 6rem;
        color: #020e35;
      }
      button {
        width: 160px;
        height: 50px;
        border: none;
        outline: none;
        font-size: 1.25rem;
        font-family: Poppins;
        color: white;
        cursor: pointer;
        background: linear-gradient(to left, #d332f0, #e73587);
      }
    }
    .hero-image {
      height: 100%;
      width: 60%;
      display: flex;
      img {
        height: 100%;
        margin-left: auto;
      }
    }
  }
}
</style>
