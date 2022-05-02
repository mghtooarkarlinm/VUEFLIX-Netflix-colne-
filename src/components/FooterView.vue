<template>
  <footer>
      <p>Questions? Call +959 7933 844 82</p>
      <div class="tags">
          <div class="tag">
              <li>FAQ</li>
              <li>Investor Relations</li>
              <li>Privacy</li>
              <li>Speed Test</li>
          </div>
          <div class="tag">
              <li>Help Centre</li>
              <li>Jobs</li>
              <li>Cookie Preferences</li>
              <li>Legal Notices</li>
          </div>
          <div class="tag">
              <li>Account</li>
              <li>Ways to Watch</li>
              <li>Corporate Informatio</li>
              <li>Only on Netflix</li>
          </div>
          <div class="tag">
              <li>Media Centre</li>
              <li>Terms of Use</li>
              <li>Contact Us</li>
          </div>
      </div>

      <div class="lang">
        <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 20 20" fill="currentColor">
            <path fill-rule="evenodd" d="M4.083 9h1.946c.089-1.546.383-2.97.837-4.118A6.004 6.004 0 004.083 9zM10 2a8 8 0 100 16 8 8 0 000-16zm0 2c-.076 0-.232.032-.465.262-.238.234-.497.623-.737 1.182-.389.907-.673 2.142-.766 3.556h3.936c-.093-1.414-.377-2.649-.766-3.556-.24-.56-.5-.948-.737-1.182C10.232 4.032 10.076 4 10 4zm3.971 5c-.089-1.546-.383-2.97-.837-4.118A6.004 6.004 0 0115.917 9h-1.946zm-2.003 2H8.032c.093 1.414.377 2.649.766 3.556.24.56.5.948.737 1.182.233.23.389.262.465.262.076 0 .232-.032.465-.262.238-.234.498-.623.737-1.182.389-.907.673-2.142.766-3.556zm1.166 4.118c.454-1.147.748-2.572.837-4.118h1.946a6.004 6.004 0 01-2.783 4.118zm-6.268 0C6.412 13.97 6.118 12.546 6.03 11H4.083a6.004 6.004 0 002.783 4.118z" clip-rule="evenodd" />
            </svg>
        <select>
            <option value="">English</option>
            <option value="">Chinese</option>
        </select>
      </div>

      <p class="last">VUEFLIX MM</p>
  </footer>
</template>

<script>
export default {

}
</script>

<style scoped>
footer{
    padding: 60px 180px;
    background-color: #000;
    color: #999;
}
.tags{
    display: flex;
    align-items: center flex-start;
    justify-content: center flex-start;
}
.tag{
    margin: 20px 50px;
}
.tag li{
    list-style: none;
    margin: 18px 0;
    font-size: 14px;
    cursor: pointer;
    transition: all .2s;
}
.tag li:hover{
    text-decoration: underline;
}
p{
    margin-left: 47px;
}
.last{
    margin-top: 40px;
    font-size: 14px;
    margin-left: 51px;
}
.lang{
    position: relative;
    display: inline;
    cursor: pointer;
    margin-left: 50px;
}
.lang select{
    background: transparent;
    color: #999;
    appearance: none;
    padding: 12px 26px 12px 30px;
    font-size: 18px;
    cursor: pointer;
    border: 2px solid #999;
}
.lang::after{
    content: '';
    border-width: 8px;
    border-style: solid;
    border-color: transparent;
    border-top-color: #999;
    display: inline-block;
    position: absolute;
    border-radius: 2px;
    top: 38%;
    right: 4%;
    margin-right: 4px;
}
.lang svg{
    position: absolute;
    top: -1px;
    width: 22px;
    margin-left: 6px;
}
@media screen and (max-width: 456px){
    p{
        margin-left: 8px;
    }
    footer{
        padding: 50px 28px;
        background-color: #000;
        color: #999;
    }
    .tags{
        display: block;
    }
    .tag{
        margin: 20px 10px;
    }
    .lang{
        position: relative;
        display: inline;
        cursor: pointer;
        margin-left: 13px;
    }
    .last{
        margin-top: 20px;
        font-size: 14px;
        margin-left: 16px;
    }
}
</style>
