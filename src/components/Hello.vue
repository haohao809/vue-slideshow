<template>
  <div class="hello">
   	<slideshow :slides= 'slides' :inv= 'invTime'></slideshow>
  </div>
</template>

<script>
import slides from './slideshow.vue'
export default {
	components:{
		slideshow:slides
	},
  name: 'hello',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      invTime :2000,
      slides: [
      	{
      		title : '1',
      		src :   require('../assets/1.jpg')
      	},
      	{
      		title : '2',
      		src :   require('../assets/2.jpg')
      	},
      	{
      		title : '3',
      		src :   require('../assets/3.jpg')
      	},
      	{
      		title : '4',
      		src :   require('../assets/4.jpg')
      	},
      
      ]
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
</style>
