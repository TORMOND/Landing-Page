<template>
  <div class="home">
    <div id="side-menu">
      <div class="closer">
        <font-awesome-icon class="side-menu-icon" @click="closeMenu" icon="xmark" />
      </div>
      <ul>
        <li>HOME</li>
        <li>ABOUT</li>
        <li>UPCOMING EVENTS</li>
        <li>MORE</li>
        <li>HOST NEWS</li>
        <li>TESTIMONIALS</li>
        <li>CONTACT</li>
      </ul>

      <span>P:+2540000000</span>
     <span>@: support@pieme.info</span>
    </div>
    <div class="container">
 
 <div class="home-intro" @scroll="scrollListener">

       <video playsinline autoplay loop class="video">
    <source src="newVideo.mp4" type="video/mp4" autoplay loop  >
  </video>


<nav>
    <div class="logo">
<img src="piemelogo.png" alt="" class="image-logo">
    </div>
    <div class="button">
  <button class="btn-scroll">Become a Host</button>
    </div>
  
    <div class="sidemenu">
<font-awesome-icon class="side-menu-icon" @click="closeMenu" icon="xmark" v-if="toggled" />
<font-awesome-icon class="side-menu-icon" @click="toggleMenu" icon="align-justify" v-else  />


    </div>
  </nav>


  <div class="wrapper">
    <div class="side-infor">
      <h1>Pieme</h1>
      <h5>FOR US BY US</h5>
      <div class="line"></div>
      <div class="social-icons">
         <div class="brand">
          <font-awesome-icon icon="fabFacebook" class="brand-icons" /> 
         </div>
         <div class="brand">
          <font-awesome-icon icon="fab-twitter" class="brand-icons" />
         </div>
         <div class="brand">
          <font-awesome-icon icon="fab-instagram" class="brand-icons" />
         </div>
         <div class="brand">
          <font-awesome-icon icon="fab-linkedin" class="brand-icons" />
         </div>
      </div>
    </div>
    <div class="main-infor">
<h1>PIEME. FOR US, BY US.</h1>
<p>Do you love cooking? Turn your home into a part-time resturant
and host events at you home.</p>
<div class="btns">
<button class="login" @click="loginPage">LOGIN</button>
<button class="host">BECOME A HOST</button>
</div>

    </div>
  </div>

    </div>
    <div class="about-section">
       <div class="about-details">
      <div class="headers">
        <h1>ABOUT</h1>
       <h1 class="pieme-header">PIEME</h1>
      </div>
     
        <p>
          Pieme is the first of its kind social platform that enables individuals to turn their home into part-time restaurant or event venues.
        </p>
        <p>
         Just like Uber decentralized the taxi business, Airbnb decentralized the hotel industry,
         Pieme is decentralizing the restaurant business by enabling individuals to monetize home-cooked meals.
        </p>
        <p>
         With Pieme, any one can turn their home into a part-time restaurant or event venue and share authentic 
         local dishes with the community around them.
       </p>   
       </div>
        <div class="image-section">
          <!-- <img src="pieme1.png" alt=""> -->
          <div class="overlay">PIEME</div>
        </div>
    
    </div>
