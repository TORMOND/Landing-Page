<template>
  <div class="footer">
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
        <p></p>
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
    background-color: #fff;
    padding:20px;
}
.company-details{
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 10px;
}
.company-details span{
    color: #777777;
}
.phone-details, .email-details, .address-details{
    display: flex;
    flex-direction: column;
    gap: 10px;
}
footer{
    padding: 20px;
    color: #777777;
    font-size: 12px;
    display: flex;
    justify-content: space-between;
}
</style>