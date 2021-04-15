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
        <p>CONTACT</p>
      </div>
      <img src="@/assets/hamburger.svg" class="hamburger" />
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
  min-height: 95vh;
  display: flex;
  align-items: center;
  flex-direction: column;
  nav {
    height: 10vh;
    width: 90%;
    display: flex;
    align-items: center;
    font-size: 1.25rem;
    .logo {
      height: 100%;
      position: relative;
      img {
        height: 100px;
      }
    }
    .hamburger {
      display: none;
    }
    .menu {
      display: flex;
      min-width: 50%;
      justify-content: space-between;
      align-self: flex-end;
      margin-left: auto;
      gap: 10px;
      p {
        display: flex;
        justify-content: center;
        align-items: center;
        font-size: 1rem;
        width: 25%;
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
    min-height: 80vh;
    width: 90%;
    display: flex;
    align-items: center;
    .hero-content {
      height: 100%;
      display: flex;
      justify-content: center;
      flex-direction: column;
      height: 100%;
      h1 {
        font-size: 6vw;
        margin: 20px 0px;
        color: #020e35;
        font-family: Yeseva One;
      }
      button {
        width: 160px;
        height: 50px;
        border: none;
        outline: none;
        font-size: 1rem;
        font-family: Poppins;
        color: white;
        cursor: pointer;
        background: linear-gradient(to left, #d332f0, #e73587);
      }
    }
    .hero-image {
      width: 100%;
      min-height: 100%;
      display: flex;
      align-items: center;
      img {
        height: inherit;
        width: inherit;
      }
    }
  }
}
@media only screen and (max-width: 700px) {
  .hero {
    .hero-container {
      flex-direction: column;
      justify-content: center;
      .hero-content {
        h1 {
          text-align: center;
          font-size: 10vw;
        }
        button {
          display: none;
        }
      }
    }
    nav {
      .logo {
        img {
          height: 100%;
        }
      }
      .menu {
        display: none;
      }
      .hamburger {
        display: inline;
        margin-left: auto;
        height: 50%;
      }
    }
  }
}
</style>
