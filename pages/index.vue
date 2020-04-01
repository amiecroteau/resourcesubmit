<template>
  <div class="container">
    <column>
      <row>
        <h3 class="subtitle">
          Resource information
        </h3>
      </row>
      <h2 class="title">
        Share your favorite link so I can add to a master list
      </h2>

      <form
        name="contact"
        action="/thank-you"
        netlify-honeypot="bot-field"
        method="post"
        netlify
        class="title"
      >
        <input type="hidden" name="form-name" value="contact" />
        <p class="hidden">
          <label>Don’t fill this out: <input name="bot-field"/></label>
        </p>
        <label class="form-label" for="name">
          Name:
        </label>
        <input class="form-field" name="name" id="name" />

        <label class="form-label" for="link">
          Https Link:
        </label>
        <input class="form-field" name="link" id="message" />

        <input class="form-button" type="submit" value="Send message" />
      </form>
    </column>
  </div>
</template>

<script>
export default {
  components: {}
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
  font-size: 20px;
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
