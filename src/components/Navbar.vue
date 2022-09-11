<template>
     <nav>
          <div class="fb-point">
          <div class="logo">
      <img src="piemelogo.png" alt="" class="image-logo">
    </div>
          <input type="text" placeholder="Search" class="field">

           <span class="search" @click="toggle">
            <font-awesome-icon icon="fa-magnifying-glass" />
            
            </span>
          </div>
          
          <div class="navigate">
              
            <span>
               <font-awesome-icon icon="fa-house" />
                </span>            
           <span>
           <font-awesome-icon icon="fa-play" />
           </span>
             <span>
        <font-awesome-icon icon="fa-shop" />
                </span>      
             <span><label class="user" >
                <i class="fas fa-users"></i></label>
                </span>
          </div>
          <div class="extras">
              <label @click="run">
              
                  <div class="user-pic">        
  <img :src="profilePic" v-if="profilePic=this.profilePic ">
              <span v-else>
                <i class="fas fa-user"></i>
                </span>  
</div>   
              <p>{{name}}</p>
              </label>
        
          </div>
      </nav>
</template>

<script>
export default {

}
</script>
<style scoped>
nav{
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    align-items: center;
    gap: 110px;
    padding: 5px 10px;
    box-shadow: 3px 3px 3px #ceced1;
    position: fixed;
    width: 100%;
    z-index: 1;
    background: #fff;
}
nav input{
    border: none;
    border-radius: 36px;
    background: #f0f2f5;
    padding: 7px 16px 9px 36px;
    font-size: 16px;
}
.navigate{
    display: grid;
    grid-template-columns: repeat(4, 1fr);
}
.navigate span{
 display: flex;
justify-content: center;   
border-radius:10px ;
cursor: pointer;
padding: 10px ;
}
.navigate span:hover{
background: #f0f2f5;

}
.navigate i{
    font-size: 28px;  
}
.fa-youtube{
    color: #65676b;
    font-weight: lighter;
}
.fa-store{
    color: #65676b;
    font-weight: lighter;
}

.fa-home{
  font-size: 28px;
    color: #216FD8;
}
.user{
  width: 30px;
    height: 30px;
    border-radius: 50%;
    border: 1px solid #65676b;
    display: flex;
    justify-content: center;
    align-items: center;  
    padding: 0; 
}
.user i{
    color: #65676b;
    font-size: 20px;
}
.extras{
 display: flex;
 gap: 10px;
 justify-content: flex-end;
 padding: 0 24px;
}
.extras span{
    width: 40px;
    height: 40px;
    border-radius: 50%;
    background: #e4e6eb;
    display: flex;
    justify-content: center;
    align-items: center;
    cursor: pointer;
}
.extras span:hover{
    background: #d1d2d4;
}
.fa-user{
    color: #fff;
}
.fb-point{
    display: flex;
    gap: 10px;
    align-items: center;
}
</style>

