<div class="col-lg-3">
  <img src="profile.jpg" alt="Stephen Sandini" style="border-radius:15%; width:250px;">
  <h5>Software Developer <button class="toggle-btn" onclick="toggleDarkMode()"> 🌙 Dark Mode </button></h5>     
  <a href="https://www.linkedin.com/in/stephen-sandini/" target="_blank"><img src="linkedin.png" style="width:35px; height:35px;"></a>
  <a href="https://github.com/StephenSandini" target="_blank"><img src="git.png" style="width:35px; height:35px;"></a>
</div>
<div class="col-lg-3">
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
