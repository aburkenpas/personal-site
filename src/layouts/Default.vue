<template>
  <div class="layout">
    <header class="header">
      <strong>
        <g-link class="logo" to="/">{{ $static.metaData.siteName }}</g-link>
      </strong>
      <nav class="nav">
        <g-link class="nav__link" to="/">Home</g-link>
        <g-link class="nav__link" to="/about">About</g-link>
      </nav>
    </header>
    <slot />
  </div>
</template>

<static-query>
query {
  metaData {
    siteName
  }
}
</static-query>

<style lang="scss">
.logo {
  font-family: "Libre Barcode 39 Extended Text", cursive;
  text-transform: uppercase;
  font-size: 4rem;
  color: $mine-shaft;
  font-weight: 400;

  &:visited,
  &:hover {
    color: $mine-shaft;
  }
}

.layout {
  max-width: 140rem;
  margin: 0 auto;
  padding-left: 20px;
  padding-right: 20px;
}

.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
  height: 80px;
}

.nav__link {
  margin-left: 20px;
}
</style>
