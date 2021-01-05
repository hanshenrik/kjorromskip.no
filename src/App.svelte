<script>
  export let name;

  // Load Facebook SDK for JavaScript
  window.fbAsyncInit = function () {
    FB.init({
      xfbml: true,
      version: "v9.0",
    });
  };

  (function (d, s, id) {
    var js,
      fjs = d.getElementsByTagName(s)[0];
    if (d.getElementById(id)) return;
    js = d.createElement(s);
    js.id = id;
    js.src = "https://connect.facebook.net/nb_NO/sdk/xfbml.customerchat.js";
    fjs.parentNode.insertBefore(js, fjs);
  })(document, "script", "facebook-jssdk");
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
    max-width: 100%;
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

  <!-- Messenger Chat Plugin -->
  <div id="fb-root" />
  <div
    class="fb-customerchat"
    attribution="setup_tool"
    page_id="143074806532195"
    theme_color="#0A7CFF"
    greeting_dialog_display="hide"
    logged_in_greeting="Heisann! Var det noe?"
    logged_out_greeting="Heisann! Var det noe?" />
</div>
