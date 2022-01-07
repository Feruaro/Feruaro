<head>
    <style>
       @mixin center {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
//Completely customizable
//--
$font-size: 40px;
$letter-spacing: 0.0625em; //This counts for 1px on 16px font;
$letter-count: 20; //Number of letters in text !important
$transition-time: 3s; //Typing speed
$bg-color: #eff5ed;
$mask-color: #eff5ed; //Change it to see how this works :)
$font-color: #152860;

$letter-size: calc(1ch + #{$letter-spacing});
$cursor-width: 1px; //Change this to $letter-size if you want Insert:active effect
//--
$cursor-blink-duration: $letter-count;
$font-width: calc(#{$letter-count}ch + #{$letter-count}*#{$letter-spacing});

*, *:after, *:before {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

body {
  background: #eff5ed;
  font-family: courier, serif; //Need monospace font for this to work
  text-align: center;
    -webkit-font-smoothing: antialiased;
}

.hello {
  @include center;
  top: 25%;

  h3 {
    position: relative;
      color: $font-color;
      text-align: center;
      white-space: nowrap;
    font-size: $font-size;
    letter-spacing: $letter-spacing;
    width: $font-width;

      &:after {
      display: block;
      position: absolute;
      content: '';
      width: $font-width;
      height: 2ex;
      left: 0;
      top: 0;
      background: $mask-color;
      animation: .6s blink $cursor-blink-duration, move $transition-time 1.5s forwards steps(1);
      border-left: $cursor-width solid $font-color;
      box-shadow: 0px 1ex 0px 0px $mask-color;

      @keyframes move {
        @for $i from 1 through $letter-count {
          $temp: 100/$letter-count;
          $percent: $i*$temp;
          #{$percent}% {
            width: calc(#{$font-width} - (#{$i}ch + #{$i}*#{$letter-spacing}));
            left: calc(#{$i}ch + #{$i}*#{$letter-spacing});
          }
        }
      }

      @keyframes blink {
        0% {
            border-left-color: $font-color;
        }
        50% {
            border-left-color: $font-color;
        }
        51% {
            border-left-color: $mask-color;
        }
        100% {
            border-left-color: $mask-color;
        }
      }
      }
  }
}   
    </style>
</head>
<body>
<img align="right" height="270em" src="https://github.com/Feruaro/Feruaro/blob/main/1.png"/>

<div class="hello">
    <H1> Hi there, I'm Fernanda Ruaro 🤝</H1>
</div>
  
<H4> 📚 A student of Software Engineer and Data Science </H4>
<H4> ❤ Passionate about everything that involves technology </H4>
<H4> ☁ If you can dream it, you can do it! </H4>  
<br><br>

  ##

<div align="center"><br>
    <img height="150em" src="https://github-readme-stats.vercel.app/api?username=Feruaro&show_icons=true&theme=dracula&include_all_commits=true&count_private=true"/>
    <img height="150em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Feruaro&layout=compact&langs_count=7&theme=dracula"/>
</div>

<div align="center" style="display: inline_block"><br>
    <img alt="Fe-Java" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/java/java-original.svg" />
    <img alt="Fe-C" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/c/c-original.svg" />
    <img alt="Fe-C++" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/cplusplus/cplusplus-original.svg" />
    <img alt="Fe-PHP" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/php/php-original.svg" />
    <img alt="Fe-HTML" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg" />
    <img alt="Fe-Spring" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/spring/spring-original-wordmark.svg" />
    <img alt="Fe-Linux" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/linux/linux-original.svg" />  
</div>

  ##


<div align="center"><br> 
    <a href="https://www.linkedin.com/in/fernanda-ruaro/" target="_blank"><img src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank"></a> 
    <a href="https://www.instagram.com/ruarofe/" target="_blank"><img src="https://img.shields.io/badge/-Instagram-%23E4405F?style=for-the-badge&logo=instagram&logoColor=white" target="_blank"></a>
    <a href = "mailto:feayres26@gmail.com"><img src="https://img.shields.io/badge/-Gmail-%23333?style=for-the-badge&logo=gmail&logoColor=white" target="_blank"></a> 
 
 ![Snake animation](https://github.com/Feruaro/Feruaro/blob/output/github-contribution-grid-snake.svg)
 
</div>

  ##
  
<div align="center"><br>
  <p align="center"> Thank you and come again!👋 </p>  
  <p> <img align="center" src="https://profile-counter.glitch.me/Feruaro/count.svg" /></p>
</div>
</body>

