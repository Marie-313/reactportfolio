<!DOCTYPE html>
<html lang="en">
  <head>
    <meta http-equiv="Content-Type" content="text/html; charset=UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>My Responsive Page</title>
    <style>
      body {
        font-family: Verdana, Geneva, Tahoma, sans-serif;
        margin: 0;
        padding: 0;
        background-color: rgb(245, 241, 208);
      }
      header {
        background-color: #67a8f3;
        color: rgb(13, 14, 10);
        padding: 10px 20px;
        display: flex;
        justify-content: flex-start;
      }
      h1 {
        text-align: center;
        padding: 3%;
        margin: 3%;
      }
      h2 {
        text-align: center;
        padding: 0%;
        margin: 0%;
      }
      nav {
        display: flex;
        gap: 15px;
      }
      nav a {
        color: rgb(68, 41, 41);
        text-decoration: none;
      }
      nav a:hover {
        text-decoration: underline;
        color: rgb(247, 247, 244);
      }
      main {
        height: 100vh;
        overflow: auto;
      }
      section {
        display: none;
        height: 100%;
        padding: 20px;
      }
      section.active {
        display: block;
      }
      footer {
        background-color: #4999f5;
        color: rgb(0, 0, 0);
        text-align: center;
        padding: 10px 0;
        position: relative;
        bottom: 0;
        width: 100%;
      }
      img,
      video {
        max-width: 100%;
        height: auto;
        display: block;
        margin: 10px auto;
      }
      img {
        text-align: center;
      }
      .medium-text {
        font-size: 20px;
        font-weight: bold;
        text-align: center;
        color: #358ef3;
      }
      .large-text {
        font-size: 29px;
        font-weight: bold;
        text-align: center;
        color: #29015e;
      }
      .project-grid {
        display: grid;
        grid-template-columns: repeat(2, 1fr);
        grid-template-rows: repeat(2, 1fr);
        gap: 20px;
        margin: 20px;
      }
      section#projects.active {
        display: block;
        height: auto;
        overflow-y: auto;
      }
      .project-item {
        background-color: #4696f1;
        border-radius: 8px;
        padding: 15px;
        display: flex;
        flex-direction: row;
        align-items: center;
      }
      .project-description {
        flex: 1;
        padding-right: 20px;
      }
      .project-image {
        flex: 1;
      }
      .project-image img {
        width: 100%;
        height: 200px;
        object-fit: cover;
        border-radius: 8px;
      }
       @media (max-width: 768px) {
        .project-grid {
          grid-template-columns: 1fr;
        }
      .project-item {
          flex-direction: column;
        }
      .project-description {
          padding-right: 0;
          padding-bottom: 15px;
        }
      }
    </style>
  </head>
  <body>
    <header>
      <nav>
        <a href="#" onclick="showSection('home')">Home</a>
        <a href="#" onclick="showSection('about')">About Me</a>
        <a href="#" onclick="showSection('projects')">My Projects</a>
      </nav>
    </header>
    <main>
      <section id="home" class="active">
        <h1>👩🏼‍💻I'm Maria Weathington👩🏼‍💻</h1>
        <video controls>
          <source
            src="https://www.w3schools.com/html/mov_bbb.mp4"
            type="video/mp4"
          />
        </video>
        <p class="medium-text">A Software Developer based in America.</p>
        <p class="large-text">
          I specialize in creating efficient and scalable software solutions.
        </p>
      </section>

      <section id="about">
        <h2>About Me</h2>
        <p>
          Maria Weathington is a software developer with a passion for
          coding and design. Born and raised in Detroit, Michigan, Maria
          discovered her love for programming through SheCodes.io, where her
          curiosity blossomed into a full-fledged career as a Front-End
          Developer. Maria was drawn to the
          limitless possibilities that software development offers. She finds
          joy in the process of creating and designing solutions, seeing
          each project as an opportunity to bring ideas to life through code.
          Maria's goal is to join a forward-thinking company where she can apply
          her skills, contribute to projects, and be apart of a great
          team. With her enthusiasm for learning and her ability to meet
          deadlines, Maria is poised to make significant contributions to the
          tech industry. Her journey from curious beginner to dedicated coder
          exemplifies her determination, adaptability, and team work that makes
          her an asset to any development team. 
        </p>
       <img src="C:\Users\lines\Downloads\Maria.jpg" 
       alt="Maria" 
       width="300" 
       height="200">

    
