<template>
  <div id="sigupPage">
    <div class="container">
        <div class="form-section">
            <div class="top-section">
              <h2>Connect Share & Host Events and Meals</h2>
              <h2 class="btlogin" @click="loginPage">Back to login</h2>
            </div>
            <div class="wrapper">
                <form>

               <section>
                 <input type="text" placeholder="name" class="name-input">
               </section>
       
          <section>
                 <input type="email" placeholder="email" class="email-input">
      </section>
       <section>
                <input type="number" placeholder="number" class="number-input"> 
        </section>
        <section>
                <input type="password" placeholder="password" class="password-input"> 
        </section>
         <section>
                <input type="password" placeholder="confirm password" class="password-input"> 
        </section>
            </form>
           <div class="second-segment">

            <form action="">
              <section>
                 <input type="text" placeholder="Username" class="name-input">
      </section>
      <select name="" id="">
        <option value="male">Male</option>
        <option value="female">Female</option>
      </select>
      <section>
                 <input type="text" placeholder="select your interest" class="name-input">
      </section>
      <button @click.prevent="register" class="register">Register</button>
            </form>
           </div>

            </div>
            


        </div>
       
    </div>

  </div>
</template>

<script>
export default {
data() {
  return {
    
  }
},
methods: {
    register:function(){

    },
    loginPage:function(){
      this.$router.push('/LoginPage')
    }
  },
}
</script>

<style scoped>
#sigupPage{
  background: url(/happy.jpg)no-repeat center;
  background-size:cover;
  object-fit: cover;  
  min-height: 100vh;
  width: 100vw;
}
.container{
  background-color: rgba(0, 0, 0, 0.5);
  min-height: 100vh;
  width: 100vw;
  box-sizing: border-box; 
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 40px;
}
.form-section{
  background-color: #fff;
  padding:40px 16px;
  border-radius: 5px;
  /* width: 60vw; */
}
.top-section{
  display: flex;
  gap: 20px;
  align-items: center;
  justify-content: center;
}
.wrapper{
  display: flex;
  gap:20px;
  flex-wrap: wrap;
}
form{
  display: flex;
  flex-direction: column;
  gap: 20px;
  padding: 10px 24px;
}
section{
  padding: 10px 24px;
  border-radius: 5px;
  border:0.5px solid #ceced1;
}
section:hover{
  border: 0.5px solid black;
}
.email-input, .password-input, .name-input, .number-input{
  padding: 10px 20px;
  outline: none;
  border: none;
}
select{
  padding:10px;
}
.btlogin{
  color: #1976d2;
  text-decoration: underline;
  cursor: pointer;
}
.register{
  padding: 10px 20px;
  border: none;
  background-color:#1976d2;
  color:#fff;
  cursor: pointer;
  border-radius: 5px;
  font-weight: 600;
}
</style>