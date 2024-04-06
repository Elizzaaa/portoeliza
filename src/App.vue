<template>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.2/css/all.min.css" integrity="sha512-SnH5WK+bZxgPHs44uWIX+LLJAJ9/2PkPKZ5QiAj6Ta86w+fsb2TkcmfRyVX3pBnMFcV7oQPJkl9QevSCWr3W6A==" crossorigin="anonymous" referrerpolicy="no-referrer" />
  <div id="header">
        <div class="container">
            <nav>
                <img src="./assets/Logo2.png" class="logo">
                <ul id="sidemenu">
                  <li><a href="#header" @click="scrollToSection('header')">Home</a></li>
                  <li><a href="#about" @click="scrollToSection('about')">About</a></li>
                  <li><a href="#portfolio" @click="scrollToSection('portfolio')">Project</a></li>
                  <li><a href="#contact" @click="scrollToSection('contact')">Contact</a></li>
                </ul>
            </nav>
            <div class="header-text">
                <p>Mahasiswa Teknik Informatika</p>
                <h1>hello, i'm  <span>ELIZZA HARRI PUTRI</span><br>I'm A Programmer</h1>
            </div>
        </div>
    </div>


  
    <div id="about">
        <div class="container">
            <div class="row">
                <div class="about-col-1">
                    <img src="./assets/profile.png">
                </div>
                <div class="about-col-2">
                    <h1 class="sub-title">About me</h1>
                    <p>hello, nice to meet you all. I'm Elizza Harri Putri. 
                      I'm currently studying at Riau Islamic University and majoring in Informatics 
                      Engineering and I'm currently in my 4th semester. Is it quite short? because 
                      I don't know what to say,thank you :D
                    </p>

                        <div class="tab-titles">
                          <p class="tab-links" :class="{ 'active-link': activeTab === 'skills' }" @click="changeTab('skills')">Hobby</p>
                          <p class="tab-links" :class="{ 'active-link': activeTab === 'experience' }" @click="changeTab('experience')">Experience</p>
                          <p class="tab-links" :class="{ 'active-link': activeTab === 'education' }" @click="changeTab('education')">Education</p>
                          <p class="tab-links" :class="{ 'active-link': activeTab === 'biodata' }" @click="changeTab('biodata')">Biodata</p>
                        </div>
                        <div class="tab-contents" :class="{ 'active-tab': activeTab === 'skills' }" id="skills">
                            <ul>
                                <li><span>Ngedrakor</span><br>The most exciting thing is when you're tired of your college 
                                  assignments, you can do a drama because the story gives an extraordinary effect.</li>
                                <li><span>Sport</span><br>Every afternoon, I definitely squeeze in some exercise, even 
                                  if it's only for a short time because it's so addictive that if you don't sweat it 
                                  out it's weird hehehe</li>
                                <li><span>Cooking</span><br>When I come home, I'm sure cooking is something I do, 
                                  especially when I make the most exciting cakes, I really like it :D</li>
                            </ul>
                        </div>
                        <div class="tab-contents" :class="{ 'active-tab': activeTab === 'experience' }" id="experience">
                            <ul>
                                <li><span>COMING SOON</span></li>
                            </ul>
                        </div>
                        <div class="tab-contents" :class="{ 'active-tab': activeTab === 'education' }" id="education">
                            <ul>
                                <li><span>SD</span><br>SDN 002 PANCOR<br>SDN 012 KP.PANJANG</li>
                                <li><span>SMP</span><br>SMPN 01 KAMPAR</li>
                                <li><span>SMA</span><br>SMAN 01 KAMPAR</li>
                            </ul>
                        </div>
                        <div class="tab-contents" :class="{ 'active-tab': activeTab === 'biodata' }" id="biodata">
                            <ul>
                                <li><span>Nama</span><br>ELIZA HARRI PUTRI</li>
                                <li><span>Jenis Kelamin</span><br>PEREMPUAN</li>
                                <li><span>Tempat Lahir</span><br>PANCOR LAUQ MESJID</li>
                                <li><span>Tanggal Lahir</span><br>07 JULI 2003</li>
                                <li><span>Pekerjaan</span><br>Mahasiswa</li>
                                <li><span>Kewarganegaraan</span><br>Indonesia</li>
                            </ul>
                        </div>
                </div>
            </div>
        </div>
    </div>



  
    <div id="portfolio">
        <div class="container">
            <h1 class="sub-title">My Work</h1>
            <div class="work-list">
                <div class="work">
                    <img src="./assets/Work1.png">
                    <div class="layer">
                        <h3>COMING SOON</h3>
                        <p>I'm still working on some project, will be update soon</p>
                            <a href="#"><i class="fa-solid fa-arrow-up-right-from-square"></i></a>
                    </div>
                </div>
            </div>
            <a href="#" class="btn">See more</a>
        </div>
    </div>


  
    <div id="contact">
        <div class="container">
            <div class="row">
                <div class="contact-left">
                    <h1 class="sub-title">Contact Me</h1>
                    <p><i class="fa-solid fa-paper-plane"></i> example@mail.com</p>
                    <p><i class="fa-solid fa-square-phone"></i> 08012222222</p>
                    <div class="social-icons">
                        <a href="https://www.instagram.com/elizzaharp?igsh=b29vNXR0OGEwZHJi"><i class="fa-brands fa-instagram"></i></a>
                        <a href="https://github.com/Elizzaaa"><i class="fa-brands fa-github"></i></a>
                    </div>
                    <a href="./assets/background.png" download class="btn btn2">Download CV</a>
                </div>
                <div class="contact-right">
                    <form>
                        <input type="text" name="Name" placeholder="Your Name" required>
                        <input type="email" name="Email" placeholder="Your Email" required>
                        <textarea name="Massage" rows="6" placeholder="Your Message"></textarea>
                        <button type="submit" class="btn btn2">Submit</button>
                    </form>
                </div>
            </div>
        </div>
        <div class="copyright">
            <p>Copyright © ElizzaHarriPutri.</p>
        </div>
    </div>
