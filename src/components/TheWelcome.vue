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
        <p id="title">Hello and welcome to my website.</p>
        <p>I'm Milan, a developer from Belgrade, Serbia.
        I'm 26 years old economist who fell in love with coding.
        I enjoy to develop websites, components and applications. I would also like to get into game development one day.</p>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
  * {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
  }

  #cover {
    width: 100%;
    #myVideo {
      position: relative;
      top: 90px;
      width: 100%;
    }
    #content {
      position: absolute;
      top: 20%;
      left: 15%;
      background: rgba(0, 0, 0, 0.5);
      color: #f1f1f1;
      width: 70%;
      padding: 20px;
      display: flex;
      #photo {
        width: 30%;
        img {
          width: 80%;
        }
      }
      #intro {
        width: 70%;
        display: flex;
        flex-direction: column;
        justify-content: center;
        text-align: center;
        align-items: center;
        #title {
          font-size: 24px;
          margin-bottom: 20px;
          letter-spacing: 4px;
          color: #f1f1f1;
          font-weight: 700;
        }
        p {
          font-size: 16px;
          letter-spacing: 3px;
          line-height: 25px;
        }

        @media only screen and (max-width:748px) {
        #title {
          font-size: 16px;
        }
        p {
          font-size: 10px;
          line-height: 10px;
        }
      }

        @media only screen and (min-width:749px) and (max-width:930px) {
        #title {
          font-size: 20px;
        }
        p {
          font-size: 12px;
          line-height: 20px;
        }
      }
      }


      @media only screen and (max-width:748px) {
        #intro {
          width: 90%;
        }
      }

      @media only screen and (min-width:749px) and (max-width:930px) {
        #intro {
          width: 80%;
        }
      }
    }



    @media only screen and (max-width:748px) {
        #content {
          width: 90%;
          left: 5%;
        }
      }

    @media only screen and (min-width:749px) and (max-width:930px) {
        #content {
          width: 80%;
          left: 10%;
        }
      }
  }

  
</style>