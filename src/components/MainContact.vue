<template>
  <section>
    <div class="contact-container">
      <div class="contact-content">
        <h2>Questions,Comments,Concerns?</h2>
        <h1>We'd love to <span>hear</span> from your!</h1>
      </div>
      <div class="contact-form">
        <div>
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
  min-height: 60vh;
  margin-bottom: 50px;
  display: flex;
  justify-content: center;

  .contact-container {
    display: flex;
    width: 90%;
    min-height: 100%;
    gap: 30px;
    justify-content: center;
    .contact-content {
      width: 50%;
      height: 100%;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      h2 {
        font-size: 1.5vw;
        margin: 0;
      }
      h1 {
        font-size: 5vw;
        margin: 0;
        span {
          color: #e73587;
        }
      }
    }
    .contact-form {
      width: 50%;
      height: 100%;
      display: flex;
      flex-direction: column;
      justify-content: center;
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
@media only screen and (max-width: 700px) {
  section {
    .contact-container {
      flex-direction: column;
      justify-content: center;
      align-items: center;
      .contact-content {
        width: 80vw;
        justify-content: center;
        align-items: center;
        h1 {
          font-size: 5vw;
        }
        h2 {
          font-size: 4vw;
        }
      }
      .contact-form {
        width: 80vw;
      }
    }
  }
}
</style>
