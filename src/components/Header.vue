<template>
  <header>
    <nav id="nav">
      <ul class="nav__list">
        <li class="nav__item">
          <router-link class="nav__link" to="/">Home</router-link>
        </li>
        <li class="nav__item">
          <router-link class="nav__link" to="/about">About</router-link>
        </li>
      </ul>
    </nav>
  </header>
</template>
<script>
export default {
  name: 'Header'
};
</script>
<style lang="scss" scoped>
#nav {
  padding: 30px;

  .nav__list {
    display: flex;
    justify-content: center;
  }

  .nav__item {
    display: inline;
    padding: 0 rem(5);

    &:first-child {
      border-right: 1px solid $secondary;
    }
  }

  .nav__link {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