>
      </section>

      <section id="projects">
        <h2>My Projects</h2>
        <div class="project-grid">
          <div class="project-item">
            <div class="project-description">
              <h3>Project 1</h3>
              <p>This was my very first page. This is the project that made me believe that it is possible to actually become a Software Developer. I decided to do my page about one of my favorite authors Rick Smith. This page was created with CSS, HTML and JavaScript. The background is a nice blue to purple gradient. The book cover was centered, theres a brief decription under it, links to his website were placed under the decription and a basic button was added to the bottom.</p>
            </div>
            <div class="project-image">
              <img src="C:\Users\lines\Downloads\Rick Smith Page.jpg" 
              alt="RickSmith.jpeg" 
              />
            </div>
          </div>

          <div class="project-item">
            <div class="project-description">
              <h3>Project 2</h3>
              <p>This R&B music page was created with CSS, HTML, and Javascript. The background is a dark blue with a orange 2 color circle. The container is a beautiful caramel brown. The Michael Jackson picture was wrapped as link to his concert in Bucarest on Youtube.</p>
            </div>
            <div class="project-image">
              <img src="C:\Users\lines\Downloads\RnB Music.jpg" 
              alt="RnB Music.jpeg" />
            </div>
          </div>

          <div class="project-item">
            <div class="project-description">
              <h3>Project 3</h3>
              <p>This advanced clock was created with javacript, CSS, React and Responsive. I put the background color as powder blue to white. I gave the container a ocean scene with blue split.</p>
            </div>
            <div class="project-image">
              <img src="C:\Users\lines\Downloads\advanced weather app.jpg" 
              alt="advanced weather app" />
            </div>
          </div>

          <div class="project-item">
            <div class="project-description">
              <h3>Project 4</h3>
              <p>This AI project gives funny jokes about computers when clicked. The machine was created with CSS, HTML, Javacript and AI joke creations. The container is a white color. The background color is a gradient soft pink to yellow, and I gave the button a beautiful chocolate color. </p>
            </div>
            <div class="project-image">
              <img src="C:\Users\lines\Downloads\joke machine.jpg"
              alt="jokemachine.jpeg" />
           </div>
           </div>

          <div class="project-item">
            <div class="project-description">
                <h3>Project 5</h3>
                <p>This world ckock has six places with accurate world time. The clock was made with HTML, CSS, Div Class and Javascript. I put a soft green Gradient color for the back ground and gave the container a soft white color</p>
            </div>
                <div class="project image">
                <img src="C:\Users\lines\Downloads\world clock.jpg" 
                alt="world clock"/>
           </div>
           </div>
            </div>
          </div>
        </div>
      </section>
    </main>

    <footer>
      <p>
        Contact:
        <a href="mailto:marieloparis@gmail.com" target="_blank">marieloparis</a>
      </p>
      <p>
        GitHub:
        <a href="https://github.com/Marie-313/monica3/blob/main/monica3" target="_blank">monica3</a>
      </p>
      <p>
        Vercel:
        <a href="" target="_blank"
          >marie-313</a
        >
      </p>
    </footer>

    <script>
      function showSection(sectionId) {
        const sections = document.querySelectorAll("section");
        sections.forEach((section) => {
          section.classList.remove("active");
        });
        const activeSection = document.getElementById(sectionId);
        if (activeSection) {
          activeSection.classList.add("active");
        }
      }
    </script>
  </body>
</html>
