<template>
  <!-- template直下には１つのHTMLのみ ここではdiv（それより下層はいくつでもOK） -->
  <div>
    <!-- Page Header -->
    <header class="masthead" style="background-image: url('/images/hero-bg-index.jpg')">
      <div class="overlay"></div>
      <div class="container">
        <div class="row">
          <div class="col-lg-8 col-md-10 mx-auto">
            <div class="site-heading">
              <h1>おいしい焼肉の食べ方</h1>
              <span class="subheading">生きた命を余す事なく大事に頂く</span>
            </div>
          </div>
        </div>
      </div>
    </header>

    <!-- Main Content -->
    <div class="container">
      <div class="row">
        <div class="col-lg-8 col-md-10 mx-auto">
          <div class="post-preview">
            <a href="post.html">
              <h2 class="post-title">
                赤身はサッと脂はじっくり
              </h2>
              <h3 class="post-subtitle">
              赤身は脂よりもタンパク質が強く、固まる温度が早いので、焼きすぎるとどんどん硬くなる。脂が多いものはある程度焼いても柔らかさが失われないため、しっかり火を通す。</h3>
            </a>
            <p class="post-meta">2021-06-19</p>
          </div>
          <hr>
          <div class="post-preview">
            <a href="post.html">
              <h2 class="post-title">
                タンは網の真ん中で
              </h2>
              <h3 class="post-subtitle">表面に網目の焼き目をつけつつ、中まで火を通しすぎないようにする。最初に焼いた面が少し反りだしたらひっくり返す。</h3>
            </a>
            <p class="post-meta">2021-06-19</p>
          </div>
          <hr>
          <div class="post-preview">
            <a href="post.html">
              <h2 class="post-title">
								迷ったら店員さんに聞く
              </h2>
              <h3 class="post-subtitle">焼肉屋さんにもよるが、店員さんがしっかり知識を持っている場合はいろいろ聞いてみるのが吉。</h3>
            </a>
            <p class="post-meta">2021-06-19</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
  }
</script>

<style lang="scss" scoped>
  a {
    color: #212529;
    transition: all 0.2s;
  }

  #mainNav {
    position: absolute;
    border-bottom: 1px solid #e9ecef;
    background-color: white;
    font-family: 'Open Sans', 'Helvetica Neue', Helvetica, Arial, sans-serif;
  }

  header.masthead {
    margin-bottom: 50px;
    background-repeat: no-repeat;
    background-position: center center;
    background-color: #868e96;
    background-attachment: scroll;
    position: relative;
    background-size: cover;
    text-align: center;
    padding: 200px 0 150px;
    color: white;
  }

  header.masthead .overlay {
    position: absolute;
    top: 0;
    left: 0;
    height: 100%;
    width: 100%;
    background-color: #212529;
    opacity: 0.5;
  }
  .post-subtitle{
    @include clamp(1);
  }

  footer {
    padding: 50px 0 65px;
    text-align: center;
  }
</style>
