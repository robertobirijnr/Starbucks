<template>
  <section>
    <div class="circle"></div>
    <header>
      <a href="#" ><img src="../assets/logo.png" class="logo" alt=""></a>
      <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">Menu</a></li>
        <li><a href="#">What's New</a></li>
        <li><a href="#">Contact us</a></li>
      </ul>
    </header>
    <div class="content">
      <div class="textbox">
        <h2>It's not just Coffee <br>It's <span>Starbucks</span></h2>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Inventore blanditiis eligendi cupiditate odio eveniet iste libero error asperiores. Obcaecati vero, illo doloribus vitae pariatur laborum tempore? Eos minima placeat similique.</p>
        <a href="#">Learn More</a>
      </div>
      <div class="imgBox">
        <img src="../assets/img1.png" class="starbucks" alt="">
      </div>
    </div>
    <ul class="thumb">
      <li><img src="../assets/thumb1.png" ></li>
      <li><img src="../assets/thumb2.png" ></li>
      <li><img src="../assets/thumb3.png" ></li>
    </ul>
    <ul class="sci">
      <li><a href="#"><img src="../assets/facebook.png" alt=""></a></li>
      <li><a href="#"><img src="../assets/twitter.png" alt=""></a></li>
      <li><a href="#"><img src="../assets/instagram.png" alt=""></a></li>
    </ul>
  </section>
</template>

<script>
  export default {
    
  }
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,500;1,200;1,300;1,400&display=swap');

*{
  margin:0;
  padding:0;
  box-sizing: border-box;
  font-family: 'Poppins', sans-serif;
}

section{
  position: relative;
  width: 100%;
  min-width: 100vh;
  padding: 100px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  background: #fff;
}
header{
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  padding: 20px 100px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

header .logo{
  position:relative;
  max-width: 80px;
}

header ul{
  position: relative;
  display: flex;
}

header ul li{
  list-style: none ;
}

header ul li a{
  display: inline-block;
  color: #333;
  font-weight: 400;
  margin-left: 40px;
  text-decoration: none;
}

.content{
  position: relative;
  width: 100%;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.content .textbox{
  position: relative;
  max-width: 600px;
}

.content .textbox h2{
  color:#333;
  font-size: 4em;
  line-height: 1.4em;
  font-weight: 500;
}

.content .textbox h2 span{
  color: #017143;
  font-size: 1.2em;
  font-weight: 900;
}
.content .textbox p{
  color: #333;
}
.content .textbox a{
  display: inline-block;
  margin-top: 20px;
  padding: 8px 20px;
  background: #017143;
  color: white;
  border-radius: 40px;
  font-weight: 500;
  letter-spacing: 1px;
  text-decoration: none ;
}
.content .imgBox{
  width: 600px;
  display: flex;
  justify-content: flex-end;
  padding-right: 50px;
  margin-top: 50px;
}
.content.imgBox img{
  max-width: 340px;
}
.thumb{
  position: absolute;
  left: 50%;
  bottom: 20px;
  transform: translateX(-50%);
  display: flex;
}

.thumb li{
  list-style: none;
  display: inline-block;
  margin: 0 20px;
  cursor: pointer;
  transition: 0.5s;
}
.thumb li img{
  max-width: 60px;
} 

.thumb li:hover{
  transform: translateY(-15px);
}
.sci{
  position: absolute;
  top: 50%;
  right: 30px;
  transform: translateY(-50%);
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}
.sci li{
  list-style: none;
}

.sci li a{
  display: inline-block;
  margin: 5px 0;
  transform: scale(0.6);
}
.circle{
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: #017143;
  clip-path: circle(600px at right 800px);
}

</style>