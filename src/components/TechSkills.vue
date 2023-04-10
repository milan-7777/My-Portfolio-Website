<template>
  <div id="cover">
    <video autoplay muted loop id="myVideo">
      <source src="/cover.mp4" type="video/mp4">
      Your browser does not support HTML5 video.
    </video>

    <div id="content">
      <div id="photo">
        <img src="/imgCV.jpg" alt="My Photo">
      </div>

      <div id="intro">
          <p id="title">Technical Skills</p>
          <p>1 year experience</p>
          <p>HTML, CSS (SCSS,SASS), CSS animations, responsive design, CSS Libraries (Bootstrap, Tailwind)</p>
          <p>Figma,Git, Wordpress and WooCommerce, familiar with Jest and Cypress testing, Canvas 2D</p><br>
          <p>Javascript, Vue.js (Vue3), Pinia, Vue Router, REST API, React basics</p>
          <div id="logos">
            <img src="../assets/3logos.png" alt="html css js logo">
            <img src="../assets/wplogo.png" alt="wordpress logo">
            <img src="../assets/vuejs.png" alt="vue logo">
            <img src="../assets/react.png" alt="react logo">
            <img src="../assets/git.png" alt="git logo">
          </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
  #intro {
    display: flex;
    flex-direction: column;
    justify-content: center;
    #logos {
      height: 60px;
      display: flex;
      justify-content: center;
      align-items: center;
      gap: 35px;
      img {
        margin-top: 20px;
        margin-bottom: 5px;
        height: 50px;
        transition: 0.7s all;
        border-radius: 50px;
      }
      img:hover {
        transform: scale(1.2);
        background-color: rgba(17, 98, 136, 0.664);
        border-radius: 5px;
      }

      @media only screen and (max-width:748px) {
      img {
        height: 35px;
      }
    }

    @media only screen and (min-width:749px) and (max-width:930px) {
      img {
        height: 40px;
      }
    }
    }
    
  }
</style>