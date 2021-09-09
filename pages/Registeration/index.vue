<template>
  <div class="container">
    <div class="row">
     <div class="col-12 text-center" >
       <h1>Registration Form</h1>
     </div>
    </div>
  <div class="form-row">
    <div class="form-group col-md-12">
      <label for="inputEmail4">Email</label>
      <input v-model="form.email" type="email" class="form-control" id="inputEmail4" placeholder="Email">
    </div>
        <div class="form-group col-md-6">
      <label for="firstName">First Name</label>
      <input v-model="form.firstName" type="text" class="form-control" id="fname" placeholder="First name">
    </div>
        <div class="form-group col-md-6">
      <label for="lastName">Last Name</label>
      <input v-model="form.lastName" type="text" class="form-control" id="lname" placeholder="Last name">
    </div>
    <div class="form-group col-md-6">
      <label for="inputPassword4">Password</label>
      <input v-model="form.password" type="password" class="form-control" id="inputPassword1" placeholder="Password">

  </div>
  </div>

  
  <button type="submit" @click="register" class="btn btn-primary">Register</button>
  </div>
</template>

<script>
export default {
  data(){
    return{
      form:{
        firstName:'',
        lastName:'',
        email:'',
        password:''
      }
    }
  },
  methods:{
    async register(){
      console.log('a')
      await this.$axios.post('/auth/register',this.form);

      this.$auth.login({data:this.form})
      this.$router.push({name:'index'})
    }
  }
}
</script>
