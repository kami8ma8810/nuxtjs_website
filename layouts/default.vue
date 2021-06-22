<template>
<!-- layoutファイル内には必ず</nuxt>を記述。この</nuxt>部分でpagesの中身が展開される -->
  <div>
    <nav class="navbar navbar-expand-lg navbar-light fixed-top" id="mainNav">
      <div class="container">
        <a class="navbar-brand" href="/"><img src="/images/header-nav-icon.jpg" width="50" height="auto"></a>
        <button class="navbar-toggler navbar-toggler-right" type="button" data-toggle="collapse" data-target="#navbarResponsive" aria-controls="navbarResponsive" aria-expanded="false" aria-label="Toggle navigation">
          Menu
        </button>
        <div class="collapse navbar-collapse" id="navbarResponsive">
          <ul class="navbar-nav ml-auto">
            <li class="nav-item">
              <router-link class="nav-link" to="/">Home</router-link>
            </li>
            <li class="nav-item">
              <router-link class="nav-link" to="/about">About</router-link>
            </li>
          </ul>
        </div>
      </div>
    </nav>
    <nuxt />
    <hr>
    <!-- Footer -->
    <footer>
      <div class="container">
        <div class="row">
          <div class="col-lg-8 col-md-10 mx-auto">
            <p class="copyright text-muted">Copyright &copy; Hayato Kamiyama 2021</p>
          </div>
        </div>
      </div>
    </footer>
  </div>
</template>

<script>
export default {
}
</script>

<style>
/* nuxt-link-exact-active : 現在のURLとリンク先のURLが完全に一致する場合 */
  a.nuxt-link-exact-active{
    font-weight: bold;
  }
</style>
