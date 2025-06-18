
<style>
  #draggable-panel {
    width: 300px;
    height: 180px;
    position: absolute;
    top: 50px;
    left: 50px;
    background-color: #111;
    border-radius: 10px;
    box-shadow: 0 0 10px #00f7c1;
    padding: 10px;
    cursor: grab;
  }

  #draggable-panel img {
    width: 100%;
  }
</style>

<div id="draggable-panel">
  <img src="https://github-readme-stats.vercel.app/api?username=TU-USUARIO&theme=tokyonight&show_icons=true" />
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

<h1 align="center">Hey there <img src="https://raw.githubusercontent.com/MartinHeinz/MartinHeinz/master/wave.gif" width="30px"/> I'm Amor</h1>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&duration=2000&pause=1000&color=00F7C1&center=true&vCenter=true&width=435&lines=Backend+Engineer+%7C+Node.js+%26+NestJS;Hexagonal+Architecture+%7C+Clean+Code;PostgreSQL+%7C+Redis+%7C+Docker+%7C+CI%2FCD;Always+debugging+with+coffee+%E2%98%95%EF%B8%8F" alt="Typing SVG" />
</p>

---

## 👨‍💻 About Me

- 🧠 Backend-only Developer (Frontend? no, gracias)
- ⚙️ Specializing in **NestJS**, **Node.js**, **PostgreSQL**, **Redis**, **Docker**
- 🧱 Fanático de la **arquitectura hexagonal** y el código limpio
- 📈 Experiencia construyendo APIs escalables y mantenibles desde **2020**
- ☁️ Automatización: CI/CD, testing, documentación
- 🚫 CSS-free zone. Solo back, con amor y excepciones bien lanzadas.

---

## 🧰 Tech Stack

<img align="right" src="https://media.tenor.com/qJ5evVs-_uUAAAAC/coding.gif" width="200"/>

### 🖥️ Core Backend

<div>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nodejs/nodejs-original.svg" width="40"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nestjs/nestjs-plain.svg" width="40"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/express/express-original.svg" width="40"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/socketio/socketio-original.svg" width="40"/>
</div>

### 🛢️ Databases

<div>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/postgresql/postgresql-original.svg" width="40"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/mongodb/mongodb-original.svg" width="40"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/mysql/mysql-original.svg" width="40"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/firebase/firebase-plain.svg" width="40"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/redis/redis-original.svg" width="40"/>
</div>

### ⚙️ DevOps & Tools

<div>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/docker/docker-original.svg" width="40"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-original.svg" width="40"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/github/github-original.svg" width="40"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/npm/npm-original-wordmark.svg" width="40"/>
</div>

---

## 📊 GitHub Stats

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=TU-USUARIO&theme=tokyonight&show_icons=true&hide_border=false&count_private=true" height="150" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=TU-USUARIO&theme=tokyonight&layout=compact&hide_border=false" height="150" />
</div>

---

## 🗂️ Architecture & Philosophy

- 🧱 Hexagonal Architecture
- 🧼 Clean Code & SOLID Principles
- 💡 CQRS when needed, pragmatism always
- 🧪 Unit & E2E Testing
- 💬 *“Si no lanza excepciones claras, no es backend serio.”*

---

## 📫 Contact

- 📧 Email: `tu-correo@ejemplo.dev`
- 🐙 GitHub: [@tu-usuario](https://github.com/tu-usuario)

---

<sub>Last Updated: 18/06/2025</sub>