<div id="contain">
 <div class="offers-section">
      <div class="offers-header">
       <h1>WHAT PIEME OFFERS</h1>
      </div>
      <div class="offers-table">
        <div class="offer">
          <div class="offer-title">
            <h3>FOOD CONTENT CREATORS.</h3>
          </div>
          <div class="progress-line"></div>
          <div class="offer-list">
               <ul>
                <li>Monetizes Skills</li>
                <li>A place to show case skills</li>
                <li>A place to network withother creators</li>
               </ul>
          </div>
        </div>
        <div class="offer">
          <div class="offer-title">
            <h3>CULINARY SCHOOL STUDENTS AND GRADUATES.</h3>
          </div>
          <div class="progress-line"></div>
          <div class="offer-list">
               <ul>
                <li>A platform to network with their role model Chefs and content creators.</li>
                <li>A place to show case skills</li>
                <li>A place to launch their career</li>
               </ul>
          </div>
        </div>
        <div class="offer">
          <div class="offer-title">
            <h3>CHEFS AND HOME COOKS</h3>
          </div>
          <div class="progress-line"></div>
          <div class="offer-list">
               <ul>
                <li>A place to show case their skills</li>
                <li>Earn from orders</li>
                <li>A platform to network</li>
               </ul>
          </div>
        </div>
        <div class="offer">
          <div class="offer-title">
            <h3>HOME BAKERS</h3>
          </div>
          <div class="progress-line"></div>
          <div class="offer-list">
               <ul>
                <li>Pieme provides a platform to reach a wider audience/More customers.</li>
                <li>Showcase their Cakes</li>
                <li>A place to network</li>
               </ul>
          </div>
        </div>
        <div class="offer">
          <div class="offer-title">
            <h3>AIRBNB HOSTS/ USERS.</h3>
          </div>
          <div class="progress-line"></div>
          <div class="offer-list">
               <ul>
                <li>A new niche of customers, who want space and meals.</li>
                <li>A new revenue stream.</li>
                <li>Pieme provides a social platform.</li>
               </ul>
          </div>
        </div>
        <div class="offer">
          <div class="offer-title">
            <h3>ANYONE WHO WANTS TO CONNECT.</h3>
          </div>
          <div class="progress-line"></div>
          <div class="offer-list">
               <ul>
                <li>A social platform.</li>
                <li>A community.</li>   
               </ul>
          </div>
        </div>
      </div>
    </div>
    <div class="pieme-news-section">
      <div class="news-headers">
      <h1>PIEME</h1><h1 class="pieme-header">NEWS</h1>
      </div>
      <div class="carousel">
        <div class="carousel-elements">

      <carousel :slides="pictures" controls indicators>

      </carousel>
         
        </div>
      </div>
    </div>
    <div class="promo-section">
      <div class="banner">
        <div class="top-section">
          <h2>WHAT HOSTS SAY?</h2>
          <p>Great Concept that's giving many of us a chance to grow our skills.</p>
        </div>

        <div class="commentor-profile">
          <img src="" alt="" class="profilePic">
          <div class="profile-details">
            <div class="name">Chef Raphael</div>
            <div class="institution">
              <p>Raphael Studios</p>
            </div>
          </div>
        </div>
      </div>
    </div>
</div>
   
    <Footer />
    </div>
   <div class="scroll-button">

   </div>

  </div>
</template>

