<template>
  <div id="loginPage">
    <div class="container">
      <div class="form-section">
      <div class="top-section">
        <img src="piemelogo.png" alt="" class="logo">
        <h1>Pieme</h1>
      </div>
      <form action="">
      <section>
                 <input type="email" placeholder="email" class="email-input">
      </section>
        <section>
                <input type="password" placeholder="password" class="password-input"> 
        </section>
     <p class="fgt-pass">forgot password?</p>

     <button class="login" @click.prevent="login">LOGIN</button>
     <span>or</span>
     <button class="signup" @click.prevent="signupPage">SIGN UP</button>
    </form> 
    </div>
   <div class="infor-section">
    <h1>Authentic Local food:</h1>
    <h1>For Us, By Us</h1>
 
   <div class="description">
    <div class="description-image">
<img src="meal.png" alt="">
    </div>
    <p>We connect you to Hosts offering authentic Local dishes</p>
   </div>
   <div class="description">
     <div class="description-image">
      <img src="events.png" alt="">
    </div>
    <p>As a Host, share your Home as a part-time Restaurant or Event venue</p>
   </div>
   <div class="description">
     <div class="description-image">
      <img src="network.png" alt="">
    </div>
    <p>Connect directly with your Guests in Pie Chat</p>
    </div>
   <div class="description">
     <div class="description-image">
      <img src="piemelogo.png" alt="">
    </div>
    <p>The Pie Token is an exclusive payment option on Pieme</p>
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
  signupPage:function(){
    this.$router.push('/signupPage')
  },
  login:function(){

  }
},
}
</script>

<style scoped>
#loginPage{
  background: url(/happy.jpg)no-repeat center;
  background-size:cover;
  object-fit: cover;  
  box-sizing: border-box; 
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
  width: 30vw;
}
.top-section{
  display: flex;
  gap: 20px;
  align-items: center;
  justify-content: center;
}
.top-section h1{
  color: #1976d2;

}
.top-section h2{
  color:#1976d2;
}
.fgt-pass{
    color:#1976d2;
    cursor: pointer;
    text-align: start;
}
.fgt-pass:hover{
  text-decoration: underline;
}
.signup{
   color:#1976d2;
   font-weight: 900;
   border: 2px solid #1976d2;
   border-radius: 32px;
   padding: 10px 20px ;
}
.logo{
  width: 80px;
  height: 90px;
}
form{
  display: flex;
  flex-direction: column;
  gap: 20px;
  padding: 10px 24px;
}
section{
  padding: 10px;
  border-radius: 5px;
  border:0.5px solid #ceced1;
}
section:hover{
  border: 0.5px solid black;
}
.email-input, .password-input{
  padding: 10px 20px;
  outline: none;
  border: none;
}
.infor-section{
  text-align: start;
}
.infor-section h1{
color: #edd00a;
}
.infor-section p{
  color:#fff;
  text-align: start;
  padding-block: 10px;
}
.login{
  border: none;
  padding:10px 20px;
  font-weight: 900;
  border-radius: 32px;
   opacity:0.5;
  background-color:#ceced1;
}
.learn-more{
  background-color: #1976d2;
  color:#fff;
  border-radius:32px;
  padding: 5px 20px;
  border:none;
  cursor: pointer;
  font-weight: 900;
}
.btns{
  display: flex;
  gap: 20px;
  padding-block: 20px;
}
.btns p{
  font-size: 10px;
}

.google-play, .app-store{
  color: #fff;
  border: 0.5px solid #fff;
  cursor: pointer;
  padding: 2px 20px;
  background: transparent;

}
.description{
  display: flex;
  padding-block: 20px;
  align-items: center;
  gap:20px;
}
.description-image{
  width:60px;
  height: 60px;
  border-radius: 50%;
  background-color:#fff;
  object-fit: cover;
  display:flex;
  justify-content: center;
  align-items: center;
  overflow:hidden;
}
.description-image img{
  margin:auto;
  width:80px;
  height: 60px;
  border-radius: 50%;
}
</style>