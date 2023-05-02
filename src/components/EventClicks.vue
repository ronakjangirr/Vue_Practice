<template>
    <!-- Topic- 3 Events like onclick etc -->
<h1 v-on:mousemove="getConsole()">Events</h1>
<button v-on:click="getData('Button 1 clicked')">Click Me</button>
<h2>{{ count }}</h2>
<button v-on:click="countIncrease()">Increase Count</button>

</template>

<script>
export default{
    name:"EventClicks",
    data()
    {
        return{
            count:0
        }
    },
    methods:{
        getData(data)
        {
            alert(data);
        },
        getConsole()
        {
            console.log("function Called")
        },
        countIncrease(){
            this.count= this.count+1;
        }
    }
}
</script>

<style>

</style>