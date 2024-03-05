<script>
	import LinkCard from "../../components/LinkCard.svelte";
  import img0 from "$lib/assets/0.jpg";
  import img1 from "$lib/assets/1.jpg";
  import img2 from "$lib/assets/2.jpg";
  import img3 from "$lib/assets/3.png";
  import img5 from "$lib/assets/5.jpg";
</script>
<div class="margin">
  <h1>
    Projects <br>
    우리가 쌓아온 흔적.
  </h1>
  <div class="wrap">
    <LinkCard
    title="Myclass"
    description="반배정을 한눈에! 새학년 반배정 확인 사이트"
    creator="권호준"
    link={img0}
    href="https://myclass-banbaejung.vercel.app/"
  />

  <LinkCard
    title="세미콜론 홈페이지"
    description="세미콜론의 공식 홈페이지"
    creator="권호준"
    link={img1}
    href="/"
  />

  <LinkCard
    title="자연재해 서바이벌"
    description="자연재해들을 피해서 최대한 오래 살아남아야 하는 게임"
    creator="전재혁"
    link={img2}
    href="https://scratch.mit.edu/projects/757540875"
  />

  <LinkCard
    title="도담인이 자랑하는 도담중학교"
    description="도담중학교 홍보 사이트"
    creator="박인호"
    link={img3}
    href="https://hobakin.github.io/dodam-hongbo"
  />

  <LinkCard
    title="치킨 설명 사이트"
    description="여러 치킨들에 대해 알려주는 사이트"
    creator="정성훈, 도규민"
    link={img5}
    href="https://solarcdev.github.io/chicken-explain-jung-and-do/"
  />

  <LinkCard
    title="세종시 소개 사이트"
    description="세종시에 살게 되며 느낀 점들을 설명한 사이트"
    creator="강이수"
    link="https://upload.wikimedia.org/wikipedia/commons/e/e9/Hannuridaero_and_Bangchukcheon.jpg"
    href="https://leesu0710.github.io/Webpractice2/"
  />
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
  }

  .wrap {
    margin-top: 24px;
  }
</style>