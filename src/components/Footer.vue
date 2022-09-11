<template>
  <div class="footer">
    <div class="other-platforms">
         <div class="btns"> 
      <button class="learn-more">Learn more</button>
      <button class="google-play">
        <font-awesome-icon icon="fa-brands fa-google-play" class="google-play-icon" />
        <div>
          <p>GET IT ON</p>
          <h3>Google Play</h3>
        </div>
      </button>
      <button class="app-store">
        <font-awesome-icon icon="fa-brands fa-app-store-ios" class="app-store-icon" />
          <div>
          <p>Download on the</p>
          <h3>App Store</h3>
        </div>
      </button>
    </div>
    </div>
    <div class="company-details">
        <div class="phone-details">
         <p>Phone</p>
         <span>+254 794643128</span>
        </div>
        <div class="email-details">
        <p>Email</p>
        <span>support@pieme.info</span>
        </div>
    <div class="address-details">
      <p>Our Address</p>
      <span>Mutahaiga North Gardens, Balozi Estate</span>
        </div>
    </div>
    <footer>
        <p>@2022 Pieme.All rights reserved</p>
        <div class="social-icons">
         <div class="brand">
          <font-awesome-icon icon="fa-brands fa-facebook" class="brand-icons" /> 
         </div>
         <div class="brand">
          <font-awesome-icon icon="fa-brands fa-twitter" class="brand-icons" />
         </div>
         <div class="brand">
          <font-awesome-icon icon="fa-brands fa-instagram" class="brand-icons" />
         </div>
         <div class="brand">
          <font-awesome-icon icon="fa-brands fa-linkedin" class="brand-icons" />
         </div>
      </div>
        <p>Privacy Policy Terms & Conditions</p>
    </footer>
  </div>
</template>
<script>

export default {
    
}
</script>

<style scoped>
.footer{
    background-color: #777777;
    color:#fff;
    padding:20px;
}
.company-details{
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 10px;
}
.company-details span{
    color: #dfdbdb;
}
.phone-details, .email-details, .address-details{
    display: flex;
    flex-direction: column;
    gap: 10px;
}
footer{
    padding: 20px 20px 5px 0px;
    color: #dfdbdb;
    font-size: 12px;
    display: flex;
    justify-content: space-between;
    align-items:center;
}
.other-platforms{
    display: flex;
    justify-content: center;
}
.learn-more{
  background-color: #1976d2;
  color:#fff;
  padding: 8px 20px;
  border:none;
  cursor: pointer;
  font-weight: 900;
}
.btns{
  display: flex;
  gap: 20px;
  padding-block: 20px;
  flex-wrap: wrap;
}
.btns p{
  font-size: 10px;
}

.google-play, .app-store{
  color: #fff;
  border: 0.5px solid #fff;
  cursor: pointer;
  padding: 2px 10px;
  background: transparent;
  display:flex;
  gap:5px;
}
.google-play-icon, .app-store-icon{
  font-size:24px;
}
.brand{
  width: 40px;
  height: 40px;
  border: 0.5px solid #fff;
  border-radius: 50%;
  display: flex;
  justify-content: center;
  align-items: center;
  cursor: pointer;
  transition: 0.8s;
}
.brand:hover{
   border: 1px solid #1976d2; 
}
.brand-icons{
  font-size: 12px;
  color: #fff;
}
.social-icons{
  display: flex;
  gap: 5px;
}
</style>