# Ex01 Portfolio
## Date:

## AIM
To create a Portfolio using HTML and CSS.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for introduction, about, projects, and contact details.

### STEP 5
Define global styles for fonts, colors, and layout.

### STEP 6
Style the header, navigation bar, and sections.

### STEP 7
Use Flexbox or CSS Grid for layout design.

### STEP 8
Add hover effects and transitions for interactivity.

### STEP 9
Add Images and Media.

### STEP 10
Use optimized images for a professional look.

### STEP 11
Open the HTML file in a browser to check layout and functionality.

### STEP 12
Fix styling issues and refine content placement.

### STEP 13
Deploy the Portfolio.

### STEP 14
Upload to GitHub Pages for free hosting.

## PROGRAM
index.html
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Vasundra Sri R | Portfolio</title>
  <link rel="stylesheet" href="style.css" />
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap" rel="stylesheet">
</head>
<body>
  <header>
    <nav>
      <div class="logo">Vasundra Sri R</div>
      <ul>
        <li><a href="#intro">Home</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#certifications">Certifications</a></li>
        <li><a href="#skills">Skills</a></li>
        <li><a href="#projects">Projects</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <section id="intro" class="section">
    <div class="intro-container">
    <img src="vasundra img.jpeg" alt="Vasundra Sri" class="profile-img" />
    <div>
    <h1>Hello, I'm <span class="highlight">Vasundra Sri R</span></h1>
    <p class="subtitle">AI & Data Science Enthusiast | Problem Solver</p>
  </section>

  <section id="about" class="section">
    <h2>About Me</h2>
    <p>
      I'm a final-year engineering student specializing in Artificial Intelligence and Data Science. I’m passionate about building intelligent solutions, analyzing data, and designing clean web interfaces.
    </p>
    <p>
    During my internship at Arjun Vision Tech Solutions, I honed my skills in data preprocessing, model building, and performance evaluation using tools like Python, Pandas, and Scikit‑learn. I’m also well‑versed in web technologies—HTML, CSS. I’m passionate about applying AI to real‑world problems.
  </p>

  <section id="certifications" class="section">
  <h2>Certifications</h2>
  <ul class="cert-list">
    <li><strong>AWS Cloud Practitioner</strong></li>
    <li><strong>NPTEL - Introduction to IoT</strong></li>
    <li><strong>Introduction to Web Data Mining</strong></li>
  </ul>
</section>

<section id="skills" class="section">
  <h2>Skills</h2>
  <ul class="cert-list">
    <li>Python, Java, Pandas, NumPy, Scikit-learn, TensorFlow, Keras</li>
    <li>MySQL, Git, HTML, CSS</li>
    <li>Machine Learning, Deep Learning, Data Visualization</li>
  </ul>
</section>


  </section>

  <section id="projects" class="section">
  <h2>Projects</h2>

  <div class="project-card">
  <h3>Recruitment Revolution: Predictive Analysis for Smarter Hiring</h3>
  <img src="hiring.jpg" alt="Recruitment Revolution" class="project-img"/>
  <p><strong>Tools:</strong> Python, Scikit-learn, Pandas</p>
  <p>Built a predictive model using machine learning to help HR teams make smarter hiring decisions based on candidate data.</p>
</div>

<div class="project-card">
  <h3>Enhancing SAR for Interoperability through Colorization Using Deep Learning Models</h3>
  <img src="sar.jpg" alt="SAR Colorization" class="project-img"/>
  <p><strong>Tools:</strong> Python, OpenCV, TensorFlow</p>
  <p>Applied deep learning models to improve Synthetic Aperture Radar image interpretation by converting grayscale to color.</p>
</div>

<div class="project-card">
  <h3>Stock Price Predictor</h3>
  <img src="stock.png" alt="Stock Price Predictor" class="project-img"/>
  <p><strong>Tools:</strong> Python, Streamlit, yFinance, LSTM, Keras</p>
  <p>Developed a web app that predicts future stock prices using historical data and deep learning models.</p>
</div>

