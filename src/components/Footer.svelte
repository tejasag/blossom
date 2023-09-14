<script>
  let formatter = new Intl.DateTimeFormat([], {
    timeZone: "Asia/Kolkata",
    hour: "numeric",
    minute: "numeric",
    hour12: false,
  });
  let time = formatter.format(Date.now());

  // TODO: connect this to spotify;
  let music = "playing nothing";
</script>

<div class="footer flex flex-col items-center justify-center">
  <div class="socials flex flex-row items-center">
    <a href="https://github.com/tejasag" target="_blank" rel="noreferrer">
      <img class="icon" src="GitHub.svg" alt="" />
    </a>
    |
    <a href="https://twitter.com/tejasag0" target="_blank" rel="noreferrer">
      <img class="icon" src="Twitter.svg" alt="" />
    </a>
    |
    <a href="https://behance.net/tejasag" target="_blank" rel="noreferrer">
      <img class="icon" src="behance.svg" alt="" />
    </a>
    |
    <a href="http://linkedin.com/in/tejasag0" target="_blank" rel="noreferrer">
      <img class="icon" src="LinkedIn.svg" alt="" />
    </a>
    |
    <a href="mailto:me@tejasag.com">
      <img class="icon" src="email.svg" alt="" />
    </a>
  </div>
  <div class="locale flex flex-col sm:inline items-center">
    ⏰ {time.toLocaleLowerCase()} ~ 📍 new delhi, india
    <div class="sm:inline">
      <span class="invisible sm:visible"> ~</span> 🎵 {music}
    </div>
  </div>
  <div class="end mb-2">made w/ ❤️ and peer pressure by me</div>
</div>

<style>
  .footer {
    font-family: "Cedarville Cursive";
    font-size: 1.2rem;
    color: #8b787c;
  }
  .icon {
    @apply m-3;
    height: 1.7rem;
  }
</style>
