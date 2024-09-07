<script>
    var toDayFromNow =
      new Date("Sep 09, 2024 23:59:59").getTime() / 1000 +
      3600 / 60 / 60 / 24 -
      1;
    const initializeFlip = () => {
      new FlipDown(toDayFromNow, {
        theme: "light",
      }).start();
    };
</script>



<svelte:head>
  <link
    href="https://pbutcher.uk/flipdown/css/flipdown/flipdown.css"
    rel="stylesheet"
  />
  <script
    src="https://pbutcher.uk/flipdown/js/flipdown/flipdown.js"
    onload={initializeFlip}
  ></script>
</svelte:head>

<main >
    <h1 class="unselectable">
      <span class="payverge">payverge</span> <br /> coming soon
    </h1>
  
    <div id="flipdown" class="flipdown"></div>
  </main>
  
  <footer>
    <div class="socials unselectable">
      <a id="pseudelink-to-facebook"
        ><span class="icon facebook-icon"
          ><i class="fab fa-facebook-square"></i></span
        ></a
      >
      <a id="pseudelink-to-pinterest"
        ><span class="icon pinterest-icon"><i class="fab fa-pinterest"></i></span
        ></a
      >
      <a id="pseudelink-to-instagram"
        ><span class="icon instagram-icon"><i class="fab fa-instagram"></i></span
        ></a
      >
    </div>
  </footer>





  <style>
    @import url("https://fonts.googleapis.com/css2?family=Red+Hat+Text:wght@700&display=swap");
  
    :global(:root) {
      --grayish-blue: hsl(237, 18%, 59%);
      --soft-red: hsl(345, 95%, 68%);
      --white: hsl(0, 0%, 100%);
      --dark-blue: hsl(236, 21%, 26%);
      --darker-blue: hsl(235, 16%, 14%);
      --darkest-blue: hsl(234, 17%, 12%);
      font-size: 14px;
      font-family: "Red Hat Text", sans-serif;
      font-weight: 700;
    }
  
    :global(html) {
      margin: 0;
      text-align: center;
      height: 100%;
      overflow: hidden;
      background-color: var(--darker-blue);
      background-image: url(bg-stars.svg);
      background-image: url(bg-stars.svg),
        linear-gradient(var(--darkest-blue), var(--darker-blue));
    }
    :global(body > *) {
      position: relative;
    }
  
    main {
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      /* border: 10px solid red; */
      /* margin-top: 5em; */
      height: 70vh;
      gap: 4rem;
      /* padding: 20px; */
    }
  
    h1 {
      top: 20vh;
      color: var(--white);
      font-size: 18px;
      letter-spacing: 0.3em;
      text-transform: uppercase;
    }
  
    .flipdown {
      width: fit-content;
    }
  
    footer {
      background-image: url(pattern-hills.svg);
      background-repeat: no-repeat;
      background-position-y: top;
      background-position-x: 80%;
      background-size: cover;
      width: 100%;
      height: 26vh;
      bottom: 0;
      position: absolute;
      vertical-align: middle;
    }
  
    .socials {
      font-size: 28px;
      color: var(--grayish-blue);
      text-align: center;
      bottom: 5vh;
      position: absolute;
      width: 100%;
    }
  
    .socials a {
      margin: 0 0.5em 0 0.5em;
      transition: color 0.2s ease-in-out;
    }
  
    .socials a:hover {
      color: var(--soft-red);
    }
    .payverge {
      color: tomato;
      font-size: 5rem;
      text-transform: lowercase;
    }
  
    @media only screen and (max-width: 600px) {
      :root {
        font-size: 8px;
      }
    }
  </style>