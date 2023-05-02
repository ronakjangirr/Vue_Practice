<template>
<!-- Topic- 4 Two Way Binding -->
<h1>Topic - 4 Two Way Binding</h1>
<input type="text" v-model="count"/>
<h2>{{ count }}</h2>

</template>

<script>
export default{
    name:"TwowayBind",

    data(){
        return{
            count:10
        }
    },
}
</script>

<style>

</style>