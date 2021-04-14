<template>
  <section>
    <h1>About us</h1>
    <p>
      Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
      tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim
      veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea
      commodo consequat.
    </p>
  </section>
</template>

<script>
export default {
  name: "MainAbout",
};
</script>

<style lang="scss" scoped>
section {
  height: 50vh;
  width: 90%;
  display: flex;
  align-items: center;
  flex-direction: column;
  h1 {
    margin: 50px 0 0 0;
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
  p {
    width: 50%;
    text-align: center;
    color: #2b2b2b;
    font-size: 1.25rem;
  }
}
</style>
