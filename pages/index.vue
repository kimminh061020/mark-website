<template>
  <div class="site-wrapper">
  <header class="site-home-header">
    <div class="site-header-content">
                    <span class="site-title">
                        <img class="my-face" src="../assets/images/my-face.jpg" alt="Mark Nguyen's Website">
                        <div class="intro anim-typewriter">
                        Hi, I'm Mark Nguyen
                        </div>
                    </span>
                    <span class="site-description anim-typewriter-2" >I am a self-taught programmer.</span>
                    <p style="color: #818189; margin: 24px auto 0; text-align: center; max-width: 500px; animation: pulse 5s infinite;">I'm building an app called <a href="https://weather-app-mark-nguyen.netlify.app" target="_blank">Awesome Weather</a> using Nuxt.js</p>
                    <br>
                    <div>
<a href="https://twitter.com/Minh17234068?ref_src=twsrc%5Etfw" class="twitter-follow-button" data-show-count="false">Follow me</a><script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>
<!-- Place this tag where you want the button to render. -->
<a class="github-button" href="https://github.com/kimminh061020" aria-label="Follow me on GitHub">Follow me</a><script async defer src="https://buttons.github.io/buttons.js"></script>
</div>
                </div>
  </header>
  <main class ="content">
    <div class="img-card">
  <div class="tile is-horizontal is-parent">
    <div class="tile is-child box img-wrapper">
      <a href="https://weather-app-mark-nguyen.netlify.app" target="_blank">
      <img src="https://www.sciencenewsforstudents.org/wp-content/uploads/2021/02/1030_LL_snow.jpg" alt="Placeholder image">
      <p class="fade">Awesome Weather App</p>
      </a>
      </div>
      
    <div class="tile is-child box img-wrapper">  
      <a href="https://to-do-app-mark-nguyen.netlify.app" target="_blank">
      <img src="https://images.viblo.asia/1460817c-e8dd-45fe-a3fe-00c86256553a.jpg" alt="Placeholder image">
      <p class="fade">To do app</p>
      </a>
    </div>

    <div class="tile is-child box img-wrapper">
      <a href="https://drive.google.com/file/d/11yNroh39ojR8wKA7VWCEMbb7Eza34a3P/view?usp=sharing" target="_blank">
      <img src="https://dpbnri2zg3lc2.cloudfront.net/en/wp-content/uploads/2021/01/web_dev_pillar_page.jpg" alt="Placeholder image">
      <p class="fade">Techical Support Experience</p>
      </a>
    </div>
  </div>



  </div>
  </main>
  </div>
  
</template>

<script>




export default {
  mounted() {
    let userwayscript = document.createElement('script')
      userwayscript.setAttribute('src', 'https://cdn.userway.org/widget.js')
      userwayscript.setAttribute('data-account', 'Y1wLGDw71E')
      document.head.appendChild(userwayscript)
  }
}
</script>

<style scoped>
.site-home-header .site-header-content {
    padding: 5vw 3vw 6vw;
}

.site-header-content {
    z-index: 100;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 6vw 3vw;
    max-height: 100%;
    color: #fff;
    background: #090a0b no-repeat 50%;
    background-size: cover;
}

.site-home-header .site-title {
    text-align: center;
}

.site-title {
    z-index: 10;
    margin: 0 0 0 -2px;
    padding: 0;
    font-size: 3rem;
    line-height: 1em;
    font-weight: 600;   
}

.intro {
  text-align: center;
    white-space: nowrap;
    overflow: hidden;
}

.my-face {
    width: 150px;
    border-radius: 100%;
    display: block;
    margin: 0 auto 24px;
}

@media (prefers-color-scheme: dark) {
img {
    opacity: .9;
}
}
img {
  vertical-align: middle;
  border: 0;
  max-width: 100%;
  height: 100%;
}

.site-home-header {
    height: auto;
    width: 100%;
    background: #090a0b no-repeat 50%;
}

.site-description {
    z-index: 10;
    margin: 0;
    padding: 10px 0;
    font-size: 1.2rem;
    line-height: 1.4em;
    font-weight: 400;
    opacity: .8;
    text-align: center;
    white-space: nowrap;
    overflow: hidden;
}

.content {
  display: flex;
    flex-direction: column;
    align-items: center;
    padding-top: 5%;
    padding-bottom: 5%;
    background: rgb(0, 0, 0 , 95%);
}
.img-card {
  width: 80%;
}

.box {
  padding: 0;
  margin: 0.4rem !important;
}
.img-wrapper {
  position: relative;
}
.img-wrapper a p {
  position: absolute;
  inset: 0;
  font-size: 2rem;
  padding: 1rem;
  background: rgb(0, 0, 0 , 60%);
  color: white;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.img-wrapper  a  img, .img-wrapper  a  p {
  transition: 200ms ease-in-out;
}

.img-wrapper  a  p.fade {
  opacity: 0;
}

.img-wrapper:hover  a  p.fade {
  opacity: 1;
}

h1 {
  text-align: center;
  cursor: pointer;
  margin-top: 3em;
}

/* Animation */
.anim-typewriter{
  animation: typewriter 4s steps(44) 1s 1 normal both,
             blinkTextCursor 500ms steps(44) infinite normal;
}
@keyframes typewriter{
  from{width: 0;}
  to{width: 24em;}
}
@keyframes blinkTextCursor{
  from{border-right-color: rgba(255,255,255,.75);}
  to{border-right-color: transparent;}
}

.anim-typewriter-2 {
  animation: typewriter 4s steps(44) 3s 1 normal both,
             blinkTextCursor 500ms steps(44) infinite normal;
}
</style>