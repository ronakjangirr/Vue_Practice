<template>
<h1>Topic -5 Fetch Input Data</h1>
<input type="text" placeholder="Enter Email" v-model="email"/>
<br/>
<br/>
<input type="text" placeholder="Enter Password" v-model="password"/>
<button v-on:click="getData()">Fetch data</button>
</template>

<script>
export default{
    name:"FetchInput",
    data()
    {
        return{
            email:null,
            password:null,
        }
    },
    methods:{
        getData()
        {
            console.log("Values", this.email, this.password)
        }
    }
}
</script>

<style>

</style>