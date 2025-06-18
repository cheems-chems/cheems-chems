<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <title>Amor - Backend Dev</title>
    <style>
      body {
        background-color: #0f1117;
        color: #eee;
        font-family: 'Fira Code', monospace;
        padding: 2rem;
      }

      h1 {
        text-align: center;
      }

      #draggable-panel {
        width: 340px;
        height: 180px;
        position: absolute;
        top: 60px;
        left: 60px;
        background-color: #111;
        border-radius: 10px;
        box-shadow: 0 0 10px #00f7c1;
        padding: 10px;
        cursor: grab;
        z-index: 10;
      }

      #draggable-panel img {
        width: 100%;
        height: auto;
      }

      .section {
        margin-top: 40px;
      }

      .tech-stack img {
        margin-right: 10px;
      }

      .center {
        text-align: center;
      }

      .typing {
        display: flex;
        justify-content: center;
        margin-bottom: 30px;
      }

      .gif-right {
        float: right;
        margin-left: 20px;
      }
    </style>
  </head>
  <body>
    <h1>
      Hey there
      <img
        src="https://raw.githubusercontent.com/MartinHeinz/MartinHeinz/master/wave.gif"
        width="30px"
      />
      I'm Amor
    </h1>

    <div class="typing">
      <img
        src="https://readme-typing-svg.demolab.com?font=Fira+Code&duration=2000&pause=1000&color=00F7C1&center=true&vCenter=true&width=435&lines=Backend+Engineer+%7C+Node.js+%26+NestJS;Hexagonal+Architecture+%7C+Clean+Code;PostgreSQL+%7C+Redis+%7C+Docker+%7C+CI%2FCD;Always+debugging+with+coffee+%E2%98%95%EF%B8%8F"
        alt="Typing"
      />
    </div>

    <div class="section">
      <h2>👨‍💻 About Me</h2>
      <ul>
        <li>🧠 Backend-only Developer (Frontend? no, gracias)</li>
        <li>⚙️ Especializado en <strong>NestJS</strong>, <strong>Node.js</strong>, <strong>PostgreSQL</strong>, <strong>Redis</strong>, <strong>Docker</strong></li>
        <li>🧱 Fanático de la <strong>arquitectura hexagonal</strong> y el código limpio</li>
        <li>📈 Experiencia construyendo APIs escalables y mantenibles desde <strong>2020</strong></li>
        <li>☁️ Automatización: CI/CD, testing, documentación</li>
        <li>🚫 CSS-free zone. Solo back, con amor y excepciones bien lanzadas.</li>
      </ul>
    </div>

    <div class="section">
      <h2>🧰 Tech Stack</h2>
      <img class="gif-right" src="https://media.tenor.com/qJ5evVs-_uUAAAAC/coding.gif" width="200" />
      <h3>🖥️ Core Backend</h3>
      <div class="tech-stack">
        <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nodejs/nodejs-original.svg" width="40" />
        <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nestjs/nestjs-plain.svg" width="40" />
        <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/express/express-original.svg" width="40" />
        <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/socketio/socketio-original.svg" width="40" />
      </div>

      <h3>🛢️ Databases</h3>
      <div class="tech-stack">
        <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/postgresql/postgresql-original.svg" width="40" />
        <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/mongodb/mongodb-original.svg" width="40" />
        <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/mysql/mysql-original.svg" width="40" />
        <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/firebase/firebase-plain.svg" width="40" />
        <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/redis/redis-original.svg" width="40" />
      </div>

      <h3>⚙️ DevOps & Tools</h3>
      <div class="tech-stack">
        <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/docker/docker-original.svg" width="40" />
        <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-original.svg" width="40" />
        <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/github/github-original.svg" width="40" />
        <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/npm/npm-original-wordmark.svg" width="40" />
      </div>
    </div>

    <div class="section center">
      <h2>📊 GitHub Stats</h2>
      <img
        src="https://github-readme-stats.vercel.app/api?username=amor-dev&theme=tokyonight&show_icons=true&hide_border=false&count_private=true"
        height="150"
      />
      <img
        src="https://github-readme-stats.vercel.app/api/top-langs/?username=amor-dev&theme=tokyonight&layout=compact&hide_border=false"
        height="150"
      />
    </div>

    <div class="section">
      <h2>🗂️ Architecture & Philosophy</h2>
      <ul>
        <li>🧱 Hexagonal Architecture</li>
        <li>🧼 Clean Code & SOLID Principles</li>
        <li>💡 CQRS when needed, pragmatism always</li>
        <li>🧪 Unit & E2E Testing</li>
        <li>💬 “Si no lanza excepciones claras, no es backend serio.”</li>
      </ul>
    </div>

    <div class="section">
      <h2>📫 Contact</h2>
      <ul>
        <li>📧 Email: <code>tu-correo@ejemplo.dev</code></li>
        <li>🐙 GitHub: <a href="https://github.com/amor-dev">@amor-dev</a></li>
      </ul>
    </div>

    <div id="draggable-panel">
      <img
        src="https://github-readme-stats.vercel.app/api?username=amor-dev&theme=tokyonight&show_icons=true"
        alt="GitHub Stats Floating"
      />
    </div>

    <script>
      const panel = document.getElementById('draggable-panel');
      let isDragging = false;
      let offsetX, offsetY;

      panel.addEventListener('mousedown', (e) => {
        isDragging = true;
        offsetX = e.clientX - panel.offsetLeft;
        offsetY = e.clientY - panel.offsetTop;
        panel.style.cursor = 'grabbing';
      });

      document.addEventListener('mousemove', (e) => {
        if (!isDragging) return;
        panel.style.left = `${e.clientX - offsetX}px`;
        panel.style.top = `${e.clientY - offsetY}px`;
      });

      document.addEventListener('mouseup', () => {
        isDragging = false;
        panel.style.cursor = 'grab';
      });
    </script>
  </body>
</html>
