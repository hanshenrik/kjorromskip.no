<script>
  export let name;
</script>

<div class="wrapper">
  <div class="release">
    <iframe
      title="Kjør Romskip – Romturist"
      class="youtube"
      width="560"
      height="315"
      src="https://www.youtube-nocookie.com/embed/-GzNoOeA7ho"
      frameborder="0"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
      allowfullscreen
    />
    Romturist (musikkvideo)
  </div>
  <div class="floating-spaceship">{name}</div>
  <h1>Musikk</h1>
  <div class="releases">
    <div class="release">
      <!-- <a
        href="https://open.spotify.com/track/7rmzPefl4J4BmEhnz51nY3"
        class="cover-link"
        rel="noopener noreferrer"
        target="_blank"
      > -->
      <img
        src="https://i1.sndcdn.com/artworks-SM3C4SGPruyWAyOL-zZZREg-t500x500.jpg"
        alt="natteting"
        class="cover"
      />
      <!-- </a> -->
      natteting (album)
    </div>
    <div class="release">
      <a
        href="https://open.spotify.com/track/3qs27OFo6B9Lqc0GPPbO1v?si=5277caceac044e65"
        class="cover-link"
        rel="noopener noreferrer"
        target="_blank"
      >
        <img
          src="https://i1.sndcdn.com/artworks-5qC0wHTkn8GHAWBg-KgbP0g-t500x500.jpg"
          alt="oslo gigolo"
          class="cover"
        />
      </a>
      oslo gigolo (singel)
    </div>
    <div class="release">
      <a
        href="https://open.spotify.com/track/25p9haFiESoTwbjdQWKplu?si=c3e5c7ce1794477d"
        class="cover-link"
        rel="noopener noreferrer"
        target="_blank"
      >
        <img
          src="https://i1.sndcdn.com/artworks-rjAKbKgxRT3NSpcG-5OQ9JQ-t500x500.jpg"
          alt="mr rino"
          class="cover"
        />
      </a>
      mr rino (singel)
    </div>
    <div class="release">
      <a
        href="https://open.spotify.com/album/10qT4ktbWSHt0l8gLwO65f?si=DMkFo0BqQgqYjJ9aVYUQ3A"
        class="cover-link"
        rel="noopener noreferrer"
        target="_blank"
      >
        <img
          src="https://i1.sndcdn.com/artworks-rb5N8WJKUzH34n3f-0tMdjA-t500x500.jpg"
          alt="Chili Cheese / Premadonna"
          class="cover"
        />
      </a>
      Chili Cheese / Premadonna (dobbelsingel)
    </div>
    <div class="release">
      <a
        href="https://open.spotify.com/track/0ftuszDppBh03LyyoUZwO8?si=e01f34bd13c840b4"
        class="cover-link"
        rel="noopener noreferrer"
        target="_blank"
      >
        <img
          src="https://i1.sndcdn.com/artworks-000572129276-8kpg9o-t500x500.jpg"
          alt="Romturist"
          class="cover"
        />
      </a>
      Romturist (singel)
    </div>
  </div>
  <div class="contact">
    <h1>Kontakt</h1>
    <a href="mailto:kjor.romskip@gmail.com">kjor.romskip@gmail.com</a>
  </div>
</div>

<style>
  .wrapper {
    display: grid;
    justify-content: center;
    align-items: center;
    justify-items: center;
    gap: 2rem;
    padding: 5rem 0;
  }

  .floating-spaceship {
    text-align: center;
    animation-name: move-around;
    animation-delay: 1s;
    animation-duration: 20s;
    animation-timing-function: ease-in-out;
    animation-iteration-count: infinite;
    font-size: 4rem;
  }

  .youtube,
  .cover {
    border-radius: 4px;
    box-shadow: -6px 6px 0px 0px rgba(0, 0, 0, 0.7);
  }

  .cover {
    width: 100%;
    max-width: 375px;
  }

  .youtube {
    max-width: 100%;
    height: 171px;
  }

  @media only screen and (min-width: 375px) {
    .youtube {
      height: 202px;
    }
  }

  @media only screen and (min-width: 414px) {
    .youtube {
      height: 224px;
    }
  }

  @media only screen and (min-width: 768px) {
    .youtube {
      height: 315px;
    }
  }

  .cover-link .cover {
    transition: filter 1s ease-in-out, transform 0.3s ease-in-out,
      box-shadow 0.3s ease-in-out;
  }
  .cover-link:hover .cover {
    filter: hue-rotate(180deg);
    box-shadow: -10px 10px 0px 0px rgba(0, 0, 0, 0.7);
    transform: translate(4px, -4px);
  }

  .releases {
    display: grid;
    grid-template-columns: 1fr;
    justify-items: center;
    gap: 2rem;
  }
  @media only screen and (min-width: 768px) {
    .releases {
      grid-template-columns: 1fr 1fr;
    }
  }

  .release {
    display: grid;
    justify-items: center;
    gap: 1rem;
  }

  .contact {
    text-align: center;
    font-size: 0.8rem;
  }

  @keyframes move-around {
    0% {
      transform: translate(0, 0) rotate(0);
    }
    10% {
      transform: translate(100px, -100px) rotate(0);
    }
    25% {
      transform: translate(70px, 0) rotate(90deg);
    }
    50% {
      transform: translate(150px, 100px) rotate(30deg);
    }
    55% {
      transform: translate(200px, 100px) rotate(70deg);
    }
    75% {
      transform: translate(50px, 300px) rotate(-170deg);
    }
    90% {
      transform: translate(0, 50px) rotate(270deg);
    }
    100% {
      transform: translate(0, 0) rotate(-360deg);
    }
  }
</style>
