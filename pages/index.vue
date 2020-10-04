<template>
  <section>
    <div>
      <Logo :width="350" />
      <h1 class="title">NUXT<span class="green">JS</span></h1>
      <h2 class="subtitle">SkyWayチュートリアル</h2>
      <div class="links">
        <a
          href="http://localhost/index.html"
          target="_blank"
          class="button--green"
          >通話を開始 <IconLink
        /></a>
        <NLink to="/about" class="button--grey">チャットを開始</NLink>
      </div>
    </div>
  </section>
</template>

<script>
import Logo from "~/components/Logo.vue";
import IconLink from "~/components/IconLink.vue";

export default {
  components: {
    Logo,
    IconLink,
  },
};
</script>

<style scoped>
.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont,
    "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  display: block;
  font-weight: 400;
  font-size: 100px;
  color: #2E495E;
  letter-spacing: 1px;
  font-size: 6em;
}
.green {
  color: #00C48D;
}

.subtitle {
  font-weight: 300;
  font-size: 3em;
  color: #2E495E;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
