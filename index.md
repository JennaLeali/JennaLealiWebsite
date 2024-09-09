<!-- Navigation Bar -->
<div style="position: fixed; top: 0; left: 0; right: 0; background-color: #6A5ACD; padding: 15px 0; box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1); z-index: 999;">
  <div style="display: flex; justify-content: center; gap: 20px;">
    <a href="#home" style="color: white; font-size: 18px; text-decoration: none; padding: 10px;">Home</a>
    <a href="#projects" style="color: white; font-size: 18px; text-decoration: none; padding: 10px;">Projects</a>
    <a href="#education" style="color: white; font-size: 18px; text-decoration: none; padding: 10px;">Education</a>
    <a href="#resume" style="color: white; font-size: 18px; text-decoration: none; padding: 10px;">Resume</a>
    <a href="#fun-facts" style="color: white; font-size: 18px; text-decoration: none; padding: 10px;">Fun Facts</a>
    <a href="#contact" style="color: white; font-size: 18px; text-decoration: none; padding: 10px;">Contact</a>
  </div>
</div>



<!-- Compressed Home Section with Rearranged Layout -->
<div id="home" style="display: flex; flex-direction: column; align-items: center; justify-content: center; background: linear-gradient(135deg, #6A5ACD, #1E90FF); padding: 40px; border-radius: 15px; min-height: 80vh; margin-top: 80px;"> 

  <!-- Row containing image and name -->
  <div style="display: flex; align-items: center; gap: 30px; margin-bottom: 30px;">
    <img src="assets/images/jenna.png" alt="Jenna Leali" style="max-width: 150px; border-radius: 10%; transition: transform 0.3s ease-in-out, box-shadow 0.3s ease-in-out;">
    
    <h1 style="font-family: 'Comic Sans MS', cursive, sans-serif; color: white; font-size: 45px; text-align: center;">
      Jenna Leali
    </h1>
  </div>

  <!-- Typing animation directly below name -->
  <div class="typing-animation" style="font-size: 20px; color: white; text-align: center; margin-bottom: 20px;">
    <span id="typed-text"></span>
    <span class="cursor">|</span>
  </div>

  <!-- Button under typing text -->
  <a href="https://github.com/JennaLeali" style="font-size: 18px; background-color: #FF69B4; color: white; padding: 10px 15px; border-radius: 5px; text-decoration: none; margin-bottom: 20px;">
    View project on GitHub
  </a>

  <!-- Project Cards Section arranged horizontally -->
  <div style="display: flex; justify-content: center; gap: 10px; margin-top: 30px; width: 90%;">
    <!-- Project 1 -->
    <div class="project-card" style="background-color: white; border-radius: 10px; padding: 15px; width: 180px; box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1); text-align: center; transition: transform 0.3s, box-shadow 0.3s;">
      <h3 style="font-family: 'Comic Sans MS', sans-serif; font-size: 20px;">Project 1</h3>
      <p style="font-size: 14px;">Data analysis on customer behavior patterns.</p>
    </div>

    <!-- Project 2 -->
    <div class="project-card" style="background-color: white; border-radius: 10px; padding: 15px; width: 180px; box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1); text-align: center; transition: transform 0.3s, box-shadow 0.3s;">
      <h3 style="font-family: 'Comic Sans MS', sans-serif; font-size: 20px;">Project 2</h3>
      <p style="font-size: 14px;">Machine learning model predicting stock prices.</p>
    </div>

    <!-- Project 3 -->
    <div class="project-card" style="background-color: white; border-radius: 10px; padding: 15px; width: 180px; box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1); text-align: center; transition: transform 0.3s, box-shadow 0.3s;">
      <h3 style="font-family: 'Comic Sans MS', sans-serif; font-size: 20px;">Project 3</h3>
      <p style="font-size: 14px;">Natural language processing for sentiment analysis.</p>
    </div>
  </div>

  <!-- CSS for Hover Effects -->
  <style>
    .project-card:hover {
      transform: scale(1.05);
      box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
    }
    
    img:hover {
      transform: scale(1.2);
      box-shadow: 0 0 30px #FF69B4;
    }

    /* Typing text animation */
    .typing-animation #typed-text {
      font-family: 'Comic Sans MS', cursive, sans-serif;
      color: white;
      font-size: 20px;
      white-space: nowrap;
      overflow: hidden;
      border-right: 3px solid white;
      width: 0;
      animation: typing 3s steps(40, end), blink-caret 0.75s step-end infinite;
    }

    @keyframes typing {
      from { width: 0; }
      to { width: 100%; }
    }

    @keyframes blink-caret {
      from, to { border-color: transparent; }
      50% { border-color: white; }
    }
  </style>