</section>


  <section id="contact" class="section">
  <h2>Contact</h2>
  <p>Phone: +917806983505</p>
  <p>Email: vasundrasri49@gmail.com</p>
  <p>LinkedIn: <a href="https://www.linkedin.com/in/vasundrasri" target="_blank">linkedin.com/in/vasundrasri</a></p>
  <p>GitHub: <a href="https://github.com/vasundrasriravi" target="_blank">github.com/vasundrasriravi</a></p>
</section>


  <footer>
    <p>© 2025 Vasundra Sri. All rights reserved.</p>
  </footer>
</body>
</html>
```
style.css
```
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html {
  scroll-behavior: smooth;
}

body {
  font-family: 'Poppins', sans-serif;
  background-color:#F5F5F5;
  color:#333333;
  line-height: 1.6;
}

header {
  background-color:#0D1B2A;
  color:#FCA311;
  padding: 20px 0;
  box-shadow: 0 2px 10px rgba(0,0,0,0.1);
}

.intro-container {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 40px;
  flex-wrap: wrap;
  text-align: center;
}

.profile-img {
  width: 202px;
  height: 202px;
  border-radius: 50%;
  object-fit: cover;
  border: 4px solid #fca311;
  box-shadow: 0 4px 10px rgba(0,0,0,0.1);
}

nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  max-width: 1200px;
  margin: auto;
  padding: 0 20px;
}

.cert-list {
  list-style: disc inside;
  max-width: 800px;
  margin: 0 auto;
  padding: 0;
}

.cert-list li {
  margin-bottom: 10px;
  font-size: 1rem;
  color: #444;
}

.logo {
  font-size: 1.5rem;
  font-weight: bold;
  color: #fca311;
}

nav ul {
  list-style: none;
  display: flex;
  gap: 30px;
}

nav a {
  color: #fff;
  text-decoration: none;
  font-weight: 600;
  transition: color 0.3s;
}

nav a:hover {
  color: #fca311;
}

.section {
  max-width: 1000px;
  margin: auto;
  padding: 60px 20px;
}

h1, h2 {
  text-align: center;
  margin-bottom: 20px;
}

.subtitle {
  text-align: center;
  font-size: 1.2rem;
  color: #555;
}

.highlight {
  color: #fca311;
}

.project-card {
  background: #fff;
  border: 1px solid #E36414;
  padding: 25px;
  margin-bottom: 25px;
  border-radius: 10px;
  transition: box-shadow 0.3s;
}

.project-card:hover {
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
}

.project-img {
  width: 80%;
  height: auto;
  max-height: 150px;
  object-fit: contain;
  margin: 15px auto;
  display: block;
  border-radius: 6px;
}


footer {
  background-color: #0d1b2a;
  color: #fff;
  text-align: center;
  padding: 20px;
  margin-top: 50px;
}

a {
  color: #fca311;
  text-decoration: none;
}

a:hover {
  text-decoration: underline;
}

/* Social Media Icons */
.social-links {
  margin-top: 15px;
  display: flex;
  justify-content: center;
  gap: 20px;
}

.social-links a {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 40px;
  height: 40px;
  background-color: #fff;
  border-radius: 50%;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
  color: #0d1b2a;
  font-size: 20px;
  transition: all 0.3s ease;
}

.social-links a:hover {
  transform: translateY(-3px);
  color: #fca311;
  box-shadow: 0 4px 12px rgba(0,0,0,0.15);
}
```
## OUTPUT
![Screenshot 2025-05-25 114853](https://github.com/user-attachments/assets/0635a5c1-148f-4e2a-823a-b4543e8373c1)

![Screenshot 2025-05-25 114908](https://github.com/user-attachments/assets/c003dbee-ecc2-4025-829c-d42babe61c96)

![Screenshot 2025-05-25 114943](https://github.com/user-attachments/assets/65316692-ad61-4a84-88ee-89a32b86c0a1)

![Screenshot 2025-05-25 115004](https://github.com/user-attachments/assets/dc604294-e88a-4f9e-8e4c-149f92e9c4ce)

## RESULT
The program for creating Portfolio using HTML and CSS is executed successfully.
