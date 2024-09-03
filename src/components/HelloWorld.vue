<template>
  <h1>Simple Forms</h1>
  <p>{{ form }}</p>
  <form>
    <lable>Email :</lable>
    <input type="text" placeholder="enter email" v-model="form.email" />
    <br /><br />
    <lable>Password :</lable>
    <input type="password" placeholder="enter password" v-model="form.password" />
    <br /><br />
    <input type="password" placeholder="enter password" v-model="form.password" />
    <br /><br />
    <select v-model="form.country">
      <option>India</option>
      <option>USA</option>
    </select>
    <br />
    <h3>Gender: </h3>
    <input type="radio" name="gender" value="Male" v-model="form.gender" />
    <label>Male</label>
    <input type="radio" name="gender" value="Female" v-model="form.gender" />
    <label>Female</label>
    <br /><br />
    <h3>Technology</h3>
    <input type="checkbox" value="java" v-model="form.technology" />
    <label>Java</label>
    <input type="checkbox" value="C#" v-model="form.technology" />
    <label>C#</label>
    <input type="checkbox" value="SQL" v-model="form.technology" />
    <label>SQL</label>
    <button v-on:click="login()" type="button">Login</button>
  </form>
</template>
<script>
export default {
  name: "HomePage",
  data() {
    return {
      form: {
        email: '',
        password: '',
        country: '',
        gender: '',
        technology: []

      },
      error:[]
    }
  },
  methods: {
    login() {
      this.error=[]
      for(const item in this.form){
        if(this.form[item]==="" || this.form[item].length===0){
          this.error.push(item)
          alert("Please fill all data");
        }
      }
      if(this.error.length===0){
        alert("data submitted")
      }
    }
  }
}
</script>