</div>

<!-- JavaScript for Typing Effect -->
<script>
  document.addEventListener("DOMContentLoaded", function() {
    const typedText = "Showcasing my abilities in data science and analytics through projects and experiences.";
    let i = 0;
    const typingSpeed = 50; // Speed in milliseconds

    function typeWriter() {
      if (i < typedText.length) {
        document.getElementById("typed-text").innerHTML += typedText.charAt(i);
        i++;
        setTimeout(typeWriter, typingSpeed);
      }
    }

    typeWriter();
  });
</script>
---

<!-- Contact Section with Animated Icons and Subtle Background Animation -->
<div id="contact" style="padding: 60px; background: linear-gradient(135deg, #6A5ACD, #1E90FF); border-radius: 15px; background-size: 400% 400%; animation: gradientAnimation 5s ease infinite;">
  <h2 style="font-family: 'Comic Sans MS', cursive, sans-serif; color: white; font-size: 45px; text-align: center; margin-bottom: 40px;">
    Contact Information
  </h2>

  <div style="display: flex; flex-direction: column; align-items: center; gap: 20px;">
    
    <!-- Email with Icon -->
    <div>
      <a href="mailto:jallureleali@gmail.com" style="font-size: 20px; background-color: #FFB6C1; color: white; padding: 15px 30px; border-radius: 5px; text-decoration: none; display: flex; align-items: center; gap: 10px; transition: background-color 0.3s ease, transform 0.3s ease;">
        <img src="assets/icons/email.png" alt="Email Icon" style="width: 35px;"> Click here to email me
      </a>
    </div>

    <!-- LinkedIn with Icon -->
    <div>
      <a href="https://www.linkedin.com/in/jennaleali/" target="_blank" style="font-size: 20px; background-color: #FFB6C1; color: white; padding: 15px 30px; border-radius: 5px; text-decoration: none; display: flex; align-items: center; gap: 10px; transition: background-color 0.3s ease, transform 0.3s ease;">
        <img src="assets/icons/linkedin.png" alt="LinkedIn Icon" style="width: 35px;"> Click here to see my LinkedIn
      </a>
    </div>

    <!-- GitHub with Icon -->
    <div>
      <a href="https://github.com/JennaLeali" target="_blank" style="font-size: 20px; background-color: #FFB6C1; color: white; padding: 15px 30px; border-radius: 5px; text-decoration: none; display: flex; align-items: center; gap: 10px; transition: background-color 0.3s ease, transform 0.3s ease;">
        <img src="assets/icons/github.png" alt="GitHub Icon" style="width: 35px;"> Click here to visit my GitHub
      </a>
    </div>
  
  </div>
</div>

<!-- CSS for Hover Effects and Background Animation -->
<style>
  #contact a:hover {
    background-color: #FFD7D7; /* Slightly lighter pink on hover */
    transform: scale(1.05);
  }

  #contact a img {
    transition: transform 0.3s ease;
  }

  #contact a:hover img {
    transform: rotate(360deg);
  }

  @keyframes gradientAnimation {
    0% {
      background-position: 0% 50%;
    }
    50% {
      background-position: 100% 50%;
    }
    100% {
      background-position: 0% 50%;
    }
  }
</style>

---

