<template>
<div id="download">
  <div class="container">
    <div class="row">
      <div class="col-xs-12 col-sm-12 col-md-6">
        <aside class="wow fadeInDown">
          <img src="/static/img/home/app.png">
        </aside>
      </div>
      <div class="col-xs-12 col-sm-12 col-md-6">
        <article class="wow fadeInDown">
          <h2>超极探针APP下载</h2>
          <section>
            <img src="/static/img/home/download-ios.png" >
            <a :href="prodLink.DOWNLOAD_IOS">
                <i class="icon iconfont">&#xe68c;</i>
                <span>IOS</span>
              </a>
          </section>
          <section>
            <img src="/static/img/home/download-andriod.png" >
            <a :href="prodLink.DOWNLOAD_ANDRIOD" >
                <i class="icon iconfont">&#xe68d;</i>
                <span>Andriod</span>
              </a>
          </section>
        </article>
      </div>
    </div>
  </div>
</div>
</template>

<script>
export default {

}
</script>

<style lang="less" scoped>
#download {
  .mixin-bg(@url: @footerlink-download-bg-url;
  @height: @common-fullscreenpic-height);
  .mixin-center;

  .row {

    aside {
      img {
        max-width: 100%;

        @media only screen and (max-width: 768px) {
          display: none;
        }
      }
    }

    article {
      color: @common-fs-color;

      h2 {
        color: currentColor;
      }

      section {
        display: inline-block;
        width: 12em;
        padding: 10px;

        img {
          border-radius: 1em;
          padding: 10px;
          margin: 0 0 2em 0;
        }

        a {
          display: block;
          text-decoration: none;
          font-size: 1em;
          color: currentColor;
          padding: .8em 0;
          border: .05em solid currentColor;
          border-radius: .5em;

          &:hover {
            text-decoration: none;
            background: rgba(255, 255, 255, .2);
          }
        }
      }
    }
  }
}
</style>
