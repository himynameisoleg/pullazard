<template>
  <div class="container">
    <div class="section">
      <h1 class="title is-1">PULL A ZARD</h1>
      <h2 class="subtitle">Great pulls await</h2>
    </div>
    
    <div class="section">
      <div class="columns">

        <div class="column is-flex is-justify-content-center is-one-third" v-for="i in [1, 2, 3]" :key="i.id">
          <figure class="image">
            <img :src="require('@/assets/cards/c1.jpeg')">
          </figure>
        </div>

      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data() {
    return {
      cards: [
        {path: require('@/assets/cards/c1.jpeg')},
        {path: require('@/assets/cards/b1.jpeg')},
        {path: require('@/assets/cards/v1.jpeg')}
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
h3 {
  margin: 40px 0 0;
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
</style>
