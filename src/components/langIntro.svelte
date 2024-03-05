<script>
  
  export let title;
  export let level;
  export let description;
  export let src;
</script>

<div class="lang">
  <div class="sub-title">
    <div class="lang-name">
      <img {src} alt="img">
      <span>{title}</span>
    </div>
    <span>난이도 {level}</span>
  </div>
  <p>
    {description}
  </p>
</div>