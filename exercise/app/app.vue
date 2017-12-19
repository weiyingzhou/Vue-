<style lang="stylus" scoped>
    .box{
        width:200px;
        height:200px;
        border:1px solid red;
    }
</style>
<template>
  <div>
        <div class="box" v-bind:style = "{background:'rgb('+color.r+','+color.g+','+color.b+')'}"></div>
        <range v-bind:color='color' colorName = 'r'></range>   
        <range v-bind:color='color' colorName = 'g'></range>   
        <range v-bind:color='color' colorName = 'b'></range>  
  </div>
</template>
<script>
import range from './components/range.vue';
    export default {
        data : function(){
            return {
                color : {
                    r : 0,
                    g : 0,
                    b : 0
                }
            }
        },
        components : {
            range
        }
    }
</script>
