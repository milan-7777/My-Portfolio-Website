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
          <a href="https://code.edu.rs/" target="_blank">IT Course – Code by Comtrade 2022 - 2023</a>
          <p>Frontend Development</p>
          <br>
          <a href="https://www.bpa.edu.rs/en-us" target="_blank">Belgrade business school 2015 - 2018</a>
          <p>Finances, accounting and banking</p>
          <p>Bachelor of Applied Studies in Economics</p>
        </div>
      </div>
    </div>
  
  </template>

<style lang="scss" scoped>
  #intro {
    display: flex;
    flex-direction: column;
    justify-content: center;
  }
  a {
    text-decoration: none;
    font-size: 22px;
    letter-spacing: 3px;
    line-height: 30px;
    color: rgb(17, 98, 136);
    transition: 0.4s all;
    font-size: 24px;
    margin-bottom: 5px;
  }

    @media only screen and (max-width:748px) {
      a {
        font-size: 14px;
        line-height: 20px;
      }
    }

    @media only screen and (min-width:749px) and (max-width:930px) {
      a {
        font-size: 20px;
      }
    }
  a:hover {
    transform: scale(1.1);
    color: rgb(17, 128, 136);
  }
</style>