<div id="education" style="padding: 60px; background: linear-gradient(135deg, #ADD8E6, #87CEFA);">
  <h2 style="text-align: center; font-family: 'Comic Sans MS', cursive, sans-serif; color: #1E90FF;">Education</h2>
  
  <div style="display: flex; justify-content: center; align-items: center; gap: 20px;">
    
    <!-- FAU Logo -->
    <div>
      <img src="https://raw.githubusercontent.com/JennaLeali/JennaLealiWebsite/main/assets/images/fau-logo.png" alt="FAU Logo" style="max-width: 150px; border-radius: 5px;">
    </div>
    
    <!-- Education Details -->
    <div style="text-align: left; max-width: 600px;">
      <h3 style="color: #1E90FF; margin-bottom: 10px;">
        Master of Science in Data Science and Analytics, Florida Atlantic University
      </h3>
      <p><a href="https://www.fau.edu/engineering/eecs/graduate/ms/data-science-and-analytics/courses/" target="_blank" style="color: #1E90FF;">Link to Degree Requirements</a></p>
      <p>Minor in Artificial Intelligence - <a href="https://www.fau.edu/engineering/eecs/undergraduate/minors/artificial-intelligence/" target="_blank" style="color: #1E90FF;">Link to Minor Details</a></p>
      <p>Big Data Analytics Certificate - <a href="https://www.fau.edu/engineering/eecs/graduate/certificates/big-data/" target="_blank" style="color: #1E90FF;">Link to Certificate Details</a></p>
      <p><strong>(Expected graduation: Dec 2024)</strong></p>
      
      <h3 style="color: #1E90FF; margin-top: 30px; margin-bottom: 10px;">
        Bachelor of Science in Data Analytics, Florida Atlantic University Harriet L. Wilkes Honors College
      </h3>
      <p><a href="https://www.fau.edu/honors/academics/majors/data-analytics/" target="_blank" style="color: #1E90FF;">Link to Degree Requirements</a></p>
      <p>Minor in Economics - <a href="https://www.fau.edu/honors/academics/majors/economics/" target="_blank" style="color: #1E90FF;">Link to Minor Details</a></p>
      <p><strong>Graduated: 2024</strong></p>
    </div>
  
  </div>
  
</div>

---

<div style="background: linear-gradient(135deg, #FFB6C1, #FFD700); padding: 30px; border-radius: 15px; text-align: center; margin-top: 30px;">

  <h2 style="font-family: 'Comic Sans MS', cursive, sans-serif; color: #FF69B4; font-size: 40px; margin-bottom: 20px;">
    Read My Undergraduate Thesis
  </h2>

  <p style="font-size: 18px; color: #000; margin-bottom: 15px;">
    I completed my undergraduate thesis on data science and analytics at Florida Atlantic University. You can read it by clicking the button below:
  </p>

  <!-- Make the image larger and reduce the margin -->
  <div style="margin-bottom: 20px;">
    <img src="assets/images/thesis.png" alt="Thesis Image" style="max-width: 250px; border-radius: 5px;">
  </div>
  
  <a href="assets/documents/final.pdf" target="_blank" style="font-size: 18px; background-color: #FF69B4; color: white; padding: 12px 25px; border-radius: 5px; text-decoration: none; display: inline-block; margin-top: 10px;">
    Click here to read my thesis
  </a>

  <!-- Cool button link to Medallion Award Recipients page -->
  <div style="margin-top: 20px;">
    <a href="https://www.fau.edu/honors/current-students/student-awards/medallion-award-recipients/" target="_blank" style="font-size: 18px; background-color: #6A5ACD; color: white; padding: 12px 25px; border-radius: 5px; text-decoration: none; display: inline-block;">
      Learn more about the Medallion Award Recipients
    </a>
  </div>

</div>

---

