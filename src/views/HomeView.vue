<template>
  <div class="home">
    <div class="filter"></div>
    <header>
      <div class="nav">
        <div class="logo">
          <h1>VUEFLIX</h1>
        </div>
        <div class="lang-sign">
          <div class="lang">
              <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 20 20" fill="currentColor">
                <path fill-rule="evenodd" d="M4.083 9h1.946c.089-1.546.383-2.97.837-4.118A6.004 6.004 0 004.083 9zM10 2a8 8 0 100 16 8 8 0 000-16zm0 2c-.076 0-.232.032-.465.262-.238.234-.497.623-.737 1.182-.389.907-.673 2.142-.766 3.556h3.936c-.093-1.414-.377-2.649-.766-3.556-.24-.56-.5-.948-.737-1.182C10.232 4.032 10.076 4 10 4zm3.971 5c-.089-1.546-.383-2.97-.837-4.118A6.004 6.004 0 0115.917 9h-1.946zm-2.003 2H8.032c.093 1.414.377 2.649.766 3.556.24.56.5.948.737 1.182.233.23.389.262.465.262.076 0 .232-.032.465-.262.238-.234.498-.623.737-1.182.389-.907.673-2.142.766-3.556zm1.166 4.118c.454-1.147.748-2.572.837-4.118h1.946a6.004 6.004 0 01-2.783 4.118zm-6.268 0C6.412 13.97 6.118 12.546 6.03 11H4.083a6.004 6.004 0 002.783 4.118z" clip-rule="evenodd" />
              </svg>
            <span>English</span>
            <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 20 20" fill="currentColor">
              <path fill-rule="evenodd" d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z" clip-rule="evenodd" />
            </svg>
          </div>
          <div class="sign">
            <span>Sign In</span>
          </div>
        </div>
      </div>
    </header>
    <main>
        <div class="main-content">
          <span class="main-txt">Unlimited films, TV<br>programmes and more.</span>
          <p class="sec-txt">Watch anywhere. Cancel at any time.</p>
          <p class="last-txt">Ready to watch? Enter your email to create or restart your membership.</p>
          <form>
              <input type="text" placeholder="What are you looking for ?">
              <button>
                <span>Get Start</span>
                <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 20 20" fill="currentColor">
                  <path fill-rule="evenodd" d="M7.293 14.707a1 1 0 010-1.414L10.586 10 7.293 6.707a1 1 0 011.414-1.414l4 4a1 1 0 010 1.414l-4 4a1 1 0 01-1.414 0z" clip-rule="evenodd" />
                </svg>
              </button>
          </form>
        </div>
    </main>
    <footer></footer>
  </div>
</template>

<script>
// @ is an alias to /src

export default {

}
</script>

<style scoped>
.home{
  width: 100%;
  height: 100vh;
  background-image: url('../assets/main-bg.jpg');
  background-position: center;
  background-size: cover;
  position: relative;
  z-index: 1;
}
.filter{
  position: absolute;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0 , .5);
  z-index: 2;
}
header,footer{
  z-index: 3;
  position: relative;
}
.nav,.lang-sign{
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.nav{
  padding: 20px 46px;
}
.logo h1{
  color: hsl(357, 92%, 47%);
  font-size: 40px;
}
.lang{
  background: #000;
  color: #fff;
  border: 1px solid #fff;
  border-radius: 4px;
  padding: 8px 6px;
  display: flex;
  align-items: center;
  justify-content: center;
  cursor: pointer;
}
.sign{
  background: #e30813 ;
  color: #fff;
  padding: 8px 15px;
  font-size: 15px;
  font-weight: 500;
  margin-left: 32px;
  border-radius: 4px;
  cursor: pointer;
}
.lang svg{
  width: 20px;
  color: #fff;
  margin-right: 2px;
}
main{
  z-index: 3;
  position: relative;
  color: #fff;
  text-align: center;
}
.main-content{
  margin-top: 11%;
}
.main-txt{
  font-size: 50px;
  font-weight: 600;
}
.sec-txt{
  margin: 8px 0 32px 0;
  font-size: 26px;
  font-weight: 500;
}
.last-txt{
  font-size: 19px;
  margin-bottom: 20px;
}
main form{
  display: flex;
  align-items: center;
  justify-content: center;
  flex-wrap: wrap;
}
main form input{
  width: 500px;
  font-size: 18px;
  padding: 18px 8px;
}
main form input:focus{
  outline: none;
}
main form button{
  width: 180px;
  display: flex;
  align-items: center;
  justify-content: center;
  outline: none;
  border: none;
  font-size: 28px;
  color: #fff;
  background: #e30813;
  line-height: 60px;
  cursor: pointer;
}
main form button svg{
  width: 30px;
}
@media screen and (max-width: 456px){ 
  .nav{
    padding: 16px 22px;
  }
  .logo h1{
    font-size: 20px;
  }
  .filter{
    background: rgba(0, 0, 0, .7);
  } 
  .lang{
    font-size: 12px;
    padding: 2px 3px;
  }
  .sign{
    padding: 4px 8px;
    font-size: 12px;
    margin-left: 10px;
  }
  .main-content{
    margin-top: 11%;
  }
  .main-txt{
    font-size: 25px;
    font-weight: 600;
  }
  .sec-txt{
    margin: 8px 0 32px 0;
    font-size: 16px;
    font-weight: 500;
  }
  .last-txt{
    font-size: 20px;
    margin-bottom: 20px;
  }
  main form input{
    display: block;
    width: 80%;
    padding: 10px 8px;
  }
  main form button{
    margin-top: 16px;
    width: 140px;
    font-size: 16px;
    line-height: 40px;
  }
}
</style>
