<template>
  <section>
    <div class="contact-container">
      <div class="contact-content">
        <h2>Questions,Comments,Concerns?</h2>
        <h1>We'd love to <span>hear</span> from your!</h1>
      </div>
      <div class="contact-form">
        <div>
          <label for="email">Your Email Address</label>
          <input type="text" id="email" placeholder="example@mail.com" />
        </div>
        <div>
          <label for="subject">Subject</label>
          <input type="text" id="subject" placeholder="I would love to.." />
        </div>
        <div>
          <label for="message">Your Email Address</label>
          <textarea
            type="text"
            id="message"
            placeholder="Your message starts with.."
          />
        </div>
        <button>Send a message</button>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "MainContact",
};
</script>

<style lang="scss" scoped>
section {
  width: 100%;
  height: 60vh;
  display: flex;
  justify-content: center;

  .contact-container {
    display: flex;
    width: 90%;
    height: 100%;
    .contact-content {
      margin-top: 5%;
      width: 50%;
      height: 100%;
      display: flex;
      flex-direction: column;
      h2 {
        font-size: 2rem;
        margin: 0;
      }
      h1 {
        font-size: 5rem;
        margin: 0;
        span {
          color: #e73587;
        }
      }
    }
    .contact-form {
      margin-top: 5%;
      width: 50%;
      height: 100%;
      display: flex;
      flex-direction: column;
      gap: 10px;
      div {
        display: flex;
        flex-direction: column;
        input {
          height: 30px;
          font-family: Poppins;
          border: #0000008c 1px solid;
          outline: none;
        }
        input::placeholder {
          color: #0000008c;
        }
        textarea {
          height: 150px;
          font-family: Poppins;
          border: #0000008c 1px solid;
          resize: none;
          outline: none;
        }
        textarea::placeholder {
          color: #0000008c;
        }
      }
      button {
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
  }
}
</style>
