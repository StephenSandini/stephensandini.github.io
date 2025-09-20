<div class="container">
  <div class="col-lg-3 left">
    <img src="profile.jpg" alt="Stephen Sandini" style="border-radius:15%; width:250px;">
    <h5>Software Developer <button class="toggle-btn" onclick="toggleDarkMode()"> 🌙 Dark Mode </button></h5>     
    <a href="https://www.linkedin.com/in/stephen-sandini/" target="_blank"><img src="linkedin.png" style="width:35px; height:35px; border-radius:15%;"></a>
    <a href="https://github.com/StephenSandini" target="_blank"><img src="git.png" style="width:35px; height:35px; border-radius:15%;"></a>
  </div>
  <div class="col-lg-3 left">
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
  </div>
  <div class="right">
    <h4>Bio:</h4>
    <p>Lorem ipsum</p>
    <h4>Additional Header?</h4>
    <p>Lorem ipsum</p>
  </div>
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
</style>
<script>
  function toggleDarkMode() {
    document.body.classList.toggle("dark-mode");
    const btn = document.querySelector(".toggle-btn");
    if(document.body.classList.contains("dark-mode")) {
      btn.textContent = "☀️ Light Mode";
    } else {
      btn.textContent = "🌙 Dark Mode";
    }
  }
</script>
