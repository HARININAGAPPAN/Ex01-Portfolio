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
```
vamsi.html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>E.Vamsi Krishna Portfolio</title>

<link rel="stylesheet" href="style.css">

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">

<script src="script.js" defer></script>
</head>

<body>

<header>

<h2 class="logo">E.Vamsi Krishna</h2>

<nav>
<a href="#home">Home</a>
<a href="#about">About</a>
<a href="#skills">Skills</a>
<a href="#projects">Projects</a>
<a href="#contact">Contact</a>
</nav>

</header>

<section class="hero" id="home">

<div class="hero-text">

<h3>Hello 👋</h3>

<h1>I'm <span>E.Vamsi Krishna</span></h1>

<h2>AIDS</h2>

<p>
Java Developer • Spring Boot • Machine Learning • Web Development
</p>

<a href="#projects" class="btn">View Projects</a>

</div>

<div class="hero-image">
<img src="image/image.png" alt="Profile Picture">
</div>

</section>

<section id="about">

<h2>About Me</h2>

<div class="glass">

<p>
I'm a Computer Science student passionate about Java,
Spring Boot, Machine Learning and Backend Development.
I enjoy building projects that solve real-world problems while learning new technologies.
</p>

</div>

</section>

<section id="skills">

<h2>Skills</h2>

<div class="skills">

<div class="card">☕ Java</div>
<div class="card">🍃 Spring Boot</div>
<div class="card">🌐 HTML</div>
<div class="card">🎨 CSS</div>
<div class="card">⚡ JavaScript</div>
<div class="card">🗄 SQL</div>
<div class="card">🤖 Machine Learning</div>
<div class="card">🐙 Git & GitHub</div>

</div>

</section>

<section id="projects">

<h2>Projects</h2>

<div class="projects">

<div class="project">
<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQXGNhEPaLfH3rqR3m8KW9RjQ-QOtxosF91td_dMcQrBB7QxB58hQGw72g&s=10" alt="Student Management Project">
<h3>Student Management</h3>
<p>Java + Spring Boot + MySQL</p>
</div>

<div class="project">
<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR_DRMvqAxRKacDqZh7-tvDyPP4tbWUZCNSbuUs1AiLjJjKDNSrW4L8sXzM&s=10" alt="Machine Learning Project">
<h3>Machine Learning</h3>
<p>Classification Project</p>
</div>

<div class="project">
<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRJCokP2NH3ggfGmvG9noL9CyLCfZwFAj2Om_eevfM9_g&s=10" alt="Portfolio Website">
<h3>Portfolio Website</h3>
<p>HTML CSS JavaScript</p>
</div>

</div>

</section>

<section id="contact">

<h2>Contact</h2>

<p>Email: eramasivamsi777@gmail.com</p>

<div class="socials">
<a href="https://github.com/25005454" target="_blank">GitHub</a>
</div>

</section>

<footer>

Made by E.Vamsi Krishna

</footer>

</body>
</html>

```
```
*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:Poppins,sans-serif;
scroll-behavior:smooth;
}

body{
background:linear-gradient(135deg,#e778cf,#203a43,#3f6f84);
color:white;
}

header{
display:flex;
justify-content:space-between;
align-items:center;
padding:20px 8%;
position:fixed;
width:100%;
top:0;
background:rgba(0,0,0,.25);
backdrop-filter:blur(10px);
z-index:100;
}

.logo{
font-size:32px;
color:#00f2ff;
}

nav a{
color:white;
text-decoration:none;
margin-left:25px;
transition:.3s;
}

nav a:hover{
color:#00f2ff;
}

.hero{
display:flex;
justify-content:space-around;
align-items:center;
padding:120px 10%;
min-height:100vh;
flex-wrap:wrap;
}

.hero-text h3{
font-size:24px;
font-weight:400;
margin-bottom:10px;
}

.hero-text h1{
font-size:65px;
margin-bottom:10px;
}

.hero-text span{
color:#00f2ff;
}

.hero-text h2{
font-size:32px;
font-weight:600;
margin-bottom:15px;
}

.hero-text p{
margin:20px 0;
font-size:18px;
line-height:1.6;
}

.btn{
display:inline-block;
padding:15px 35px;
background:#00f2ff;
color:black;
text-decoration:none;
border-radius:40px;
font-weight:bold;
transition:.3s;
}

.btn:hover{
transform:scale(1.1);
background:#ff4ecd;
}

.hero-image img{
width:320px;
height:320px;
border-radius:50%;
border:6px solid #00f2ff;
object-fit:cover;
box-shadow:0 0 40px cyan;
}

section{
padding:80px 10%;
text-align:center;
}

section h2{
font-size:42px;
margin-bottom:40px;
}

.glass{
background:rgba(255,255,255,.1);
padding:30px;
border-radius:20px;
backdrop-filter:blur(15px);
}

.skills{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(180px,1fr));
gap:25px;
}

.card{
padding:35px;
background:linear-gradient(135deg,#ff6ec4,#7873f5);
border-radius:20px;
font-size:22px;
font-weight:bold;
transition:.4s;
}

.card:hover{
transform:translateY(-12px) scale(1.05);
}

.projects{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
gap:30px;
}

.project{
background:rgba(255,255,255,.08);
border-radius:20px;
overflow:hidden;
transition:.4s;
}

.project:hover{
transform:scale(1.05);
}

.project img{
width:100%;
height:220px;
object-fit:cover;
}

.project h3{
margin:15px 0;
}

.project p{
margin-bottom:20px;
}

.socials{
margin-top:20px;
}

.socials a{
display:inline-block;
margin:10px;
padding:12px 25px;
background:#00f2ff;
color:black;
text-decoration:none;
border-radius:30px;
font-weight:bold;
transition:.3s;
}

.socials a:hover{
background:#ff4ecd;
}

footer{
padding:25px;
text-align:center;
background:black;
margin-top:50px;
}

.fade{
opacity:0;
transform:translateY(40px);
transition:1s;
}

.show{
opacity:1;
transform:translateY(0);
}

@media(max-width:768px){

.hero{
flex-direction:column-reverse;
text-align:center;
padding-top:150px;
}

.hero-text h1{
font-size:45px;
}

.hero-text h2{
font-size:24px;
}

.hero-image img{
width:250px;
height:250px;
margin-bottom:30px;
}

header{
flex-direction:column;
padding:20px;
}

nav{
margin-top:15px;
}

nav a{
margin:0 10px;
display:inline-block;
}

.logo{
font-size:28px;
}

section h2{
font-size:34px;
}

}
```

## OUTPUT
<img width="1918" height="1078" alt="Screenshot 2026-07-29 204007" src="https://github.com/user-attachments/assets/b92198b1-4068-4a06-b590-a9d14d555e1f" />

<img width="1918" height="811" alt="Screenshot 2026-07-29 204205" src="https://github.com/user-attachments/assets/3e6a36cf-0b1b-4063-ba62-57973b54b895" />
<img width="1918" height="1018" alt="Screenshot 2026-07-29 204224" src="https://github.com/user-attachments/assets/628b2082-3ef0-4698-85cd-276a351322f1" />
<img width="1918" height="887" alt="Screenshot 2026-07-29 204250" src="https://github.com/user-attachments/assets/af12bbe7-1d83-49a3-a6d1-315ea47523e1" />




## RESULT
The program for creating Portfolio using HTML and CSS is executed successfully.
