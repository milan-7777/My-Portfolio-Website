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
          <p class="title">Agency Nova Vizija</p>
          <p>2022 - ongoing (part time)</p>
          <p>Coding UI components, layouts and features with
            HTML, CSS and Javascript, testing workflows
            manually, editing text and multimedia content. Projects:
         </p>
         <div id="projects">
            <a href="https://centar-pharm.com/" target="_blank">Web shop Centar pharm</a>
            <a href="https://novavizija.org/" target="_blank">Nova Vizija consulting agency</a>
            <a href="https://metalpro-derventa.com/" target="_blank">MetalPro d.o.o.</a>
        </div>
         <p>Currently working on several new projects, websites, web shops and business applications.</p>
        </div>
      </div>
    </div>
  
  </template>

<style lang="scss" scoped>
  #intro {
    display: flex;
    flex-direction: column;
    justify-content: center;
    a {
        text-decoration: none;
        font-size: 22px;
        letter-spacing: 3px;
        line-height: 25px;
        color: rgb(17, 98, 136);
        transition: 0.4s all;
        font-size: 24px;
        margin-bottom: 5px;
    }
    a:hover {
        transform: scale(1.1);
        color: rgb(17, 128, 136);
    }
  }
  .title {
    color: rgb(17, 98, 136);
    margin-bottom: 5px;
  }
  #projects {
    display: flex;
    a {
        font-size: 18px;        
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
  
</style>