<template>
  <header>
    <div id="logo">
      <router-link to="/">
        <h1>{ Milan Stanic }</h1>
        <p>Frontend Developer</p>
      </router-link>
      
    </div>
    <div id="header">
      <nav>
        <ul>
          <li><router-link to="/tech">TECH. SKILLS</router-link></li>
          <li><router-link to="/education">EDUCATION</router-link></li>
          <li><router-link to="/experience">EXPERIENCE</router-link></li>
          <li><router-link to="/about">ABOUT ME</router-link></li>
          <li><router-link to="/contact">CONTACT</router-link></li>
        </ul>
      </nav>
    </div>
  </header>

  <RouterView />

  <footer>
    <div id="footer">
      <p>Milan Stanic 2023</p>
    </div>
  </footer>
</template>

<script setup>
</script>


<style lang="scss">
  * {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
    font-family: 'Lato', sans-serif;
  }

  header {
    position: fixed;
    width: 100%;
    height: 90px;
    display: flex;
    z-index: 9;
    #logo {
      height: 100%;
      width: 35%;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      background-color: rgb(2, 25, 44);
      text-align: center;
      a {
        text-decoration: none;
        padding: 5px;
      }
      h1 {
        font-size: 28px;
        letter-spacing: 3px;
        color: rgb(17, 98, 136);
        transition: 0.5s all;
      }
      h1:hover {
          cursor: pointer;
          color: rgb(17, 128, 136);
      }
      p {
        font-size: 14px;
        color: rgb(17, 98, 136);
        transition: 0.4s all;
      }
      p:hover {
        cursor: pointer;
        color: rgb(17, 128, 136);
      }

      @media only screen and (max-width:748px) {
        h1 {
          font-size: 16px;
        }
        p {
          font-size: 10px;
        }
      }

      @media only screen and (min-width:749px) and (max-width:930px) {
        h1 {
          font-size: 20px;
        }
        p {
          font-size: 12px;
        }
      }
    }
    

    #header {
      width: 100%;
      background-color: rgb(2, 25, 44);
      height: 90px;
      display: flex;
      align-items: center;
      nav {
        width: 90%;
      }
      nav ul {
        align-items: center;
        display: grid;
        grid-template-columns: repeat(5, 1fr);
        list-style: none;
        li a {
          width: 100%;
          display: flex;
          justify-content: center;
          list-style: none;
          text-decoration: none;
          color: #fff;
          font-size: 14px;
          letter-spacing: 3px;
          padding: 20px 0px;
          text-align: center;
          transition: 0.5s all;
          }
          li a:hover {
            background-color: rgba(17, 128, 136, 0.466);
            border-radius: 25px;
          }
        }

      @media only screen and (max-width:748px) {
        nav {
          width: 100%;
        }
        nav ul li a {
          font-size: 8px;
        }
      }

      @media only screen and (min-width:749px) and (max-width:930px) {
        nav {
          width: 100%;
        }
        nav ul li a {
          font-size: 10px;
        }
      }     
    }
  }


  footer {
    width: 100%;
    height: 90px;
    display: flex;
    z-index: 9;
    background-color: rgb(2, 25, 44);
    #footer {
      position: relative;
      width: 100%;
      display: flex;
      align-items: center;
      justify-content: center;
      background-color: rgb(2, 25, 44);
      p {
        font-size: 14px;
        text-align: center;
        color: #fff;
        color: rgb(17, 98, 136);
        letter-spacing: 3px;
      }
    }
  }
</style>
