<!-- Navigation Bar -->
<div style="position: fixed; top: 0; left: 0; right: 0; background-color: #FFB6C1; padding: 15px 0; box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1); z-index: 999;">
  <div style="display: flex; justify-content: center; gap: 20px;">
    <a href="#home" style="color: white; font-size: 18px; text-decoration: none; padding: 10px;">Home</a>
    <a href="#projects" style="color: white; font-size: 18px; text-decoration: none; padding: 10px;">Projects</a>
    <a href="#contact" style="color: white; font-size: 18px; text-decoration: none; padding: 10px;">Contact</a>
    <a href="#education" style="color: white; font-size: 18px; text-decoration: none; padding: 10px;">Education</a>
    <a href="#thesis" style="color: white; font-size: 18px; text-decoration: none; padding: 10px;">Thesis</a>
    <a href="#resume" style="color: white; font-size: 18px; text-decoration: none; padding: 10px;">Resume</a>
    <a href="#timeline" style="color: white; font-size: 18px; text-decoration: none; padding: 10px;">Timeline</a>
    <a href="#fun-facts" style="color: white; font-size: 18px; text-decoration: none; padding: 10px;">Fun Facts</a>
  </div>
</div>

<!-- Home Section with Cream and Pink Theme -->
<div id="home" style="display: flex; flex-direction: column; align-items: center; justify-content: center; background: linear-gradient(135deg, #FFF5E4, #FFC1C1); padding: 40px; border-radius: 15px; min-height: 80vh; margin-top: 80px;">

  <!-- Row containing image and name -->
  <div style="display: flex; align-items: center; gap: 30px; margin-bottom: 30px;">
    <img src="assets/images/jenna.png" alt="Jenna Leali" style="max-width: 150px; border-radius: 10%; transition: transform 0.3s ease-in-out, box-shadow 0.3s ease-in-out;">
    
    <h1 style="font-family: 'Comic Sans MS', cursive, sans-serif; color: #FF69B4; font-size: 45px; text-align: center;">
      Jenna Leali
    </h1>
  </div>

  <!-- Typing animation directly below name -->
  <div class="typing-animation" style="font-size: 20px; color: #FF69B4; text-align: center; margin-bottom: 20px;">
    <span id="typed-text"></span>
    <span class="cursor">|</span>
  </div>

  <!-- Button under typing text -->
  <a href="https://github.com/JennaLeali" style="font-size: 18px; background-color: #FFB6C1; color: white; padding: 10px 15px; border-radius: 5px; text-decoration: none; margin-bottom: 20px;">
    View project on GitHub
  </a>

  <!-- CSS for Hover Effects -->
  <style>
    img:hover {
      transform: scale(1.2);
      box-shadow: 0 0 30px #FFB6C1;
    }

    /* Typing text animation */
    .typing-animation #typed-text {
      font-family: 'Comic Sans MS', cursive, sans-serif;
      color: #FF69B4;
      font-size: 20px;
      white-space: nowrap;
      overflow: hidden;
      border-right: 3px solid #FF69B4;
      width: 0;
      animation: typing 3s steps(40, end), blink-caret 0.75s step-end infinite;
    }

    @keyframes typing {
      from { width: 0; }
      to { width: 100%; }
    }

    @keyframes blink-caret {
      from, to { border-color: transparent; }
      50% { border-color: #FF69B4; }
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

<!-- Projects Section with Cards and Modal -->
<div id="projects" style="padding: 60px; background: linear-gradient(135deg, #FFD7D7, #FFF5E4); border-radius: 15px;">
  <h2 style="text-align: center; font-family: 'Comic Sans MS', cursive; color: #FF69B4;">
    Projects
  </h2>
  <p style="text-align: center; margin-bottom: 40px;">Click on a project to learn more.</p>

  <!-- Project Cards Container in a Single Row -->
  <div class="projects-grid" style="display: flex; justify-content: center; gap: 15px; flex-wrap: wrap; max-width: 100%; margin: 0 auto;">

    <!-- Project Card 1 -->
    <div class="project-card" id="openModalNN">
      <div class="project-card-content">
        <h3 style="font-family: 'Comic Sans MS', cursive; color: #FF69B4; font-size: 16px;">Neural Network Classifier</h3>
        <p style="font-size: 12px;">Implemented a neural network with gradient descent learning.</p>
      </div>
    </div>

    <!-- Project Card 2 -->
    <div class="project-card" id="openModalHF">
      <div class="project-card-content">
        <h3 style="font-family: 'Comic Sans MS', cursive; color: #FF69B4; font-size: 16px;">Heart Failure Risk Prediction</h3>
        <p style="font-size: 12px;">Predicting heart failure risk using machine learning techniques.</p>
      </div>
    </div>

    <!-- Project Card 3 -->
    <div class="project-card" id="openModalTB">
      <div class="project-card-content">
        <h3 style="font-family: 'Comic Sans MS', cursive; color: #FF69B4; font-size: 16px;">Binary Classification</h3>
        <p style="font-size: 12px;">Classified data using threshold-based rules and visualized results.</p>
      </div>
    </div>

    <!-- Project Card 4 -->
    <div class="project-card" id="openModalHD">
      <div class="project-card-content">
        <h3 style="font-family: 'Comic Sans MS', cursive; color: #FF69B4; font-size: 16px;">Handwritten Digit Recognition</h3>
        <p style="font-size: 12px;">Classified digits using feature engineering and thresholding.</p>
      </div>
    </div>

    <!-- Project Card 5 -->
    <div class="project-card" id="openModalBL">
      <div class="project-card-content">
        <h3 style="font-family: 'Comic Sans MS', cursive; color: #FF69B4; font-size: 16px;">Boolean Logic Operations</h3>
        <p style="font-size: 12px;">Performed Boolean operations on input data using Python.</p>
      </div>
    </div>

    <!-- Project Card 6 -->
    <div class="project-card" id="openModalTTT">
      <div class="project-card-content">
        <h3 style="font-family: 'Comic Sans MS', cursive; color: #FF69B4; font-size: 16px;">Tic-Tac-Toe Game</h3>
        <p style="font-size: 12px;">Developed an AI-powered Tic-Tac-Toe game using Minimax.</p>
      </div>
    </div>

    <!-- Project Card 7 -->
    <div class="project-card" id="openModalCIFAR">
      <div class="project-card-content">
        <h3 style="font-family: 'Comic Sans MS', cursive; color: #FF69B4; font-size: 16px;">CIFAR-10 Image Classification</h3>
        <p style="font-size: 12px;">Classified images using convolutional neural networks.</p>
      </div>
    </div>

    <!-- Project Card 8 -->
    <div class="project-card" id="openModalSandy">
      <div class="project-card-content">
        <h3 style="font-family: 'Comic Sans MS', cursive; color: #FF69B4; font-size: 16px;">Hurricane Sandy Analysis</h3>
        <p style="font-size: 12px;">Analyzed NYC 311 service requests during Hurricane Sandy.</p>
      </div>
    </div>

    <!-- Project Card 9 -->
    <div class="project-card" id="openModalEnergy">
      <div class="project-card-content">
        <h3 style="font-family: 'Comic Sans MS', cursive; color: #FF69B4; font-size: 16px;">Energy Consumption Prediction</h3>
        <p style="font-size: 12px;">Predicted energy consumption using linear regression.</p>
      </div>
    </div>

    <!-- Project Card 10 -->
    <div class="project-card" id="openModalFraud">
      <div class="project-card-content">
        <h3 style="font-family: 'Comic Sans MS', cursive; color: #FF69B4; font-size: 16px;">Credit Card Fraud Detection</h3>
        <p style="font-size: 12px;">Detected fraud using logistic regression.</p>
      </div>
    </div>

    <!-- Project Card 11 -->
    <div class="project-card" id="openModalPenguin">
      <div class="project-card-content">
        <h3 style="font-family: 'Comic Sans MS', cursive; color: #FF69B4; font-size: 16px;">Penguin Data Exploration</h3>
        <p style="font-size: 12px;">Explored penguin data using R.</p>
      </div>
    </div>

    <!-- Project Card 12 -->
    <div class="project-card" id="openModalDemographic">
      <div class="project-card-content">
        <h3 style="font-family: 'Comic Sans MS', cursive; color: #FF69B4; font-size: 16px;">Demographic Data Analysis</h3>
        <p style="font-size: 12px;">Analyzed demographic data using R.</p>
      </div>
    </div>

  </div>
</div>

<!-- CSS for Project Cards and Modal Styling -->
<style>
  .projects-grid {
    display: flex;
    justify-content: center;
    gap: 15px;
    flex-wrap: wrap;
  }

  .project-card {
    background-color: white;
    border-radius: 10px;
    padding: 15px;
    text-align: center;
    width: 150px;
    height: 130px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
    cursor: pointer;
  }

  .project-card-content {
    font-family: 'Georgia', serif;
    color: #333;
  }

  .project-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
  }

  .project-card h3 {
    font-size: 16px;
    margin-bottom: 10px;
  }

  .project-card p {
    font-size: 12px;
  }

  /* Modal Styling */
  .modal {
    display: none; /* Hidden by default */
    position: fixed; /* Stay in place */
    z-index: 1; /* Sit on top */
    left: 0;
    top: 0;
    width: 100%; /* Full width */
    height: 100%; /* Full height */
    background-color: rgba(0, 0, 0, 0.5); /* Black background with opacity */
  }

  .modal-content {
    background-color: white;
    margin: 15% auto;
    padding: 20px;
    border: 1px solid #888;
    width: 80%;
    max-width: 600px;
    border-radius: 10px;
  }

  .close {
    color: #aaa;
    float: right;
    font-size: 28px;
    font-weight: bold;
  }

  .close:hover,
  .close:focus {
    color: black;
    text-decoration: none;
    cursor: pointer;
  }
</style>

<!-- Modals for the Projects -->

<!-- Neural Network Classifier Modal -->
<div id="myModalNN" class="modal">
  <div class="modal-content">
    <span class="close" id="closeModalNN">&times;</span>
    <h2>Neural Network Classifier with Gradient Descent Learning</h2>
    <p><strong>Project Overview:</strong> In this project, I implemented a single-layer neural network with gradient descent learning. The project covers important machine learning concepts, such as forward propagation, sigmoid activation, and training using real data.</p>
    <p><strong>Key Skills Highlighted:</strong></p>
    <ul>
      <li>Machine Learning: Built a neural network from scratch, trained it using gradient descent, experimented with learning rates.</li>
      <li>Data Visualization: Visualized the classifier line, learning curves, and data points to interpret machine learning outcomes.</li>
      <li>Python Programming: Used Python libraries like numpy and matplotlib to create custom classes and methods.</li>
    </ul>
    <p><a href="assets/documents/Neural Network Classifier with Gradient Descent Learning.pdf" target="_blank">View Project PDF</a></p>
  </div>
</div>

<!-- Heart Failure Risk Prediction Modal -->
<div id="myModalHF" class="modal">
  <div class="modal-content">
    <span class="close" id="closeModalHF">&times;</span>
    <h2>Heart Failure Risk Prediction Using Machine Learning</h2>
    <p><strong>Project Overview:</strong> In this project, I explored clustering techniques (K-Means, Kernel K-Means, and Expectation Maximization), regression analysis (Linear Regression and Ridge Regression), and classification methods (Naive Bayes and K-Nearest Neighbors) to predict a patient’s risk of a heart-related death event.</p>
    <p><strong>Key Skills Highlighted:</strong></p>
    <ul>
      <li>Clustering Analysis: Used K-Means, Kernel K-Means, and Expectation Maximization to analyze unsupervised learning techniques.</li>
      <li>Regression and Classification: Implemented Linear and Ridge Regression, Naive Bayes, and KNN, focusing on predictive modeling.</li>
      <li>Model Comparison and Evaluation: Compared models, performed chi-square tests, and analyzed the clinical significance of clusters.</li>
    </ul>
    <p><a href="assets/documents/Heart Failure Risk Prediction Using Machine Learning.pdf" target="_blank">View Project PDF</a></p>
  </div>
</div>

<!-- Threshold-Based Binary Classification Modal -->
<div id="myModalTB" class="modal">
  <div class="modal-content">
    <span class="close" id="closeModalTB">&times;</span>
    <h2>Threshold-Based Binary Classification with Visualization</h2>
    <p><strong>Project Overview:</strong> I worked on a two-class classification problem using threshold values for the attributes x and y to distinguish between two classes (C1 and C2).</p>
    <p><strong>Key Skills Highlighted:</strong></p>
    <ul>
      <li>Classification & Decision Boundary Visualization: Visualized the decision boundary using a threshold-based rule.</li>
      <li>Data Visualization: Created scatter plots of data points for two different classes and overlaid threshold lines.</li>
      <li>User Interaction & Error Handling: Handled user input, including invalid inputs, in an interactive script.</li>
    </ul>
    <p><a href="assets/documents/Threshold-Based Binary Classification with Visualization.pdf" target="_blank">View Project PDF</a></p>
  </div>
</div>

<!-- Handwritten Digit Recognition Modal -->
<div id="myModalHD" class="modal">
  <div class="modal-content">
    <span class="close" id="closeModalHD">&times;</span>
    <h2>Handwritten Digit Recognition with Feature Engineering and Thresholding</h2>
    <p><strong>Project Overview:</strong> In this project, I loaded the MNIST dataset, split it into training and testing sets, and visualized the data. I focused on digits 0 and 8, using feature extraction to classify digits based on a threshold.</p>
    <p><strong>Key Skills Highlighted:</strong></p>
    <ul>
      <li>Data Handling and Splitting: Managed the MNIST dataset, selecting specific digits and dividing data into sets.</li>
      <li>Feature Extraction: Extracted features from images, demonstrating my understanding of dimensionality reduction.</li>
      <li>Threshold-Based Classification: Applied a threshold to classify digits and computed classification accuracy.</li>
    </ul>
    <p><a href="assets/documents/Handwritten Digit Recognition with Feature Engineering and Thresholding.pdf" target="_blank">View Project PDF</a></p>
  </div>
</div>

<!-- Boolean Logic Operations Modal -->
<div id="myModalBL" class="modal">
  <div class="modal-content">
    <span class="close" id="closeModalBL">&times;</span>
    <h2>Boolean Logic Operations and Visualization in Python</h2>
    <p><strong>Project Overview:</strong> I performed Boolean operations on four input data points using Python functions, implemented AND, OR, and XOR operations, and visualized the data.</p>
    <p><strong>Key Skills Highlighted:</strong></p>
    <ul>
      <li>Logical Operations: Demonstrated proficiency with fundamental Boolean operations, key for decision-making algorithms.</li>
      <li>Data Visualization: Used matplotlib to plot data points, showcasing skills in visual data interpretation.</li>
      <li>Iteration and Function Design: Created reusable functions and implemented loops to process data iteratively.</li>
    </ul>
    <p><a href="assets/documents/Boolean Logic Operations and Visualization in Python.pdf" target="_blank">View Project PDF</a></p>
  </div>
</div>

<!-- Tic-Tac-Toe Game Modal -->
<div id="myModalTTT" class="modal">
  <div class="modal-content">
    <span class="close" id="closeModalTTT">&times;</span>
    <h2>Building an AI-Powered Tic-Tac-Toe Game in Python</h2>
    <p><strong>Project Overview:</strong> In this project, I created a Tic-Tac-Toe game where a player competes against the computer, using the Minimax algorithm to make optimal moves.</p>
    <p><strong>Key Skills Highlighted:</strong></p>
    <ul>
      <li>Game Development: Demonstrated turn-based game creation with interactive input and display.</li>
      <li>AI and Search Algorithms: Implemented the Minimax algorithm, showcasing AI search techniques.</li>
      <li>Input Validation and Error Handling: Handled user input effectively, ensuring a robust program structure.</li>
    </ul>
    <p><a href="assets/documents/Building an AI-Powered Tic-Tac-Toe Game in Python.pdf" target="_blank">View Project PDF</a></p>
  </div>
</div>

<!-- CIFAR-10 Image Classification Modal -->
<div id="myModalCIFAR" class="modal">
  <div class="modal-content">
    <span class="close" id="closeModalCIFAR">&times;</span>
    <h2>CIFAR-10 Image Classification Using Convolutional Neural Networks</h2>
    <p><strong>Project Overview:</strong> This project involved building multiple CNN architectures to classify images from the CIFAR-10 dataset into 10 categories. I went through several iterations of model building and optimization.</p>
    <p><strong>Key Skills Highlighted:</strong></p>
    <ul>
      <li>Deep Learning: Demonstrated proficiency in CNNs, including convolutional layers, pooling layers, and fully connected layers.</li>
      <li>Model Optimization: Implemented data augmentation and batch normalization to improve model performance.</li>
      <li>Evaluation and Plotting: Evaluated models on training, validation, and testing data, and plotted loss/accuracy curves.</li>
    </ul>
    <p><a href="assets/documents/CIFAR-10 Image Classification Using Convolutional Neural Networks.pdf" target="_blank">View Project PDF</a></p>
  </div>
</div>

<!-- Hurricane Sandy Analysis Modal -->
<div id="myModalSandy" class="modal">
  <div class="modal-content">
    <span class="close" id="closeModalSandy">&times;</span>
    <h2>Analyzing the Impact of Hurricane Sandy on NYC 311 Service Requests</h2>
    <p><strong>Project Overview:</strong> In this project, I analyzed the NYC 311 dataset to assess how service requests changed before, during, and after Hurricane Sandy.</p>
    <p><strong>Key Skills Highlighted:</strong></p>
    <ul>
      <li>Data Wrangling: Cleaned and processed large datasets, dealing with missing values and duplicates.</li>
      <li>Data Visualization: Created informative visualizations using matplotlib and seaborn to display trends and comparisons.</li>
      <li>EDA and Comparative Analysis: Conducted comparative analysis across time periods, complaint types, and agencies.</li>
    </ul>
    <p><a href="assets/documents/Analyzing the Impact of Hurricane Sandy on NYC 311 Service Requests.pdf" target="_blank">View Project PDF</a></p>
  </div>
</div>

<!-- Energy Consumption Prediction Modal -->
<div id="myModalEnergy" class="modal">
  <div class="modal-content">
    <span class="close" id="closeModalEnergy">&times;</span>
    <h2>Energy Consumption Prediction Using Linear Regression</h2>
    <p><strong>Project Overview:</strong> In this project, I applied linear regression to a dataset containing household energy consumption data. I explored the relationship between various weather-related variables (temperature, humidity, dewpoint) and energy usage.</p>
    <p><strong>Key Skills Highlighted:</strong></p>
    <ul>
      <li>Regression Analysis: Implemented linear regression, adjusted for multicollinearity, and interpreted the model’s fit and coefficients.</li>
      <li>Data Wrangling: Handled missing values, created new features (season), and conducted thorough data cleaning.</li>
      <li>Model Evaluation: Evaluated the model using metrics such as MAE, MSE, RMSE, and R².</li>
    </ul>
    <p><a href="assets/documents/Linear Regression and Binary Classification.pdf" target="_blank">View Project PDF</a></p>
  </div>
</div>

<!-- Credit Card Fraud Detection Modal -->
<div id="myModalFraud" class="modal">
  <div class="modal-content">
    <span class="close" id="closeModalFraud">&times;</span>
    <h2>Credit Card Fraud Detection Using Logistic Regression</h2>
    <p><strong>Project Overview:</strong> In this project, I built a logistic regression model to classify fraudulent transactions in a highly imbalanced credit card dataset.</p>
    <p><strong>Key Skills Highlighted:</strong></p>
    <ul>
      <li>Classification with Imbalanced Data: Handled imbalanced data by applying class weights and evaluating metrics beyond accuracy.</li>
      <li>Model Evaluation: Used metrics such as accuracy, precision, recall, F1-score, and AUC-ROC to assess model performance.</li>
      <li>Data Scaling and Feature Engineering: Applied scaling to the transaction amount feature.</li>
    </ul>
    <p><a href="assets/documents/Linear Regression and Binary Classification.pdf" target="_blank">View Project PDF</a></p>
  </div>
</div>

<!-- Penguin Data Exploration Modal -->
<div id="myModalPenguin" class="modal">
  <div class="modal-content">
    <span class="close" id="closeModalPenguin">&times;</span>
    <h2>Penguin Data Exploration and Visualization Project</h2>
    <p><strong>Project Overview:</strong> I analyzed the Palmer Penguins dataset using R and packages from the tidyverse. The goal was to explore patterns in penguin species characteristics, such as bill length, flipper length, and body mass.</p>
    <p><strong>Key Skills Highlighted:</strong></p>
    <ul>
      <li>Data Wrangling and Exploration: Used tidyverse to clean, summarize, and explore the dataset.</li>
      <li>Data Visualization: Created various visualizations such as box plots, scatter plots, and bar plots using ggplot2.</li>
      <li>Statistical Analysis: Calculated and interpreted summary statistics to uncover insights about penguin species differences.</li>
    </ul>
    <p><a href="assets/documents/Penguin Data Exploration and Visualization Project using R.pdf" target="_blank">View Project PDF</a></p>
  </div>
</div>

<!-- Demographic Data Analysis Modal -->
<div id="myModalDemographic" class="modal">
  <div class="modal-content">
    <span class="close" id="closeModalDemographic">&times;</span>
    <h2>Demographic Data Analysis Using R</h2>
    <p><strong>Project Overview:</strong> I analyzed a demographic dataset using R and packages from the tidyverse. The dataset contained various demographic attributes such as age, credit score, education, occupation, marital status, and more. My goal was to explore how these attributes affect credit scores and uncover trends or patterns that could provide actionable insights.</p>
    <p><strong>Key Skills Highlighted:</strong></p>
    <ul>
      <li>Data Wrangling and Cleaning: Handled missing data, created new variables, and performed outlier detection and removal.</li>
      <li>Data Visualization: Created box plots, scatter plots, and bar plots using ggplot2.</li>
      <li>Descriptive and Aggregative Analysis: Summarized and aggregated data by attributes like education, marital status, and occupation.</li>
    </ul>
    <p><a href="assets/documents/Demographic Data Analysis Project using R.pdf" target="_blank">View Project PDF</a></p>
  </div>
</div>

<!-- JavaScript to Open and Close Modals -->
<script>
  const modals = {
    NN: document.getElementById("myModalNN"),
    HF: document.getElementById("myModalHF"),
    TB: document.getElementById("myModalTB"),
    HD: document.getElementById("myModalHD"),
    BL: document.getElementById("myModalBL"),
    TTT: document.getElementById("myModalTTT"),
    CIFAR: document.getElementById("myModalCIFAR"),
    Sandy: document.getElementById("myModalSandy"),
    Energy: document.getElementById("myModalEnergy"),
    Fraud: document.getElementById("myModalFraud"),
    Penguin: document.getElementById("myModalPenguin"),
    Demographic: document.getElementById("myModalDemographic"),
  };

  const btns = {
    NN: document.getElementById("openModalNN"),
    HF: document.getElementById("openModalHF"),
    TB: document.getElementById("openModalTB"),
    HD: document.getElementById("openModalHD"),
    BL: document.getElementById("openModalBL"),
    TTT: document.getElementById("openModalTTT"),
    CIFAR: document.getElementById("openModalCIFAR"),
    Sandy: document.getElementById("openModalSandy"),
    Energy: document.getElementById("openModalEnergy"),
    Fraud: document.getElementById("openModalFraud"),
    Penguin: document.getElementById("openModalPenguin"),
    Demographic: document.getElementById("openModalDemographic"),
  };

  const spans = {
    NN: document.getElementById("closeModalNN"),
    HF: document.getElementById("closeModalHF"),
    TB: document.getElementById("closeModalTB"),
    HD: document.getElementById("closeModalHD"),
    BL: document.getElementById("closeModalBL"),
    TTT: document.getElementById("closeModalTTT"),
    CIFAR: document.getElementById("closeModalCIFAR"),
    Sandy: document.getElementById("closeModalSandy"),
    Energy: document.getElementById("closeModalEnergy"),
    Fraud: document.getElementById("closeModalFraud"),
    Penguin: document.getElementById("closeModalPenguin"),
    Demographic: document.getElementById("closeModalDemographic"),
  };

  for (let key in btns) {
    btns[key].onclick = function() {
      modals[key].style.display = "block";
    };
    spans[key].onclick = function() {
      modals[key].style.display = "none";
    };
  }

  window.onclick = function(event) {
    for (let key in modals) {
      if (event.target === modals[key]) {
        modals[key].style.display = "none";
      }
    }
  };
</script>

---

<!-- Contact Section with Animated Icons and Subtle Background Animation -->
<div id="contact" style="padding: 60px; background: linear-gradient(135deg, #FFF5E4, #FFB6C1); border-radius: 15px; background-size: 400% 400%; animation: gradientAnimation 5s ease infinite;">
  <h2 style="font-family: 'Comic Sans MS', cursive, sans-serif; color: #FF69B4; font-size: 45px; text-align: center; margin-bottom: 40px;">
    Contact Information
  </h2>

  <div style="display: flex; flex-direction: column; align-items: center; gap: 20px;">
    
    <!-- Email with Icon -->
    <div>
      <a href="mailto:jallureleali@gmail.com" style="font-size: 20px; background-color: #FFD7D7; color: white; padding: 15px 30px; border-radius: 5px; text-decoration: none; display: flex; align-items: center; gap: 10px; transition: background-color 0.3s ease, transform 0.3s ease;">
        <img src="assets/icons/email.png" alt="Email Icon" style="width: 35px;"> Click here to email me
      </a>
    </div>

    <!-- LinkedIn with Icon -->
    <div>
      <a href="https://www.linkedin.com/in/jennaleali/" target="_blank" style="font-size: 20px; background-color: #FFD7D7; color: white; padding: 15px 30px; border-radius: 5px; text-decoration: none; display: flex; align-items: center; gap: 10px; transition: background-color 0.3s ease, transform 0.3s ease;">
        <img src="assets/icons/linkedin.png" alt="LinkedIn Icon" style="width: 35px;"> Click here to see my LinkedIn
      </a>
    </div>

    <!-- GitHub with Icon -->
    <div>
      <a href="https://github.com/JennaLeali" target="_blank" style="font-size: 20px; background-color: #FFD7D7; color: white; padding: 15px 30px; border-radius: 5px; text-decoration: none; display: flex; align-items: center; gap: 10px; transition: background-color 0.3s ease, transform 0.3s ease;">
        <img src="assets/icons/github.png" alt="GitHub Icon" style="width: 35px;"> Click here to visit my GitHub
      </a>
    </div>
  
  </div>
</div>

<!-- CSS for Hover Effects and Background Animation -->
<style>
  #contact a:hover {
    background-color: #FFE5E5; /* Slightly lighter pink on hover */
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

<div id="education" style="padding: 60px; background: linear-gradient(135deg, #FFE5E5, #FFD7D7);">
  <h2 style="text-align: center; font-family: 'Comic Sans MS', cursive, sans-serif; color: #FF69B4;">Education</h2>
  
  <div style="display: flex; justify-content: center; align-items: center; gap: 20px;">
    
    <!-- FAU Logo -->
    <div>
      <img src="https://raw.githubusercontent.com/JennaLeali/JennaLealiWebsite/main/assets/images/fau-logo.png" alt="FAU Logo" style="max-width: 150px; border-radius: 5px;">
    </div>
    
    <!-- Education Details -->
    <div style="text-align: left; max-width: 600px;">
      <h3 style="color: #FF69B4; margin-bottom: 10px;">
        Master of Science in Data Science and Analytics, Florida Atlantic University
      </h3>
      <p><a href="https://www.fau.edu/engineering/eecs/graduate/ms/data-science-and-analytics/courses/" target="_blank" style="color: #FF69B4;">Link to Degree Requirements</a></p>
      <p>Minor in Artificial Intelligence - <a href="https://www.fau.edu/engineering/eecs/undergraduate/minors/artificial-intelligence/" target="_blank" style="color: #FF69B4;">Link to Minor Details</a></p>
      <p>Big Data Analytics Certificate - <a href="https://www.fau.edu/engineering/eecs/graduate/certificates/big-data/" target="_blank" style="color: #FF69B4;">Link to Certificate Details</a></p>
      <p><strong>(Expected graduation: Dec 2024)</strong></p>
      
      <h3 style="color: #FF69B4; margin-top: 30px; margin-bottom: 10px;">
        Bachelor of Science in Data Analytics, Florida Atlantic University Harriet L. Wilkes Honors College
      </h3>
      <p><a href="https://www.fau.edu/honors/academics/majors/data-analytics/" target="_blank" style="color: #FF69B4;">Link to Degree Requirements</a></p>
      <p>Minor in Economics - <a href="https://www.fau.edu/honors/academics/majors/economics/" target="_blank" style="color: #FF69B4;">Link to Minor Details</a></p>
      <p><strong>Graduated: 2024</strong></p>
    </div>
  
  </div>
  
</div>

---

<div id="thesis" style="background: linear-gradient(135deg, #FFD7D7, #FFF5E4); padding: 30px; border-radius: 15px; text-align: center; margin-top: 30px;">

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
    <a href="https://www.fau.edu/honors/current-students/student-awards/medallion-award-recipients/" target="_blank" style="font-size: 18px; background-color: #FFB6C1; color: white; padding: 12px 25px; border-radius: 5px; text-decoration: none; display: inline-block;">
      Learn more about the Medallion Award Recipients
    </a>
  </div>

</div>
---

<!-- Enhanced Resume Section with Rotating Border and Pulse Hover Effect -->
<div id="resume" style="padding: 60px; background: linear-gradient(135deg, #FFE5E5, #FFD7D7); border-radius: 15px; position: relative; overflow: hidden;">
  <h2 style="font-family: 'Comic Sans MS', cursive, sans-serif; color: #FF69B4; font-size: 45px; text-align: center; margin-bottom: 40px;">
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

<!-- Horizontal Sliding Achievements Timeline Section -->
<div id="timeline" style="padding: 60px; background: linear-gradient(135deg, #FFD7D7, #FFF5E4); border-radius: 15px; text-align: center; margin-top: 30px;">
  <h2 style="font-family: 'Comic Sans MS', cursive, sans-serif; color: #FF69B4; font-size: 40px; margin-bottom: 20px;">
    Achievements Timeline
  </h2>

  <!-- Slider Container -->
  <div id="slider-container" style="position: relative; max-width: 1000px; margin: 0 auto;">
    <!-- Slider -->
    <input type="range" id="timeline-slider" min="0" max="8" step="1" value="0" style="width: 100%;">

    <!-- Timeline Dates -->
    <div id="timeline-items" style="display: flex; justify-content: space-between; position: relative; margin-top: 20px;">
      <!-- Each timeline item -->
      <div class="timeline-item" data-index="0" style="position: relative;">
        <p class="timeline-term" style="font-size: 18px; font-weight: bold; color: #FF69B4; margin-bottom: 5px;">Fall 2021</p>
        <div class="timeline-content">
          <p style="font-size: 14px; font-family: 'Georgia', serif; color: #333; padding: 10px;">
            <strong>Relevant Coursework:</strong> Honors Introductory Statistics<br>
            <strong>Experience:</strong> Entered FAU's Honors College, Majored in Data Analytics
          </p>
        </div>
      </div>

      <div class="timeline-item" data-index="1" style="position: relative;">
        <p class="timeline-term" style="font-size: 18px; font-weight: bold; color: #FF69B4; margin-bottom: 5px;">Spring 2022</p>
        <div class="timeline-content">
          <p style="font-size: 14px; font-family: 'Georgia', serif; color: #333; padding: 10px;">
            <strong>Relevant Coursework:</strong> Honors Intro to Data Science, Intro to Programming in C
          </p>
        </div>
      </div>

      <div class="timeline-item" data-index="2" style="position: relative;">
        <p class="timeline-term" style="font-size: 18px; font-weight: bold; color: #FF69B4; margin-bottom: 5px;">Fall 2022</p>
        <div class="timeline-content">
          <p style="font-size: 14px; font-family: 'Georgia', serif; color: #333; padding: 10px;">
            <strong>Relevant Coursework:</strong> Honors Discrete Mathematics
          </p>
        </div>
      </div>

      <div class="timeline-item" data-index="3" style="position: relative;">
        <p class="timeline-term" style="font-size: 18px; font-weight: bold; color: #FF69B4; margin-bottom: 5px;">Spring 2023</p>
        <div class="timeline-content">
          <p style="font-size: 14px; font-family: 'Georgia', serif; color: #333; padding: 10px;">
            <strong>Relevant Coursework:</strong> Data Structures/Algorithm Analysis, Honors Calculus-Analytic Geometry, Intro to Internet Computing
          </p>
        </div>
      </div>

      <div class="timeline-item" data-index="4" style="position: relative;">
        <p class="timeline-term" style="font-size: 18px; font-weight: bold; color: #FF69B4; margin-bottom: 5px;">Summer 2023</p>
        <div class="timeline-content">
          <p style="font-size: 14px; font-family: 'Georgia', serif; color: #333; padding: 10px;">
            <strong>Relevant Coursework:</strong> Intro to Database Structures<br>
            <strong>Experience:</strong> Data Analytics Intern at MRI Software
          </p>
        </div>
      </div>

      <div class="timeline-item" data-index="5" style="position: relative;">
        <p class="timeline-term" style="font-size: 18px; font-weight: bold; color: #FF69B4; margin-bottom: 5px;">Fall 2023</p>
        <div class="timeline-content">
          <p style="font-size: 14px; font-family: 'Georgia', serif; color: #333; padding: 10px;">
            <strong>Relevant Coursework:</strong> Intro to Artificial Intelligence, Intro Data Mining/Machine Learning, Intro to Data Science (M.S.)<br>
            <strong>Experience:</strong> People Analytics and Data Intern at FreshRX, Began thesis work for M.S.
          </p>
        </div>
      </div>

      <div class="timeline-item" data-index="6" style="position: relative;">
        <p class="timeline-term" style="font-size: 18px; font-weight: bold; color: #FF69B4; margin-bottom: 5px;">Spring 2024</p>
        <div class="timeline-content">
          <p style="font-size: 14px; font-family: 'Georgia', serif; color: #333; padding: 10px;">
            <strong>Relevant Coursework:</strong> Data Analysis for Managers (M.S.), Intro Business Analytics Big Data (M.S.), Intro to Deep Learning, Software Engineering (M.S.)<br>
            <strong>Experience:</strong> Submitted thesis and graduated with B.S. in Data Analytics
          </p>
        </div>
      </div>

      <div class="timeline-item" data-index="7" style="position: relative;">
        <p class="timeline-term" style="font-size: 18px; font-weight: bold; color: #FF69B4; margin-bottom: 5px;">Summer 2024</p>
        <div class="timeline-content">
          <p style="font-size: 14px; font-family: 'Georgia', serif; color: #333; padding: 10px;">
            <strong>Relevant Coursework:</strong> Advanced Business Analytics, AI, Deep Learning (M.S.)<br>
            <strong>Experience:</strong> Data Analytics Intern at Voloridge
          </p>
        </div>
      </div>

      <div class="timeline-item" data-index="8" style="position: relative;">
        <p class="timeline-term" style="font-size: 18px; font-weight: bold; color: #FF69B4; margin-bottom: 5px;">Fall 2024</p>
        <div class="timeline-content">
          <p style="font-size: 14px; font-family: 'Georgia', serif; color: #333; padding: 10px;">
            <strong>Relevant Coursework:</strong> Data Mining & Machine Learning, Information Retrieval, Intro to Neural Networks, Natural Language Processing (M.S.)<br>
            <strong>Experience:</strong> Part-Time Data Analyst at Voloridge, Planning to graduate with M.S. in Dec 2024
          </p>
        </div>
      </div>
    </div>
  </div>

</div>

<!-- Custom-styled slider -->
<style>
  /* Style the track */
  input[type="range"] {
    -webkit-appearance: none;
    width: 100%;
    height: 8px;
    background: linear-gradient(135deg, #FF69B4, #FFD7D7);
    border-radius: 10px;
    outline: none;
    opacity: 0.7;
    transition: opacity 0.2s;
  }

  /* Change slider thumb on hover */
  input[type="range"]:hover {
    opacity: 1;
  }

  /* Style the slider thumb (handle) */
  input[type="range"]::-webkit-slider-thumb {
    -webkit-appearance: none;
    appearance: none;
    width: 25px;
    height: 25px;
    background: #FF69B4;
    border-radius: 50%;
    box-shadow: 0 0 10px rgba(255, 105, 180, 0.5);
    cursor: pointer;
    transition: transform 0.3s ease;
  }

  /* Hover effect on the slider thumb */
  input[type="range"]::-webkit-slider-thumb:hover {
    transform: scale(1.2);
    box-shadow: 0 0 15px rgba(255, 105, 180, 0.8);
  }

  /* Hide timeline content by default */
  .timeline-content {
    display: none;
    font-family: 'Georgia', serif;
  }

  /* Show content when the slider reaches the item */
  .timeline-item.active .timeline-content {
    display: block;
  }

  /* Increase font size when a date is active */
  .timeline-item.active .timeline-term {
    font-size: 22px;
  }

  /* Ensure the text looks polished and consistent */
  .timeline-content p {
    font-size: 14px;
    line-height: 1.5;
  }
</style>

<!-- JavaScript for Slider Functionality -->
<script>
  const timelineItems = document.querySelectorAll(".timeline-item");
  const timelineSlider = document.getElementById("timeline-slider");

  timelineSlider.addEventListener("input", function() {
    const index = parseInt(this.value);

    timelineItems.forEach((item, i) => {
      const content = item.querySelector(".timeline-content");
      if (i === index) {
        item.classList.add("active");
        content.style.display = "block";
      } else {
        item.classList.remove("active");
        content.style.display = "none";
      }
    });
  });

  // Initialize the first timeline item as active
  timelineItems[0].classList.add("active");
</script>

---
<!-- Fun Facts Section with Flipping Cards -->
<div id="fun-facts" style="padding: 60px; background-color: #FFD7D7; border-radius: 15px;">
  <h2 style="text-align: center; font-family: 'Comic Sans MS', cursive; color: #FF69B4;">
    Fun Facts About Me
  </h2>
  <div class="fun-facts-grid" style="display: flex; justify-content: center; gap: 40px; flex-wrap: wrap; margin-top: 30px;">
    <!-- Fun Fact 1 -->
    <div class="flip-card">
      <div class="flip-card-inner">
        <div class="flip-card-front">
          <img src="assets/images/swim.png" alt="Swimming" style="max-width: 100%; border-radius: 10px;">
        </div>
        <div class="flip-card-back">
          <p style="font-family: 'Georgia', serif; color: white; text-align: center;">I was a competitive swimmer growing up, participating in year-round, high school, summer league, and national teams.</p>
        </div>
      </div>
    </div>

    <!-- Fun Fact 2 -->
    <div class="flip-card">
      <div class="flip-card-inner">
        <div class="flip-card-front">
          <img src="assets/images/crab.png" alt="Crab Legs" style="max-width: 100%; border-radius: 10px;">
        </div>
        <div class="flip-card-back">
          <p style="font-family: 'Georgia', serif; color: white; text-align: center;">My favorite food is crab legs.</p>
        </div>
      </div>
    </div>

    <!-- Fun Fact 3 -->
    <div class="flip-card">
      <div class="flip-card-inner">
        <div class="flip-card-front">
          <img src="assets/images/golden.png" alt="Murphy" style="max-width: 100%; border-radius: 10px;">
        </div>
        <div class="flip-card-back">
          <p style="font-family: 'Georgia', serif; color: white; text-align: center;">I have a Golden Retriever named Murphy.</p>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- CSS for Flip Card Effect -->
<style>
  /* Container for the flip cards */
  .flip-card {
    background-color: transparent;
    width: 200px;
    height: 300px;
    perspective: 1000px; /* This gives a 3D effect when flipping */
    margin: 10px;
  }

  /* Inner container that holds both the front and back */
  .flip-card-inner {
    position: relative;
    width: 100%;
    height: 100%;
    text-align: center;
    transition: transform 0.8s;
    transform-style: preserve-3d;
  }

  /* On hover, rotate the card */
  .flip-card:hover .flip-card-inner {
    transform: rotateY(180deg);
  }

  /* The front side of the card */
  .flip-card-front, .flip-card-back {
    position: absolute;
    width: 100%;
    height: 100%;
    -webkit-backface-visibility: hidden; /* Safari */
    backface-visibility: hidden;
    border-radius: 10px;
  }

  /* Styling for the front side (with image) */
  .flip-card-front {
    background-color: #FFF5E4;
    color: black;
  }

  /* Styling for the back side (with text) */
  .flip-card-back {
    background-color: #FF69B4;
    color: white;
    transform: rotateY(180deg); /* This is hidden by default until the card flips */
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 15px;
    font-family: 'Georgia', serif;
    text-align: center;
  }
</style>