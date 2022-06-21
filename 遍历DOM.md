<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta http-equiv="X-UA-Compatible" content="ie=edge" />
    <link rel="shortcut icon" type="image/png" href="img/icon.png" />

    <link
      href="https://fonts.googleapis.com/css?family=Poppins:300,400,500,600&display=swap"
      rel="stylesheet"
    />
    <link rel="stylesheet" href="style.css" />
    <title>Bankist | When Banking meets Minimalist</title>
    <style>
      .header__title {
        flex: 1;

        max-width: 115rem;
        display: grid;
        grid-template-columns: 3fr 2fr;
        row-gap: 3rem;
        align-content: center;
        justify-content: center;

        align-items: start;
        justify-items: start;
      }

      h1 {
        font-size: 5.5rem;
        line-height: 1.35;
      }

      h4 {
        font-size: 2.4rem;
        font-weight: 500;
      }

      .header__img {
        width: 100%;
        grid-column: 2 / 3;
        grid-row: 1 / span 4;
        transform: translateY(-6rem);
      }

      .highlight {
        position: relative;
      }
    </style>
  </head>
  <body>
    <header class="header">
      <div class="header__title">
        <h1>
          When
          <!-- Green highlight effect -->
          <span class="highlight">banking</span>
          meets<br />
          <span class="highlight">minimalist</span>
        </h1>
        <h4>A simpler banking experience for a simpler life.</h4>
      </div>
    </header>
  </body>
  <script type="text/javascript">
    const h1 = document.querySelector("h1");
    console.log(h1.innerHTML);

    //going downwards: child
    console.log(h1.querySelectorAll(".highlight"));
    //going downwards
    //console.log(h1.querySelector());
    console.log(h1.children); //get all direct children of h1

    //get first child
    h1.firstElementChild.style.color = "red";

    //get last child
    h1.lastElementChild.style.color = "blue";

    //going upwards: parents
    console.log(h1.parentNode); //dirct parent Node
    console.log(h1.parentElement); //dirct parent element

    //select closest needed parent element
    h1.closest(".header").style.background = "var(--gradient-secondary)";

    //will return itself
    h1.closest("h1").style.background = "var(--gradient-secondary)";

    //goding sideways: siblings
    //element
    console.log(h1.previousElementSibling);
    console.log(h1.nextElementSibling);

    //node
    console.log(h1.previousSibling);
    console.log(h1.nextSibling);

    //get parent's all children
    console.log(h1.parentElement.children); //return a iterable type

    [...h1.parentElement.children].forEach(function (el) {
      if (el !== h1) el.style.transform = "scale(0.5)";
    });
  </script>
</html>
