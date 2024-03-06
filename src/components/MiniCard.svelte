<script>
  export let title;
  export let href;
</script>

<div>
  <h2>
    {title}
  </h2>
  <a href={href}><button>go!</button></a>
</div>

<style>
  div {
    width: 120px;
    height: 180px;
    margin-left: 16px;
    background-color: #121212;
    border-radius: 12px;
    padding: 12px;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
  }

  h2 {
    font-size: 20px;
    word-break: keep-all;
  }

  button {
    height: 48px;
    width: 100%;
  }
</style>