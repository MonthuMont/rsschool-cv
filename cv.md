# MonthuMont CV.

- Name
  - Arseny Sofronov
- Contacts
  - Email: insaine33@gmail.com
  - discord: **ID**-347068197410701322      **userName**-month3f4ck3r

## Brief information about me

I'm 18 years old student and at the age of 17, I started thinking about my future and what I really want to do. The field of IT technologies impressed me very much when I started preparing for computer science exams at school. At that moment I realized that I was really interested in doing this. After graduating from school, for some reason I entered the university at the Faculty of Mechanics and Mathematics, which made me even more aware that I was not doing what I liked. I want to connect my life with work in IT, despite the difficult and thorny path that everyone who wants to become a high-level specialist will have to go through. For me, this is a very important goal that I think about every day.


## My skills

I know basic Html, css, javascript

- HTML
  - BEM Methodology

* Css
  - pseudo elements/pseudo - classes
  - scss
  - basic adaptive
* JS
  - basic work with DOM
### Example of modal window

```html
<!DOCTYPE html>
<html lang="ru">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>modalWindow</title>
    <link rel="stylesheet" href="./style.css" />
  </head>
  <body>
    <main class="main">
      <div class="container">
        <div class="modalBlocks">
          <button class="modalBlocks__block window1">
            <span class="text">Модальное окно 1</span>
          </button>
          <button class="modalBlocks__block window2">
            <span class="text">Модальное окно 2</span>
          </button>
          <button class="modalBlocks__block window3">
            <span class="text">Модальное окно 3</span>
          </button>
        </div>
        <div class="modal-window hidden">
          <button class="close-modal-window">&times;</button>
          <h1 class="title">Модальное окно 1</h1>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Quam harum
            voluptatem consequatur? Vero nesciunt sunt, quos facere, quam enim
            numquam unde doloremque saepe ab alias iusto animi adipisci, ratione
            sint?Lorem ipsum dolor sit amet consectetur adipisicing elit.
            Veniam, incidunt nobis maxime temporibus fuga cupiditate eos
            deleniti quam aut impedit exercitationem minus in modi perferendis
            quia, voluptas suscipit iusto non!
          </p>
        </div>
        <div class="modal-window hidden">
          <button class="close-modal-window">&times;</button>
          <h1 class="title">Модальное окно 2</h1>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Quam harum
            voluptatem consequatur? Vero nesciunt sunt, quos facere, quam enim
            numquam unde doloremque saepe ab alias iusto animi adipisci, ratione
            sint?Lorem ipsum dolor sit amet consectetur adipisicing elit.
            Veniam, incidunt nobis maxime temporibus fuga cupiditate eos
            deleniti quam aut impedit exercitationem minus in modi perferendis
            quia, voluptas suscipit iusto non!
          </p>
        </div>
        <div class="modal-window hidden">
          <button class="close-modal-window">&times;</button>
          <h1 class="title">Модальное окно 3</h1>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Quam harum
            voluptatem consequatur? Vero nesciunt sunt, quos facere, quam enim
            numquam unde doloremque saepe ab alias iusto animi adipisci, ratione
            sint?Lorem ipsum dolor sit amet consectetur adipisicing elit.
            Veniam, incidunt nobis maxime temporibus fuga cupiditate eos
            deleniti quam aut impedit exercitationem minus in modi perferendis
            quia, voluptas suscipit iusto non!
          </p>
        </div>
      </div>
      <div class="overlay hidden"></div>
    </main>
    <script src="./script.js"></script>
  </body>
</html>
```

```css
*,
*::before,
*::after {
  margin: 0;
  padding: 0;
  border: 0;
  box-sizing: border-box;
}
li {
  list-style: none;
}
ul {
  margin: 0;
  padding: 0;
  list-style: none;
}
a,
a:visited {
  text-decoration: none;
}
a:hover {
  text-decoration: none;
}
h1,
h2,
h3,
h4,
h5,
h6 {
  font-weight: inherit;
  font-size: inherit;
}
img {
  vertical-align: top;
  max-width: 100%;
}
html,
body {
  height: 100%;
}
html {
  font-size: 16px; /* по умолчанию */
}
body {
  line-height: 1;
}
.wrapper {
  min-height: 100%;
  overflow: hidden;
}
.container {
  max-width: 1130px;
  padding: 0px 15px;
  margin: 0 auto;
}
.text {
  padding: 20px 30px;
  border-radius: 10px;
  background: linear-gradient(21deg, #dd03e4, #5611ec);
}
.modalBlocks {
  padding: 70px 0px;
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
}
.modalBlocks__block {
  transition-duration: 0.2s;
}
.modalBlocks__block:hover {
  transform: scale(1.1);

  text-decoration: none;
  cursor: pointer;
}
body {
  background: linear-gradient(90deg, #aea4e3, #d3ffe8);
}
.hidden {
  display: none;
}
.modal-window {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 70%;
  background-color: white;
  padding: 6rem;
  border-radius: 5px;
  box-shadow: 0 3rem 5rem rgba(0, 0, 0, 0.3);
  z-index: 10;
}
.overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.5);
  backdrop-filter: blur(3px);
  z-index: 5;
}
.close-modal-window {
  position: absolute;
  top: 1.2rem;
  right: 2rem;
  font-size: 5rem;
  color: #444;
  cursor: pointer;
  border: none;
  background: none;
}
.title {
  font-weight: bold;
  font-size: 20px;
  padding-bottom: 20px;
}
```


```javascript
"use strict";
const modalWindow = document.querySelectorAll(".modal-window");
const overlay = document.querySelector(".overlay");
const btnCloseModalWindow = document.querySelectorAll(".close-modal-window");
const btnShowModalWindow = document.querySelectorAll(".modalBlocks__block");
// console.log(btnShowModalWindow);
for (let i = 0; i < btnShowModalWindow.length; i++) {
  btnShowModalWindow[i].addEventListener("click", function () {
    modalWindow[i].classList.remove("hidden");
    overlay.classList.remove("hidden");
  });
  let closeModalWindow = function () {
    modalWindow[i].classList.add("hidden");
    overlay.classList.add("hidden");
  };
  btnCloseModalWindow[i].addEventListener("click", closeModalWindow);
  overlay.addEventListener("click", closeModalWindow);
  document.addEventListener("keydown", function (e) {
    if (e.key === "Escape" && !modalWindow[i].classList.contains("hidden")) {
      closeModalWindow();
    }
  });
}
```
## Work experience
I have not any work experience.
I started studying two months ago and I am still studying.
Here is my JS  [project]( https://monthumont.github.io/diceGame/) 
## Education
I take all the information from open free sources, I didn't sign up for any courses because it costs a lot of money.
## English knowledge
My english knowledge is pre-intermediate. 
I have a language barrier to speak, but at the same time I understand the language quite well by ear. I think that with full immersion in the English-speaking community, I will be able to adapt.