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
            <div id="about">
                <p>Hello, I'm Milan, I'm a developer from Belgrade, Serbia.
                    I'm 26 years old economist who fell in love with coding.
                    I enjoy to develop websites, components and applications.
                    I would also like to get into game development one day.
                </p>
            </div>
            
            <p>I like to play sports. I love to travel.
                I'm passionate about motorcycles and
                MotoGP races. I love reading books and
                watching mystery movies.
            </p>
        </div>
      </div>
    </div>
  
  </template>

<style lang="scss" scoped>
  #intro {
    display: flex;
    flex-direction: column;
    justify-content: center;
    p {
          font-size: 16px;
          letter-spacing: 3px;
          line-height: 35px;
        }
  }
  a {
    text-decoration: none;
    font-size: 22px;
    letter-spacing: 3px;
    line-height: 35px;
    color: rgb(17, 98, 136);
    transition: 0.4s all;
    font-size: 24px;
  }
  a:hover {
    transform: scale(1.1);
    color: rgb(17, 128, 136);
  }
</style>