<script>
import Carousel from "@/components/Carousel.vue";
import Footer from '../components/Footer.vue'
export default {
  name: 'Home',
  components:{
Footer, Carousel
  },
  data() {
    return {
      pictures:[
       ['chefs.png','college.png'],
       ['dine.png','onboarding.png'],
       ['chefs.png','college.png'],
       ['dine.png','onboarding.png'],
      ],
      toggled:false
    }
  },
  methods: {
    loginPage:function(){
    this.$router.push('/LoginPage')
    },
    toggleMenu:function(){
      this.toggled=true
    const sideMenu = document.querySelector('#side-menu')
    sideMenu.style.marginLeft = "80%"
    sideMenu.style.transition = "0.8s";
    },
    closeMenu:function(){
      this.toggled=false
    const sideMenu = document.querySelector('#side-menu')
    sideMenu.style.marginLeft = "120vw"
    sideMenu.style.transition = "0.8s";
    },
    scrollListener:function(){
      const header =document.querySelector("nav")
      const sectionOne = document.querySelector(".home-intro")
      const btnScroll = document.querySelector('.btn-scroll')
      const sectionOneOptions = {
        rootMargin:"-150px 0px 0px 0px"
      }
      const sectionOneObserver = new IntersectionObserver(function(
        entries, sectionOneObserver
      ){
        entries.forEach(entry=>{
          if(!entry.isIntersecting){
            header.classList.add("nav-scrolled")
            btnScroll.style.display = "block"
          }else{
            header.classList.remove("nav-scrolled")
            btnScroll.style.display = "none"
          }
        })
      }, sectionOneOptions)
      sectionOneObserver.observe(sectionOne)
    },
  },
  mounted() {
    this.scrollListener()
  },
}
</script>
<style scoped>
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
  flex-direction: column;
  gap: 5px;
  padding-left: 20px;
}
.home{
  position:relative;
  overflow: hidden;
}
.home-intro{
  height: 80vh;
  background:transparent;
  color:#fff;
  position:relative;
  width: 100vw;
  box-sizing: border-box;
}
.video{
  position:absolute;
  z-index: -1;
  margin-left: -680px;
  box-sizing: border-box;
  width:99vw;
  object-fit: cover;
  height:inherit;
}
nav{
    background: transparent;
    width: 100vw;
    box-sizing: border-box;
    display: flex;
    padding:10px 60px;
    justify-content: space-between;
    align-items: center;
}
.side-menu-icon{
  color: #b19777;
  font-size: 32px;
  font-weight: 100;
  cursor: pointer;
}
.nav-scrolled{
background-color:#fff;
position:fixed;
z-index: 2;
padding:10px 60px;
box-shadow: 3px 3px 3px #ceced1;
}
.btn-scroll{
  background-color:#166FA5;
  color:#fff;
  padding: 10px 80px;
  border-radius:32px;
  display: none;
  border: none;
  margin-top: 20px;
  cursor: pointer;
  transition: 1s;
}
.closer{
  display: flex;
  justify-content: center;
  text-align: center;
}
.image-logo{
  width: 80px;
  height: 80px;
}
.wrapper{
  display: flex;
  gap: 40px;
  padding: 10px 40px;
}
.line{
  width: 1px;
  height: 80px;
  border-right: 0.5px solid #fff;
  margin: 10px auto;
}
.side-infor{
  display: flex;
  flex-direction: column;
}
.main-infor{
  display: flex;
  flex-direction: column;
  justify-content: end;
  align-items:flex-start;
  margin-top: 100px;
}
.main-infor h1{
  font-size: 56px;
}
.main-infor p{
  text-align: start;
  width: 500px;
}
.btns{
  display: flex;
  gap: 10px;
  padding: 40px 0;
}
.login, .host{
  background: transparent;
  border:1px solid #fff;
  color: #fff;
  padding: 10px 20px;
  cursor: pointer;
}
.login:hover{
animation-name: slide;
  animation-duration: 1s;
  animation-timing-function: linear;
}
.host:hover{
animation-name: slide;
animation-direction: normal;
animation-iteration-count: infinite;
  animation-duration: 1s;
  animation-timing-function: linear;
}
@keyframes slide {
  0%{
   background: transparent;
  }
  100%{
  background:#fff;
  }
}
/* ABOUT SECTION */

.about-section{
  display:grid;
  grid-template-columns: repeat(2,1fr);
  gap:20px;
  margin: 0 auto;
   padding:40px 20px 50px 20px;
  background-color: #ffffff;
  height: 65vh;
}
.about-section p{
  text-align: start;
  padding: 20px;
  color: #777777;

}
.headers, .news-headers{
  display: flex;
  gap:20px;
  padding: 20px ;
  font-size: 24px;
  box-sizing: border-box;
}

