<template>
    <div>
      <Navbar />
      <br />
      <form style="width: 400px; padding: 0px 20px 0px 20px" class="mx-auto">
        <br />
        <h4>Collect Meter Reading</h4>
        <br />
        <div class="mb-3">
          <label for="readingInput" class="form-label">Search Meter Number</label>
          <input
            type="text"
            class="form-control"
            id="readingInput"
            placeholder="Seach meter number here"
            aria-describedby="emailHelp"
          />
        </div>
        <button type="submit" class="btn btn-primary" onclick="handleSubmit">Search</button>
      </form>
      <br />
    </div>
  </template>

  <script>
  export default {
    // layout: 'blog',
    head() {
      return {
        script: [
          {
            src: "https://cdnjs.cloudflare.com/ajax/libs/jquery/3.1.1/jquery.min.js",
          },
        ],
        link: [
          {
            rel: "stylesheet",
            href: "https://fonts.googleapis.com/css?family=Roboto&display=swap",
          },
        ],
      };
    },
    mounted() {
      this.$nextTick(() => {
        this.$nuxt.$loading.start();
        setTimeout(() => this.$nuxt.$loading.finish(), 500);
      });
    },
    methods: {
        handleSubmit() {
            return alert('You hit me?')
        }
    }
  };
  </script>


  <style scoped>
  h6 {
    font-family: Circular, Arial, sans-serif;
    /* Dejavu Sans, Arial, Verdana, sans-serif; */
  }
  </style>