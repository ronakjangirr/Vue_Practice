<template>
<h1>Topic- 6 Simple Form</h1>
<ul>
    <li v-for="item in error" v-bind:key="item">{{ item }} not valid</li>
</ul>
<br/>
<input type="text" placeholder="Email" v-model="form.email"/>
<br/>
<input type="password" placeholder="Password" v-model="form.password">
<br/>
<select v-model="form.country">
    <option>India</option>
    <option>China</option>
    <option>USA</option>
</select>
<br/>
<h3>Technology</h3>
<label>Java:</label>
<input type="checkbox" value="java" v-model="form.technology"/>
<br/>
<label>.Net:</label>
<input type="checkbox" value=".net" v-model="form.technology"/>
<br/>
<h3>Gender</h3>
<label>Male</label>
<input type="radio" value="male" name="gender" v-model="form.gender"/>
<br/>
<label>Female</label>
<input type="radio" value="female" name="gender" v-model="form.gender"/>
<br/>

<button v-on:click="login">Submit</button>

</template>

<script>
export default{
    name:"SimpleForm",
    data()
    {
        return{
            form:{
                email:'',
                password:'',
                technology:[],
                gender:''
            },
            error:[],
        }
    },
    methods:{
        // login()
        // {
        //     console.log("login data",this.form)
        // }
        
        login() {
            this.error =[];
            for(const item in this.form) {
                if(this.form[item]==="" || this.form[item].length ===0){
                    this.error.push(item)
                }
            }

            if(this.error.length===0){
                alert("data has been submitted");
            }
            console.log(this.form, this.error)
        }
    }
}
</script>

<style>

</style>