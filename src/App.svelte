<script>
  export let name;
</script>

<div class="wrapper">
  <div class="floating-spaceship-wrapper">
    <div class="floating-spaceship">{name}</div>
  </div>
  <h1>Musikk</h1>
  <div class="releases">
    <div class="release">
      <a
        href="https://open.spotify.com/album/7rmzPefl4J4BmEhnz51nY3"
        class="cover-link"
        rel="noopener noreferrer"
        target="_blank"
      >
        <img
          src="https://i1.sndcdn.com/artworks-SM3C4SGPruyWAyOL-zZZREg-t500x500.jpg"
          alt="natteting"
          class="cover"
        />
      </a>
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
  <h1>Video</h1>
  <div class="release">
    <iframe
      title="Kjør Romskip – gnist"
      class="youtube"
      width="560"
      height="315"
      src="https://www.youtube-nocookie.com/embed/qOg_ieDhuS4"
      frameborder="0"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
      allowfullscreen
    />
    gnist (musikkvideo)
  </div>
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
  <div class="buy-vinyl-section">
    <h1>Kjøp vinyl!</h1>
    <em>natteting</em> finnes i begrenset opplag på vinyl. Fysen? Da kan du
    <a href="https://merchsjappa.no/artist/kjoer-romskip/" target="_blank"
      >kjøpe den i Merchsjappa</a
    >
    eller på neste konsert.
    <br />
    <br />
    <a
      href="https://merchsjappa.no/artist/kjoer-romskip/"
      target="_blank"
      class="primary">Gå til Merchsjappa</a
    >
  </div>
  <div>
    <h1>Konserter</h1>
    <a
      href="https://www.songkick.com/artists/10064686"
      class="songkick-widget"
      data-theme="dark"
      data-track-button="on"
      data-detect-style="off"
      data-background-color="rgb(0,0,0,1)"
      data-font-color="rgb(255,255,255,1)"
      data-button-bg-color="rgb(255,255,255,1)"
      data-button-text-color="rgb(0,0,0,1)"
      data-locale="en"
      data-other-artists="on"
      data-share-button="on"
      data-country-filter="on"
      data-rsvp="on"
      data-request-show="on"
      data-past-events="off"
      data-past-events-offtour="off"
      data-remind-me="off"
      style="display: none;">Songkick</a
    >
  </div>
  <div class="contact">
    <h1>Kontakt</h1>
    <a href="mailto:kjor.romskip@gmail.com">kjor.romskip@gmail.com</a>
  </div>
</div>

<style>
  a,
  a:active,
  a:visited {
    color: #272352;
    border-bottom: 2px solid #272352;
  }

  a:hover {
    text-decoration: none;
    background-color: #272352;
    color: white;
    transition:
      background-color 0.3s ease-in-out,
      color 0.3s ease-in-out;
  }

  .wrapper {
    display: grid;
    justify-content: center;
    align-items: center;
    gap: 2rem;
    padding: 5rem 0;
  }

  .floating-spaceship-wrapper {
    transform: scaleX(-1);
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
    transition:
      filter 1s ease-in-out,
      transform 0.3s ease-in-out,
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
    gap: 1rem;
  }

  .primary {
    padding: 12px 16px;
    display: block;
    width: fit-content;
    border-radius: 4px;
    box-shadow: -3px 3px 0px 0px rgba(0, 0, 0, 0.7);
    background-color: #f6d052;
    color: black;
    transition:
      color 0.3s ease-in-out,
      background-color 0.3s ease-in-out;
    text-decoration: none;
    margin: auto;
  }
  .primary:hover {
    background-color: #3f3e7a;
    color: white;
  }

  @media only screen and (min-width: 768px) {
    .primary {
      margin: 0;
    }
  }

  @keyframes move-around {
    0% {
      transform: translate(0, 0) rotate(0);
    }
    10% {
      transform: translate(80px, -80px) rotate(0);
    }
    25% {
      transform: translate(70px, 0) rotate(90deg);
    }
    50% {
      transform: translate(120px, 100px) rotate(30deg);
    }
    55% {
      transform: translate(140px, 120px) rotate(70deg);
    }
    75% {
      transform: translate(50px, 300px) rotate(-170deg);
    }
    90% {
      transform: translate(20px, 50px) rotate(270deg);
    }
    100% {
      transform: translate(0, 0) rotate(-360deg);
    }
  }
</style>