.pieme-header{
   color: #BAD8F5;
}
.image-section{
  object-fit: contain;
   background: url(/pieme1.png)no-repeat center;
    background-size: cover;
    height: 400px;
    width: 40vw;
    position: relative;
    transition: 0.8s;
}
.image-section:hover{
  height: 380px;
}
.overlay{
  background-color: #F4F4F4;
  position: absolute;
  margin-left: 54%;
  margin-top: 68%;
  padding: 18px 80px;
}
#side-menu{
  position:fixed;
  margin-left:120vw;
  width: 280px;
  height: 100vh;
  background-color: #Fff;
  z-index: 1;
  text-align:start;
  padding: 20px 16px;
  
}
#side-menu ul{
  display: flex;
  flex-direction: column;
  height: 80%;
  justify-content: center;
}
#side-menu li{
  list-style: none;
  padding-block: 10px;
}
#contain{
 background: url(/cust4.jpg)no-repeat center;
  background-size:cover;
  object-fit: cover;
}
.offers-section{
  padding: 20px 50px 0px 50px;
  color: #fff;
   background-color: rgba(0, 0, 0, 0.5);
   width: 100%;
   box-sizing: border-box;
}
/* header{
  transform-style:preserve-3d ;
  z-index: -1;
  height: 100%;
  width: 100%;
  position: relative;
}
.bkgd{
  position:absolute;
  height: 100%;
  width: 100%;
  object-fit: cover;
  transform: translateZ(-10px) scale(2);
  z-index: -1;
} */
.offers-header{
  text-align: start;
  font-size: 24px;
  padding:24px 0;
}
.offers-table{
  display: grid;
  grid-template-columns: repeat(3,1fr);
   /* background-color: rgba(0, 0, 0, 0.5); */
  /* gap: 40px; */
}
.offer{
  height: 220px;
  padding: 20px 30px 60px 30px;
  border-left: 0.5px solid #fff;
  text-align:start;
  border-bottom: 0.5px solid #fff ;
  margin-right: 40px;
}
.offer h3{
  text-align:start;
  padding:20px 0;
}
.offer:hover{
  /* background-color: #383838; */
  cursor: pointer;
}
.offer li{
  list-style: none;
  padding-block: 5px;
}
.pieme-news-section{
  background-color: #fff;
  padding: 20px;
  height: 80vh;
}
.elements{
  display:grid;
  grid-template-columns: repeat(2,1fr);
  gap: 10px;
  padding: 20px;
}
.elements img{
  width:45vw;
  height: inherit;
}
.promo-section{
  height: 332px;
  background-color: rgba(0, 0, 0, 0.5);
  padding: 20px;
  margin: 20px 0;
}
.banner{
  background-color: #fff;
  width: 30vw;
  height: inherit;
  margin-left: 50vw;
  padding: 20px;
  box-sizing: border-box;
}

@media all and (max-width:500px) {
  #side-menu{
  margin-left:0vw;
  width:100vw;
  display: none;
}
.about-section{
  display:grid;
  grid-template-columns: repeat(1,1fr);
  gap:20px;
  margin: 0 auto;
  box-sizing: border-box;
  padding: 20px 20px;
}
nav{
background-color:#fff;
position:fixed;
z-index: 1;
box-shadow: 3px 3px 3px #ceced1;
 padding: 10px;
}
.nav-scrolled{
  padding: 10px;
}
.btn-scroll{
  margin-top: 20px;
  border-radius: 0px 32px  32px 0px ;
}
.main-infor{
  display: flex;
  flex-direction: column;
  justify-content: end;
  align-items:flex-start;
  margin-top: 200px;
}
.main-infor h1{
  font-size:24px;
  padding: 10px 0;
}
.main-infor p{
  text-align: start;
  width:70vw;
}
.offers-table{
  display: grid;
  grid-template-columns: repeat(1,1fr);
  /* gap: 40px; */
}
.image-section{
  object-fit: contain;
   background: url(/pieme1.png)no-repeat center;
    background-size: cover;
    height: 300px;
    width: 80vw;
    position: relative;
    transition: 0.8s;
}
.overlay{
  background-color: #F4F4F4;
  position: absolute;
  margin-left: 14%;
  margin-top: 88%;
  padding: 18px 80px;
}
.side-infor{
  display: none;
}
}

</style>
