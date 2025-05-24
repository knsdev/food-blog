<style>
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Arial, Helvetica, sans-serif;
  }

  h1 {
    margin: 2rem;
  }

  img {
    width: 100%;
    object-fit: contain;
    border-radius: 0.5rem;
    border: 3px solid black;
  }

  .container {
    display: grid;
    grid-template-columns: 2fr 1fr;
    grid-template-rows: repeat(4, 12rem);
    grid-auto-rows: 12rem;
    gap: 1rem;
    margin: 2rem;
    max-width: 1200px;

    .desktop-container {
      display: flex;
      flex-flow: column nowrap;
      justify-content: flex-start;
      align-items: center;
      gap: 0.5rem;
    }
  }

  #index {
    grid-column: 1 / 2;
    grid-row: 1 / 2;
  }

  #about {
    grid-column: 1 / 2;
    grid-row: 2 / 3;
  }

  #recipe-desktop {
    grid-column: 1 / 2;
    grid-row: 3 / 4;
  }

  #recipe-mobile {
    grid-column: 2 / 3;
    grid-row: 1 / 4;
  }
</style>

<h1>Food blog</h1>

<div class="container">
  <div class="desktop-container">
    <div id="index"><img src="./screenshots/index.jpg" alt="" /></div>
    <div id="recipe-desktop"><img src="./screenshots/recipe-of-the-month-desktop.jpg" alt="" /></div>
    <div id="about"><img src="./screenshots/about.jpg" alt="" /></div>
  </div>
  <div id="recipe-mobile"><img src="./screenshots/recipe-of-the-month-mobile.png" alt="" /></div>
</div>
