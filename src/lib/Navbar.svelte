<script lang="ts">
  let mobileView = false;
</script>

<nav
  class="navbar is-fixed-top is-dark"
  role="navigation"
  aria-label="main navigation"
>
  <div class="navbar-brand">
    <button
      role="button"
      class="navbar-burger burger"
      class:is-active={mobileView}
      aria-label="menu"
      aria-expanded="false"
      data-target="navbarBasicExample"
      on:click={() => {
        mobileView = !mobileView;
      }}
    >
      <span aria-hidden="true" />
      <span aria-hidden="true" />
      <span aria-hidden="true" />
    </button>
  </div>

  <div id="navbarBasicExample" class="navbar-menu" class:is-active={mobileView}>
    <div class="navbar-end">
      <a
        class="navbar-item"
        href="https://github.com/lineville/blackjack"
        target="_blank"
        rel="noopener"
      >
        <span class="icon is-medium">
          <i class="fab fa-github" />
        </span>
        <span>Code</span>
      </a>
    </div>
  </div>
</nav>

<style>
  button {
    border: none;
  }

  .navbar {
    opacity: 90%;
  }
</style>
