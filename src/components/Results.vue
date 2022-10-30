<template>
<p>Reation Time: {{score}} ms</p>
<p class="rank">{{rank}} </p>
</template>

<script>
    export default{
        props:['score'],
        data(){
            return{
                rank: null
            }
        },
        mounted(){
            if(this.score < 250){
                this.rank = "Kheyliiii khob boood"
            }
            else if(this.score < 400){
                this.rank = "Bad nabooood"
            }
            else{
                this.rank = "Halazone kiii bodiiii"
            }
        }
    }
</script>

<style>
.rank{
    font-size: 1.4em;
    color: aqua;
    font-weight: bold;
}
</style>