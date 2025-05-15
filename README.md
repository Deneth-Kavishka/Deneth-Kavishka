<canvas id="matrixCanvas" style="display:block; position:absolute; z-index:-1;"></canvas>
<script>
  var c = document.getElementById("matrixCanvas");
  var ctx = c.getContext("2d");

  // Making the canvas full screen
  c.height = window.innerHeight;
  c.width = window.innerWidth;

  // Characters - taken from the original Matrix movie
  var matrix = "ABCDEFGHIJKLMNOPQRSTUVWXYZ123456789@#$%^&*()*&^%";
  // Converting the string into an array of single characters
  matrix = matrix.split("");

  var font_size = 10;
  var columns = c.width / font_size; // Number of columns for the rain
  // An array of drops - one per column
  var drops = [];
  // X below is the x coordinate
  // 1 = y-coordinate of the drop(same for every drop initially)
  for (var x = 0; x < columns; x++)
    drops[x] = 1;

  // Drawing the characters
  function draw() {
    // Black BG for the canvas
    // Translucent BG to show trail
    ctx.fillStyle = "rgba(0, 0, 0, 0.04)";
    ctx.fillRect(0, 0, c.width, c.height);

    ctx.fillStyle = "#0F0"; // Green text
    ctx.font = font_size + "px arial";
    // Looping over drops
    for (var i = 0; i < drops.length; i++) {
      // A random character
      var text = matrix[Math.floor(Math.random() * matrix.length)];
      // x = i*font_size, y = value of drops[i]*font_size
      ctx.fillText(text, i * font_size, drops[i] * font_size);

      // Sending the drop back to the top randomly after it has crossed the screen
      // Adding a randomness to the reset to make the drops scattered on the Y axis
      if (drops[i] * font_size > c.height && Math.random() > 0.975)
        drops[i] = 0;

      // Incrementing Y coordinate
      drops[i]++;
    }
  }

  setInterval(draw, 35);
</script>



  <!-- Typing animation for name -->
<div align="center" style="background: linear-gradient(to right, #0e75b6, #2a9df4); padding: 30px; border-radius: 15px;">
  <h1 align="center" style="color: white;">
    <span align="center">
      <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=30&duration=3000&pause=500&color=FFFFFF&center=true&vCenter=true&width=735&lines=👋Hey!+I'm+Deneth+Kavishka" alt="👋Hey! I'm Deneth Kavishka">
      <p align="center">
        <img src="https://readme-typing-svg.herokuapp.com?font=Orbitron&size=14&duration=3000&pause=500&color=00FFFF&center=true&vCenter=true&width=800&lines=COLLABORATING+TO+CREATE+WHAT+MATTERS..." alt="COLLABORATING TO CREATE WHAT MATTERS..." />
      </p>
    </span>
  </h1>

  <!-- Hacker Animation with Hoodie from LottieFiles -->
  <div style="margin: 20px 0;">
    <iframe src="https://lottie.host/embed/8cc98a92-7b95-4ebc-8899-62197400555d/1VJjE0kKYt.json" 
            style="width: 300px; height: 300px; border: none; background: transparent;" 
            allowfullscreen>
    </iframe>
  </div>

  <h3 style="color: Grey;">A passionate coding enthusiast, always eager to research, find, learn and develop across the full stack.</h3>
</div>




<p align="center" style="margin-top: 15px;">
  <a href="https://github.com/deneth-kavishka">
    <img src="https://komarev.com/ghpvc/?username=deneth-kavishka&label=Profile%20Views&color=0e75b6&style=flat" alt="Deneth-Kavishka" />
  </a><br/>
  <!--strong><a href="https://github.com/deneth-kavishka">Deneth-Kavishka</a></strong-->
</p>

---

### 📊 GitHub Stats:

<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=deneth-kavishka&theme=radical" alt="GitHub streak stats" style="border-radius: 15px; box-shadow: 0px 4px 15px rgba(0, 0, 0, 0.5);" />
  <img src="https://github-readme-stats.vercel.app/api?username=deneth-kavishka&show_icons=true&locale=en&theme=radical" alt="GitHub stats" style="border-radius: 15px; box-shadow: 0px 4px 15px rgba(0, 0, 0, 0.5);" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=deneth-kavishka&layout=compact&theme=radical" alt="Most Used Languages" style="border-radius: 15px; box-shadow: 0px 4px 15px rgba(0, 0, 0, 0.5);" />
</p>

---

### 🌐 Connect with Me:
<p align="left">
<a href="https://www.linkedin.com/in/deneth-kavishka-338288284/" target="_blank">
  <img src="https://skillicons.dev/icons?i=linkedin" alt="LinkedIn" width="28" height="28" style="border-radius: 15px; padding: 5px; background: linear-gradient(145deg, #1c1c1c, #242424); box-shadow: 5px 5px 10px #1a1a1a, -5px -5px 10px #2e2e2e;" />
</a> 
<a href="https://x.com/Deneth_Kavish" target="_blank">
  <img src="https://skillicons.dev/icons?i=twitter" alt="Twitter" width="28" height="28" style="border-radius: 15px; padding: 5px; background: linear-gradient(145deg, #1c1c1c, #242424); box-shadow: 5px 5px 10px #1a1a1a, -5px -5px 10px #2e2e2e;" />
</a>

</p>
  <!--<a href="https://youtube.com/@virajwathsalag" target="_blank">
    <img src="https://skillicons.dev/icons?i=youtube" alt="YouTube" style="border-radius: 10px; padding: 5px; background: linear-gradient(145deg, #1c1c1c, #242424); box-shadow: 5px 5px 10px #1a1a1a, -5px -5px 10px #2e2e2e;" /> -->
  </a>
</p>

---

### 🛠️ Languages and Tools:
<p align="center">
  <img src="https://skillicons.dev/icons?i=vscode,visualstudio,github,git,cs,c,dotnet,html,css,javascript,bootstrap,tailwind,nodejs,react,typescript,express,java,python,laravel,arduino,mysql,mongodb,postgres" alt="Skills" style="margin: 5px; border-radius: 15px; box-shadow: 0 4px 15px rgba(0, 0, 0, 0.5);" />
  
 <!-- <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/spring/spring-original.svg" alt="Spring Boot" width="30" height="30" style="margin: 5px; border-radius: 15px; box-shadow: 0 4px 15px rgba(0, 0, 0, 0.5);" />
  
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/oracle/oracle-original.svg" alt="Oracle DB" width="30" height="30" style="margin: 5px; border-radius: 15px; box-shadow: 0 4px 15px rgba(0, 0, 0, 0.5);" />
-->
</p>


---

### 🔥 Highlights:

- 🌱 Constantly learning and improving.
- 👯 I’m looking to collaborate on web projects.
- 💻 Skilled in full-stack development, focusing on modern web, mobile app and desktop applications.
- 🚀 Passionate about creating optimized and user-friendly mobile app & software.


<!--
**Deneth-Kavishka/Deneth-Kavishka** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
