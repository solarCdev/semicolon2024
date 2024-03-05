<script>
	import MiniCard from "../components/MiniCard.svelte";
  import prism from "$lib/assets/prism.png";

</script>

<div>
  <link
    rel="stylesheet"
    as="style"
    crossorigin
    href="https://cdn.jsdelivr.net/gh/orioncactus/pretendard@v1.3.9/dist/web/static/pretendard.min.css"
  />

  <div class="main-wrap">
    <div>
      <h1 class="title">
        TEAM <br>
        SEMICOLON
      </h1>
      <span>
        팀 세미콜론(서비스 개발 동아리)
      </span>
    </div>
    <button class="main-join">
      참여하기
    </button>
  </div>

  <div class="p-wrap">
    <h2>
      프로그래밍을 하는 동아리,<br>
      어려운 수학 계산을 해야 할 것 같고,<br>
      재미없어 보이죠.
    </h2>
    <br>
    <h2>
      <strong>
        그래서 우리는 그런 생각을<br>
        깨고자 해요. 쉽고 간단한 방법으로. <br>
        프로그래밍을 아직 아예 못한다고 해도
        괜찮아요!
      </strong>
    </h2>
  </div>

  <div class="p-wrap">
    <h1>경계를 넘어</h1>
    <br>
    <p>
      프로그래밍만으로는 간단한 계산만 가능해요.
      <strong>하지만 멋진 아이디어와 디자인, 기획, 기능적 구상이 가미된다면 그 힘은 무한하죠.</strong>
      저희 동아리를 ‘프로그래밍 동아리’가 아닌 ‘서비스 개발 동아리’로 소개하게 된 이유도 여기에 있답니다.
    </p>
    <img src={prism} alt="prism logo" class="prism-img" style="width: 100%;">
  </div>

  <div class="p-wrap">
    <h1>SINCE 2022</h1>
    <br>
    <p>
      저희 동아리는 2022년 자율동아리로, 2023년 동그라미 프로젝트로 활동해왔어요. 특히 작년에는 정말 많은 프로젝트들이 만들어지게 되었죠.
      <a href="/projects">직접 보러 가보시려면 따라오세요!(바로가기)</a>
    </p>
    <!-- <div class="link-wrap">
      <MiniCard/>
      <div></div>
      <div></div>
      <div></div>
    </div> -->
  </div>

  <div class="p-wrap">
    <h1>발전하는 팀</h1>
    <br>
    <p> 작년의 활동 결과, 실제로 프로젝트에 어려움을 겪는 친구들이 많다는 사실을 느끼게 되었어요. 이번에는 여러분이 프로그램을 조금 더 여유있게 구상하도록 도울 것입니다.</p>
  </div>
</div>

<style>
  .title {
    text-align: center;
    margin-bottom: 12px;
  }

  .main-wrap {
    width: 100%;
    height: 100vh;
    background: linear-gradient(rgba(0, 0, 0, 0.8), rgb(0, 0, 0, 0.8)), url("../lib/assets/bg.jpg");
    background-size: cover;
    background-position: center;
    background-attachment: fixed;
    background-blend-mode: darken;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-around;
    padding-bottom: 48px;
  }

  /* .main-wrap::after {
    position: absolute;
    width: 100%;
    height: 100vh;
    background-color: red;
    display: block;
  } */

  .main-join {
    width: 168px;
    height: 48px;
  }

  .p-wrap {
    margin: 120px 16px 0 16px;
  }

  p {
    color: #C1C1C1;
    line-height: 24px;
  }

  h2 {
    font-size: 24px;
    line-height: 34px;
  }

  .link-wrap {
    margin-top: 24px;
  }
</style>
