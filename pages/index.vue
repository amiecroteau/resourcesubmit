<template>
  <div>
    <h1 class="title">
      Contact
    </h1>
    <div class="content">
      <form
        name="contact"
        action="/thank-you"
        netlify-honeypot="bot-field"
        method="post"
        netlify
      >
        <input type="hidden" name="form-name" value="contact" />
        <p class="hidden">
          <label>Don’t fill this out: <input name="bot-field"/></label>
        </p>
        <label class="form-label" for="name">
          Name:
        </label>
        <input class="form-field" name="name" id="name" />
        <label class="form-label" for="email">
          Email:
        </label>
        <input class="form-field" name="email" id="email" />
        <label class="form-label" for="message">
          Message:
        </label>
        <textarea class="form-field" name="message" id="message"></textarea>
        <input class="form-button" type="submit" value="Send message" />
      </form>
    </div>

    <div class="links">
      <a href="https://nuxtjs.org/" target="_blank" class="button--green"
        >Documentation</a
      >
      <a
        href="https://github.com/nuxt/nuxt.js"
        target="_blank"
        class="button--grey"
        >GitHub</a
      >
    </div>
  </div>
</template>

<script>
import AppLogo from "~/components/AppLogo.vue";

export default {
  components: {
    AppLogo
  }
};
</script>

<style>
.hidden {
  display: none;
}
.container {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont,
    "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif; /* 1 */
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
