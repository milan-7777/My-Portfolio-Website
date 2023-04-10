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
          <p>+381631067777</p>
          <p>milanstanic7777@gmail.com</p>
          <div id="social">
            <a href="https://github.com/milan-7777" target="_blank">GitHub</a>
            <a href="https://www.linkedin.com/in/milan-stanic-814641255/" target="_blank">LinkedIn</a>
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
    #social {
      width: 80%;
      margin-top: 40px;
      display: flex;
      flex-direction: row;
      justify-content: center;
      gap: 20%;
        a {
          width: 50%;
          text-decoration: none;
          letter-spacing: 3px;
          line-height: 30px;
          color: rgb(17, 98, 136);
          transition: 0.5s all;
          font-size: 20px;
          font-weight: 700;
          padding: 15px 35px;
          border: 3px solid rgb(17, 98, 136);
          border-radius: 15px; 
        }
        a:hover {
          transform: scale(1.1);
          color: rgb(17, 128, 136);
          border: 3px solid rgb(17, 128, 136);
        }
        @media only screen and (max-width:748px) {
          a {
            font-size: 12px;
            line-height: 20px;
          }
        }

        @media only screen and (min-width:749px) and (max-width:930px) {
          a {
            font-size: 16px;
          }
        }
        }
  }
  
</style>