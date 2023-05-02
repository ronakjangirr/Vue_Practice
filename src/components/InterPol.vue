<template>
<!-- Topic- 2 InterPoliation -->
<h1>InterPoliation {{ 10 + 10 }} & {{ "hello".length }} in double curlly bracket we can use javascript</h1>
<h2>Email: {{ email }}</h2>
<h2>Mobile: {{ mobile }}</h2>
<h2>Name: {{ getName() }}</h2>
</template>

<script>
export default{
    name:"InterPol",
    
    // By using or creating the function we can pass data in template
    data()
    {
        return{
            email:'anil@test.com',
            mobile:9999,
            getName:function()
            {
                return "sidhu"
            }
        }
    }
}
</script>

<style>

</style>