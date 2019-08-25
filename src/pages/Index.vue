<template>
  <Layout>
    <div class="page">
      <div class="left-side-panel">
        <h1>Home</h1>
      </div>

      <div class="content">
        <p
          class="intro"
        >I build internet. I am an Atlanta based Full Stack Developer with a focus in Javascript, Vue.js &amp; JAM stack.</p>
      </div>
    </div>
  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: "Home"
  }
};
</script>

<style lang="scss" scoped>
.page {
  position: relative;
}

.left-side-panel {
  position: absolute;
  top: 10rem;
  left: 3rem;
  transform: rotate(-90deg);
}

.left-side-panel h1 {
  font-size: 1.4rem;
  text-transform: uppercase;
  color: $blue;
}

.content {
  max-width: 80%;
  margin: 8rem auto;
}

.content .intro {
  font-size: 8.2rem;
  margin: 0;
  text-decoration: underline;
}
</style>
