<script>
  export let name;
</script>

<style>
  .wrapper {
    display: grid;
    justify-content: center;
    align-items: center;
    height: 100%;
    font-size: 7rem;
  }

  .floating-spaceship {
    text-align: center;
    animation-name: move-around;
    animation-delay: 1s;
    animation-duration: 20s;
    animation-timing-function: ease-in-out;
    animation-iteration-count: infinite;
  }

  .youtube {
    box-shadow: 0 0 16px 2px rgba(0, 0, 0, 0.5);
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

<div class="wrapper">
  <div class="floating-spaceship">{name}</div>
  <iframe
    title="Kjør Romskip – Romturist"
    class="youtube"
    width="560"
    height="315"
    src="https://www.youtube-nocookie.com/embed/-GzNoOeA7ho"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen />
</div>
