

  <nav>
    <div class="settings">
       <button class="toggle-btn" onclick="toggleDarkMode()"> 🌙 Dark Mode </button>
       <button onclick="zoomIn()">🔍+</button>
       <button onclick="zoomOut()">🔍-</button>
    </div>
  </nav>
<div class="container">
  <section class="col-lg-3 left">
    <img src="profile.jpg" alt="Stephen Sandini" style="border-radius:15%; width:250px;">
    <h5>Software Developer</h5>     
    <a href="https://www.linkedin.com/in/stephen-sandini/" target="_blank"><img src="linkedin.png" style="width:35px; height:35px; border-radius:15%;"></a>
    <a href="https://github.com/StephenSandini" target="_blank"><img src="git.png" style="width:35px; height:35px; border-radius:15%;"></a>
     <span class="info">
      <h5>Programming Languages:</h5>
        <ul>  
          <li>C#</li>
          <li>JavaScript</li>
          <li>Flutter</li>
          <li>Python</li>
          <li>HTML</li>
          <li>SQL</li>
          <li>PL/SQL</li>
        </ul>
      </span>
  </section>
  <section class="right">
    <h2>About Me</h2>
    <p>I am a software developer with experience in building practical appplications and solving real-world problems through code.  Currently, I am pursuing my master's degree in software engineering, where I am expanding my knowledge of advanced development practices, system design, and emerging technologies. My goal is to contribute to innovative projects that combine creativity and technology while continuously growing as a professional.</p>
    <h2>Areas of Interest</h2>
    <ul>
      <li>🌐 Web Development
        <ul>
          <li>building responsive, accessible, and scalable web applications</li>
        </ul> 
      </li>
      <li>📱 Mobile App Development
        <ul>
          <li>creating user-friendly, efficient applications for Android and iOS</li>
        </ul>
      </li>
      <li>🧠 Artifical Intelligence
        <ul>
          <li>exploring machine learning and AI-driven problem solving</li>
        </ul>
      </li>
      <li>🎮 Game Development
        <ul>
          <li>designing and programming engaging interactive experiences</li>
        </ul>
      </li>
      <li>🥽 Virtual Reality (VR)
        <ul>
          <li>developing immersive applciations that blend the digital and physical worlds</li>
        </ul>
      </li>
    </ul>
  </section>
</div>
<style>
  body {
    transition: background-color 0.3s, color 0.3s;
    background-color: #ffffff;
    color: black;
  }
  body.dark-mode {
    background-color: #121212;
    color: white;
  }
  body.dark-mode .toggle-btn {
    position: fixed;
    padding: 0px 15px;
    border: none;
    border-radius: 10%;
    cursor: pointer;
    color: black;
    font-size: 14px;
    background-color: #ffffff;
    }
  .toggle-btn {
    position: fixed;
    padding: 0px 15px;
    border: none;
    border-radius: 10%;
    cursor: pointer;
    color: white;
    font-size: 14px;
    background-color: #121212;
  }
  .container {
    display: flex;
    gap: 20px;
    padding: 20px;
  }
  .left {
    flex: 1;
    padding: 15px;
  }
  .right {
    flex: 2;
    padding: 15px;
  }
  .settings {
    display: flex;
    gap: 8px;
  }
  .settings button {
    background: #444;
    color: white;
    border: none;
    padding: 0px 15px;
    border-radius: 4px;
    cursor: pointer;
    font-size: 14px;
    transition: background 0.3s;
  }
  .settings button:hover {
    background: #00bcd4;
  }
  nav {
    background-color: #222;
    padding: 10px;
    position: sticky;
    top: 0;
    z-index: 999;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  nav ul  {
    list-style: none;
    margin: 0;
    padding: 0;
    display: flex;
  }
  nav li {
    margin-left: 20px;
  }
  nav a {
    text-decoration: none;
    color: white;
    font-weight: bold;
    transition: color 0.3s;
  }
  nav a:hover {
    color: #00bcd4;
  }
</style>
<script>
  let scaleLevel = 1;  
  function toggleDarkMode() {
    document.body.classList.toggle("dark-mode");
    const btn = document.querySelector(".toggle-btn");
    if(document.body.classList.contains("dark-mode")) {
      btn.textContent = "☀️ Light Mode";
    } else {
      btn.textContent = "🌙 Dark Mode";
    }
  }
 function zoomOut() {
   scaleLevel = Math.max(0.5, scaleLevel - 0.1);
   document.body.style.transform = `scale(${scaleLevel})`;
   document.body.style.transformOrigin = "top left";
 }
  function zoomIn() {
    scaleLevel += 0.1;
    document.body.style.transform = `scale(${scaleLevel})`;
    document.body.style.transform = "top left";
  }
</script>
