<script>
  export let name;
</script>

<div class="wrapper">
  <div class="release">
    <iframe
      title="Kjør Romskip – Romturist"
      class="cover"
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
    Chili Cheese / Premadonna
  </div>
</div>

<style>
  .wrapper {
    display: grid;
    justify-content: center;
    align-items: center;
    justify-items: center;
    gap: 2rem;
    height: 100%;
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

  .cover {
    height: 171px;
    max-width: 100%;
    border-radius: 4px;
    box-shadow: 0 0 16px 2px rgba(0, 0, 0, 0.5);
  }

  @media only screen and (min-width: 375px) {
    .cover {
      height: 202px;
    }
  }

  @media only screen and (min-width: 414px) {
    .cover {
      height: 224px;
    }
  }

  @media only screen and (min-width: 768px) {
    .cover {
      height: 315px;
    }
  }

  .cover-link .cover {
    transition: filter 0.6s ease-in-out;
  }
  .cover-link:hover .cover {
    filter: hue-rotate(180deg);
  }

  .release {
    display: grid;
    justify-items: center;
    gap: 1rem;
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
