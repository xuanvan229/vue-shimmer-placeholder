<template>
  <div class="content">
      <div class="image">
        <placeholder></placeholder>
      </div>
      <div class="text">
                <placeholder></placeholder>
      </div>
      <div class="text">
                <placeholder></placeholder>
      </div>
  </div>
</template>

<script>
import placeholder from './placeholder'

export default {
  name: 'hello',
  components: {
    placeholder
  },
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>


<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}

@keyframes placeHolderShimmer{
    0%{
        background-position: -468px 0
    }
    100%{
        background-position: 468px 0
    }
}
.image{
  width: 100px;
  height:100px;
}
.text{
  max-width: 100%;
  height: 20px;
  margin-bottom: 10px;
}
.content{
  margin: 0 auto;
  max-width: 500px;
  border: 1px solid pink;
}
.animated-background {
    animation-duration: 1s;
    animation-fill-mode: forwards;
    animation-iteration-count: infinite;
    animation-name: placeHolderShimmer;
    animation-timing-function: linear;
    background: #f6f7f8;
    background: linear-gradient(to right, #eeeeee 8%, #dddddd 18%, #eeeeee 33%);
    background-size: 800px 104px;
    position: relative;
}
</style>
