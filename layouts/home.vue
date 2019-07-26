<template>
  <div class="body-content">
    <section class="hero is-fullheight bg-img" id="header">
      <div class="hero-head">
        <nav-bar></nav-bar>
      </div>
      <div class="hero-body">
        <div class="typer-title">
          <h1 class="name-title">Gabriel Seymour</h1> <!-- Where to put name-->
          <no-ssr>
            <vue-typer
              class="subtitle"
              id="does-things"
              :pre-type-delay="600"
              :type-delay="70"
              :pre-erase-delay="2000"
              erase-style="clear"
              :text="[
              'plays with lasers.',
              'builds robots.',
              'simulates particles.',
	      'cooks food.',
              //'writes a blog.',
              'makes things.']"
            ></vue-typer>
          </no-ssr>
        </div>
      </div>
      <div class="hero-footer has-text-centered">
        <i class="mdi mdi-chevron-down to-rest" v-scroll-to="'#main'"></i>
      </div>
    </section>
    <div id="main">
      <nuxt/>
    </div>
    <my-footer></my-footer>
  </div>
</template>

<script>
import NavBar from "~/components/NavBar.vue";
import MyFooter from "~/components/MyFooter.vue";

export default {
  components: {
    NavBar,
    MyFooter
  }
};
</script>

<style lang="scss">
</style>
