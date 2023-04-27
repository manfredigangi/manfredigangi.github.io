<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>Mayara Riss - Front-End Developer</title>
    <link rel="stylesheet" href="style.css">
  </head>
  <body>
    <header>
      <nav>
        <a href="#about">About</a>
        <a href="#work">Work</a>
        <a href="#contact">Contact</a>
      </nav>
      <h1>Mayara Riss</h1>
      <h2>Front-End Developer</h2>
    </header>
    <main>
      <section id="about">
        <h3>About Me</h3>
        <p>Hi there! My name is Mayara Riss and I am a front-end developer with over 5 years of experience. I have worked on a variety of projects, from small static websites to large-scale web applications. I love using HTML, CSS, and JavaScript to create beautiful, responsive, and user-friendly websites that help businesses achieve their goals.</p>
        <p>When I'm not coding, I enjoy hiking, reading, and spending time with my family and pets.</p>
      </section>
      <section id="work">
        <h3>My Work</h3>
        <div class="project">
          <img src="project-1.jpg" alt="Project 1">
          <h4>Project 1</h4>
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus mattis enim et ante volutpat, non accumsan enim vulputate.</p>
          <a href="#">Learn More</a>
        </div>
        <div class="project">
          <img src="project-2.jpg" alt="Project 2">
          <h4>Project 2</h4>
          <p>Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium.</p>
          <a href="#">Learn More</a>
        </div>
        <div class="project">
          <img src="project-3.jpg" alt="Project 3">
          <h4>Project 3</h4>
          <p>Nam sit amet quam vitae neque dignissim tincidunt. Nullam et nisl ut mi commodo suscipit.</p>
          <a href="#">Learn More</a>
        </div>
      </section>
      <section id="contact">
        <h3>Contact Me</h3>
        <form>
          <label for="name">Name:</label>
          <input type="text" id="name" name="name" required>
          <label for="email">Email:</label>
          <input type="email" id="email" name="email" required>
          <label for="message">Message:</label>
          <textarea id="message" name="message" required></textarea>
          <button type="submit">Send</button>
        </form>
      </section>
    </main>
    <footer>
      <p>&copy; 2023 Mayara Riss. All rights reserved.</p>
    </footer>
    <script src="script.js"></script>
  </body>
</html>