<!-- Enhanced Resume Section with Rotating Border and Pulse Hover Effect -->
<div id="resume" style="padding: 60px; background: linear-gradient(135deg, #6A5ACD, #1E90FF); border-radius: 15px; position: relative; overflow: hidden;">
  <h2 style="font-family: 'Comic Sans MS', cursive, sans-serif; color: white; font-size: 45px; text-align: center; margin-bottom: 40px;">
    Resume
  </h2>

  <!-- Centering Content -->
  <div style="display: flex; flex-direction: column; align-items: center; justify-content: center; max-width: 80%; margin: 0 auto; position: relative; z-index: 1;">
    
    <!-- Resume image link with Glow, Pulse, and Rotating Border Effects -->
    <a href="resume.pdf" target="_blank" style="position: relative; display: inline-block;">
      <!-- Rotating border container -->
      <div class="rotate-border" style="position: absolute; top: -15px; left: -15px; width: calc(100% + 30px); height: calc(100% + 30px); border: 4px solid #FF69B4; border-radius: 15px; box-shadow: 0 0 15px rgba(255, 105, 180, 0.6); animation: rotate 5s linear infinite;"></div>
      <!-- Image -->
      <img src="assets/images/resume.png" alt="Resume Image" style="max-width: 250px; border-radius: 10px; box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1); transition: transform 0.3s ease, box-shadow 0.3s ease;">
    </a>
  
  </div>

  <!-- Hover Effects, Rotating Border, and Pulse Animation -->
  <style>
    /* Rotating border around the image */
    @keyframes rotate {
      0% {
        transform: rotate(0deg);
      }
      100% {
        transform: rotate(360deg);
      }
    }

    /* Resume image hover effect */
    a img:hover {
      transform: scale(1.1); /* Slight scaling effect */
      box-shadow: 0 8px 16px rgba(255, 105, 180, 0.4); /* Pink glow shadow on hover */
    }

    /* Enhanced gradient background animation */
    @keyframes gradientBackground {
      0% {
        background-position: 0% 50%;
      }
      50% {
        background-position: 100% 50%;
      }
      100% {
        background-position: 0% 50%;
      }
    }

    /* Pulse animation on hover */
    a:hover .rotate-border {
      animation: pulse 2s infinite alternate;
    }

    @keyframes pulse {
      from {
        box-shadow: 0 0 15px rgba(255, 105, 180, 0.6);
      }
      to {
        box-shadow: 0 0 30px rgba(255, 105, 180, 1);
      }
    }
  </style>
</div>

---

<div id="projects" style="padding: 60px; background-color: #F0F8FF;">
  <h2 style="text-align: center; font-family: 'Comic Sans MS', cursive, sans-serif; color: #1E90FF;">
    Projects
  </h2>
  <p style="text-align: center;">Here are some of the data science and analytics projects I’ve worked on:</p>
  <ul style="list-style-type: none; text-align: center;">
    <li><strong>Project 1</strong>: Description for Project 1</li>
    <li><strong>Project 2</strong>: Description for Project 2</li>
    <li><strong>Project 3</strong>: Description for Project 3</li>
    <li><strong>Project 4</strong>: Description for Project 4</li>
    <li><strong>Project 5</strong>: Description for Project 5</li>
  </ul>
</div>

---

<div id="fun-facts" style="background: linear-gradient(135deg, #FFB6C1, #FFD700); padding: 60px; border-radius: 15px;">
  <h2 style="font-family: 'Comic Sans MS', cursive, sans-serif; color: #FF69B4; font-size: 45px; text-align: center;">
    Fun Facts About Me
  </h2>

<div style="background: linear-gradient(135deg, #FFB6C1, #FFD700); padding: 40px; border-radius: 15px; text-align: center;">

  <!-- Flex container for fun facts -->
  <div style="display: flex; justify-content: space-around; align-items: flex-start; gap: 20px;">

    <!-- Fun fact 1 -->
    <div style="flex: 1; text-align: center;">
      <p style="font-size: 22px; font-family: 'Comic Sans MS', cursive; color: #FFFFFF;">
        1. I was a competitive swimmer growing up, participating in year-round, high school, summer league, and national teams.
      </p>
      <img src="assets/images/swim.png" alt="Swimming" style="max-width: 150px; border-radius: 5px;">
    </div>

    <!-- Fun fact 2 -->
    <div style="flex: 1; text-align: center;">
      <p style="font-size: 22px; font-family: 'Comic Sans MS', cursive; color: #FFFFFF;">
        2. My favorite food is crab legs.
      </p>
      <img src="assets/images/crab.png" alt="Crab Legs" style="max-width: 150px; border-radius: 5px;">
    </div>

    <!-- Fun fact 3 -->
    <div style="flex: 1; text-align: center;">
      <p style="font-size: 22px; font-family: 'Comic Sans MS', cursive; color: #FFFFFF;">
        3. I have a Golden Retriever named Murphy.
      </p>
      <img src="assets/images/golden.png" alt="Murphy" style="max-width: 150px; border-radius: 5px;">
    </div>

  </div>

</div>