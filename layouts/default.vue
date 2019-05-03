<template>
  <div>
    <header>
      <nav class="navbar navbar-expand-lg navbar-light bg-light">
        <a 
          class="navbar-brand"
          href="#">Git practice</a>
        <button
          class="navbar-toggler"
          type="button"
          data-toggle="collapse"
          data-target="#navbarNav"
          aria-controls="navbarNav"
          aria-expanded="false"
          aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"/>
        </button>
        <div
          id="navbarNav"
          class="collapse navbar-collapse">
          <ul class="navbar-nav">
            <li class="nav-item active">
              <a
                class="nav-link"
                href="#">Home
                <span class="sr-only">(current)</span>
              </a>
            </li>
          </ul>
        </div>
      </nav>
    </header>
    <nuxt/>
  </div>
</template>

<style>
html {
  font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}
</style>
