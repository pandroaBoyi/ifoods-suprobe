<template>
<div class="container">
  <div class="row">
    <div class="col-md-6" :class="{'col-md-push-6':desc.right}">
      <article>
        <h1  class="wow slideInDown">{{desc.name}}</h1>
        <h2  class="wow slideInDown" v-if="desc.post">{{desc.post}}</h2>
        <h3  class="wow slideInDown">{{desc.age}}</h3>
        <p  class="wow slideInUp">{{desc.info}}</p>
      </article>
    </div>
  </div>
</div>
</template>

<script>
export default {
  props: {
    desc: Object
  }
}
</script>

<style lang="less" scoped>
@h-fs: 2em;

article {
  background: linear-gradient(to right, rgba(0, 0, 0, 0), rgba(0, 0, 0, .3));
  border-radius: 20px;
  padding: 1em 1.4em;
  color: white;
  text-align: left;
  @media only screen and (max-width:768px) {
    margin-top: 100%;
  }

  h1,
  h2,
  h3 {
    display: inline-block;
  }

  h1 {
    font-size: @h-fs;
  }

  h2 {
    font-size: @h-fs/1.2;
  }

  h3 {
    font-size: @h-fs/1.5;
  }

  p {
    font-size: @h-fs/2;
    line-height: 2;
  }
}
</style>
