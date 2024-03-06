<script>
  import pyImg from "$lib/assets/python.svg";
  import cImg from "$lib/assets/cpp.svg";
  import jsImg from "$lib/assets/js.svg";

  let python;
  let c;
  let js;
  $: lang = {
    python: python,
    c: c,
    js: js
  }

  const scroll = () => {
    window.scrollTo({
      top: python.style.offsetTop,
      left: 0,
      behavior: 'smooth'
    })
  }
</script>

<div class="margin">
  <h1>
    Activities <br>
    우리가 하는 것들.
  </h1>

  <h2>
    <span on:click={scroll}>Python</span>, <span>Javascript</span>, <span>C++</span>, <span>Rust</span>, 
    <span>Java</span>, <span>Kotlin</span>, <span>Ruby</span>, etc... <br>
    그 어떤 프로그래밍 언어도 상관 없어요. 하나를 골라서 자신만의 프로젝트를 제작해봅시다!
  </h2>

  <span>
    아직 무엇을 할지 모르겠다면 스크롤을 내려 보세요! <br>
    저희의 주요 언어중에서 선택해보세요.
  </span>

  <div>
    <h1 bind:this={python}>Python<img src={pyImg} alt="" style="width: 36px;"></h1>
    <p>
      가장 기본적인 언어예요. 하지만 할 수 있는 것들은 기본적인 것 뿐만 아니라 미니게임 제작, 머신러닝 구현 등 다양하죠.
    </p>
  </div>

  <div>
    <h1 bind:this={js}>Javascript<img src={jsImg} alt="" style="width: 36px;"></h1>
    <p>
      웹사이트를 개발하는 언어에요. 저희 동아리의 대부분을 차지하고 있죠.
    </p>
  </div>

  <div>
    <h1 bind:this={c}>C++<img src={cImg} alt="" style="width: 36px;"></h1>
    <p>
      정석적인 알고리즘과 고성능 언어에요. 그 대신 언어가 기계어에 더 가까워 난이도가 어렵습니다.
    </p>
  </div>
</div>

<style>
  .margin {
    padding: 16px;
    padding-top: 0;
    padding-bottom: 0;
  }

  h1 {
    line-height: 42px;
    margin-top: 48px;
    display: flex;
    align-items: center;
    gap: 12px;
  }

  h2 {
    line-height: 34px;
    margin-top: 48px;
    margin-bottom: 36px;
  }

  p {
    margin-top: 12px;
  }

</style>