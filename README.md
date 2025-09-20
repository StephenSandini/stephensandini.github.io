<div class="col-lg-3">
  <img src="profile.jpg" alt="Stephen Sandini" style="border-radius:15%; width:250px;">
  <h5>Software Developer <button class="toggle-btn" onclick="toggleDarkMode()"> 🌙 Dark Mode </button></h5>     
  <span class="info">
      <h5>Programming Languages:</h5>
      <ul>  
        <li>C#</li>
        <li>SQL</li>
        <li>JavaScript</li>
        <li>HTML</li>
        <li>Python</li>
        <li>Flutter</li>
      </ul>
    </span>
</div>
<div class="col-lg-3">
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
    padding: 15px 15px;
    border: none;
    border-radius: 10%;
    cursor: pointer;
    color: black;
    font-size: 14px;
    background-color: #ffffff;
    }
  .toggle-btn {
    position: fixed;
    padding: 15px 15px;
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
