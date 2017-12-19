<style lang="stylus" scoped>

</style>
<template>
        <div>
            <span>{{colorName}}</span>
            <input type="range" min='0' max='255' v-model='color[colorName]'>
            <span>{{color[colorName]}}</span>
        </div>
</template>
<script>
    export default {
        props : ['color','colorName'],
        data : function(){
            return {

            }
        }
    }
</script>
