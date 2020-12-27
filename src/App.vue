<template>
  <h1>{{ title }}</h1>
  <p v-if="isShowing" v-html="title2"></p>
  <p v-else>{{title3}}</p>
  <p>{{ title.toUpperCase() }}</p>
</template>

<script>
export default {
  data() {
    return {
      title: "Hey Vue3",
      title2: "<h1>I am from HTML</h1>",
      title3: "I am from else",
      isShowing: false,
    };
  },
};
</script>

<!-- 
<template>
<h1>Dc Heros</h1>
  <ul id="heros" class="demo">
  <li v-for="hero in dcHeros" :key="hero">
    {{ hero }}
  </li>
</ul>
</template>

<script>
export default {
  data(){
    return {
      dcHeros: ['SuperGirl', 'Flash', 'Batman', 'Superman'],
    }
  }
}
</script>
-->