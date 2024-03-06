<script>
  import "../style/app.css";
  import kakao from "$lib/assets/kakao.svg";
  import instar from "$lib/assets/instargram.svg";
  let showMenu = false;
  const toggleMenu = () => {showMenu = !showMenu};
</script>

<main>
  {#if showMenu}
    <div class="black" on:click={toggleMenu}>
      <div class="menu-bar">
        <ul>
          <a href="/"><li>Home</li></a>
          <a href="/contact"><li>Contact</li></a>
          <a href="/projects"><li>Projects</li></a>
          <a href="/activity"><li>Activities</li></a>
        </ul>
      </div>
    </div>
  {/if}
  <div id="top-padding"></div>
  <nav>
    <div class="flex"></div>
    <a href="/">SEMICOLON</a>
    <button class="menu-btn" on:click={() => {showMenu = !showMenu;}}>Menu</button>
  </nav>

  <slot/>

  <footer>
    <h4>semicolon2024</h4>
    <br>
    <div>
      <span>Copyright&copy;team_semicolon</span><br>
      <span>제작: 세미콜론 동아리장 권호준</span><br>
      <a href="https://icons8.com/">icon by icon8</a>
    </div>
    <div class="sns">
      <a href="https://open.kakao.com/o/gHWMH4Zf" target="_blank">
        <button><img src={kakao} alt="" style="width: 48px;"></button>
      </a>
      
      <a href="https://www.instagram.com/team_semicolon.official/" target="_blank">
        <button><img src={instar} alt="" style="width: 48px;"></button>
      </a>
    </div>
  </footer>
</main>

<style>
  :global(:root){
    --blue: #3636ff;
	  --mint: #2bfca4;
  }

  #top-padding {
    height: 44px;
    width: 100%;
  }

  nav {
    height: 64px;
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 24px;
    top: 0;
    position: sticky;
    background-color: rgba(0, 0, 0, 0.2);
    backdrop-filter: blur(25px);
    border-bottom: 1px solid #474747;
    z-index: 0;

  }

  nav > a{
    text-decoration: none;
    font-size: 16px;
    font-weight: 600;
    color: white;
  }

  .flex {
    width: 64px;
    height: 64px;
  }

  .menu-btn {
    width: 64px;
    height: 64px;
    background: none;
  }

  .menu-btn:hover {
    background: none;
    border: none;
    backdrop-filter: none;
    color: var(--blue);
  }

  .menu-bar {
    display: flex;
    position: fixed;
    width: 200px;
    height: 100vh;
    right: 0;
    z-index: 100;
    background-color: #000;
    flex-direction: column;
    align-items: center;
    padding-top: 120px;
  }

  ul {
    display: flex;
    flex-direction: column;
    list-style: none;
    gap: 48px;
    font-size: 24px;
    font-weight: 700;
  }

  .black {
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 0.8);
    
    display: block;
    position: fixed;
  }

  footer {
    width: 100%;
    height: 280px;
    border-top: 1px solid #474747;
    padding: 24px;
    margin-top: 48px;
  }

  .sns {
    margin-top: 36px;
    display: flex;
    align-items: center;
  }

  .sns > a {
    width: 64px;
    height: 64px;
    margin-right: 4px;
    
  }

  .sns > a > button {
    background-color: #00000000;
  }

  .sns > a > button:hover {
    border: none;
    backdrop-filter: none;
  }

  ul > a {
    text-decoration: none;
  }
  
</style>