</template>



<script>
export default {
  data() {
    return {
      activeTab: 'skills' // Set initial active tab
    };
  },
  methods: {
    changeTab(tabName) {
      this.activeTab = tabName;
    },
    scrollToSection(sectionId) {
      const element = document.getElementById(sectionId);
      if (element) {
        element.scrollIntoView({ behavior: "smooth" });
      }
    }
  }
};
</script>

<style>
*{
  margin: 0;
  padding: 0;
  font-family: 'Poppins', sans-serif;
  box-sizing: border-box;
}
html{
  scroll-behavior: smooth;
}
body{
  background-color: #897355;
  color: #fff;
}
#header{
  width: 100%;
  height: 100vh;
  background-image: url(./assets/background.png);
  background-size: cover;
  background-position: center;
}
.container{
  padding: 10px 10%;
}
nav{
  display: flex;
  align-items: center;
  justify-content: space-between;
  flex-wrap: wrap;
}

.logo{
  display: flex;
  width: 20vh;
}

nav ul li{
  display: inline-block;
  list-style: none;
  margin: 10px 20px;
}

nav ul li a{
  color: #fff;
  text-decoration: none;
  font-size: 18px;
  position: relative;
}
nav ul li a::after{
  content: '';
  width: 0;
  height: 3px;
  background: #ffdc3f;
  position: absolute;
  left: 0;
  bottom: -6px;
  transition: 0.5s;
}
nav ul li a:hover::after{
  width: 100%;
}
.header-text{
  margin-top: 20%;
  font-size: 30px;
}
.header-text h1{
  font-size: 45px;
  margin-top: 20px;
}
.header-text span{
  color: rgb(255, 235, 169);
}
/*----------about---------*/
#about{
  padding: 80px 0;
  color: #ffffff;
}
.row{
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
}
.about-col-1{
  flex-basis: 35%;
}
.about-col-1 img{
  width: 100%;
  border-radius: 15px;
}
.about-col-2{
  flex-basis: 60%;
}
.sub-title{
  font-size: 60px;
  font-weight: 600;
  color: #fff;
}
.tab-titles{
  display: flex;
  margin: 20px 0 40px;
}
.tab-links{
  margin-right: 50px;
  font-size: 18px;
  font-weight: 500;
  cursor: pointer;
  position: relative;
}
.tab-links::after{
  content: '';
  width: 0;
  height: 3px;
  background: #ffdc3f;
  position: absolute;
  left: 0;
  bottom: -8px;
  transition: 0.5s;
}
.tab-links.active-link::after{
  width: 50%;
}
.tab-contents ul li{
  list-style: none;
  margin: 10px 0;
}
.tab-contents ul li span{
  color: #ffef5d;
  font-size: 14px;
}
.tab-contents{
  display: none;
}
.tab-contents.active-tab{
  display: block;
}

