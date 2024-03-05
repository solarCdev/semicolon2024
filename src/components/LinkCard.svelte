<script>
  export let title;
  export let description;
  export let creator;
  export let link;
  export let href;
</script>

<a href={href} target="_blank">
  <div class="link-card-wrap" style={`background: linear-gradient(rgba(0, 0, 0, 0), rgba(0, 0, 0, 1)), url(${link}); background-size: cover;`}>
    <h3>{title}</h3>
    <span>{description}</span>
    <br>
    <span class="cr">BY.{creator}</span>
  </div>
</a>

<style>
  h3 {
    font-size: 24px;
    line-height: 32px;
    margin-bottom: 4px;
  }

  span {
    font-size: 16px;
    font-weight: 400;
  }

  a {
    text-decoration: none;
  }

  .link-card-wrap {
    width: 100%;
    height: 360px;
    border-radius: 12px;
    padding: 24px;
    margin-bottom: 48px;
    display: flex;
    flex-direction: column;
    justify-content: end;
  }

  .cr {
    color: #c1c1c1;
    font-size: 14px;
  }
</style>