/*----------------Portfolio---------------*/
#portfolio{
  padding: 50px 0;
}
.work-list{
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  grid-gap: 40px;
  margin-top: 50px;
}
.work{
  border-radius: 10px;
  position: relative;
  overflow: hidden;
}
.work img{
  width: 100%;
  border-radius: 10px;
  display: block;
  transition: transform 0.5s;
}
.layer{
  width: 100%;
  height: 0;
  background: linear-gradient(rgba(0,0,0,0.6), #fffc5f);
  border-radius: 10px;
  position: absolute;
  left: 0;
  bottom: 0;
  overflow: hidden;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  padding: 0 40px;
  text-align: center;
  font-size: 14px;
  transition: height  0.5s;
}
.layer h3{
  font-weight: 500;
  margin-bottom: 20px;
}
.layer a{
  margin-top: 20px;
  color: #ffe96e;
  text-decoration: none;
  font-size: 18px;
  line-height: 60px;
  background: #fff;
  width: 60px;
  height: 60px;
  border-radius: 50%;
  text-align: center;
}
.work:hover img{
  transform: scale(1.1);
}
.work:hover .layer{
  height: 100%;
}
.btn{
  display: block;
  margin: 50px auto;
  width: fit-content;
  border: 1px solid #d3c055;
  padding: 14px 50px;
  border-radius: 6px;
  text-decoration: none;
  color: #fff;
  transition: background 0.5s;
}
.btn:hover{
  background: #d3c055;
}

/*--------------contact--------------*/
.contact-left{
  flex-basis: 35%;
}
.contact-right{
  flex-basis: 60%;
}
.contact-left p{
  margin-top: 30px;
}
.contact-left p i{
  color: #d3c055;
  margin-right: 15px;
  font-size: 25px;
}
.social-icons{
  margin-top: 30px;
}
.social-icons a{
  text-decoration: none;
  font-size: 30px;
  margin-right: 15px;
  color: #ababab;
  display: inline-block;
  transition: transform 0.5s;
}
.social-icons a:hover{
  color: #d3c055;
  transform: translateY(-5px);
}
.btn.btn2{
  display: inline-block;
  background: #d3c055;
}
.contact-right form{
  width: 100%;
}
form input, form textarea{
  width: 100%;
  border: 0;
  outline: none;
  background: #262626;
  padding: 15px;
  margin: 15px 0;
  color: #fff;
  font-size: 18px;
  border-radius: 6px;
}
form btn2{
  padding: 14px 60px;
  font-size: 18px;
  margin-top: 20px;
  cursor: pointer;
}
.copyright{
  width: 100%;
  text-align: center;
  padding: 25px 0;
  background: #897355;
  font-weight: 300;
  margin-top: 20px;
}
</style>
