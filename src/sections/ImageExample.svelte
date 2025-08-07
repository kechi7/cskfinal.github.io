<script>
  import Scroller from "../lib/Scroller.svelte";
  import ArticleText from "../lib/ArticleText.svelte";
  import orchidImg from "../images/orchidTabImg.jpg";
</script>

<div>
  <Scroller layout="right">
    {#snippet sticky()}
      <img class="orchid" src={orchidImg} alt="Orchid Tablet" />
    {/snippet}

    {#snippet scrolly()}
      <ArticleText>
        <strong>
          Your final project might look totally different from this template!
        </strong>
      </ArticleText>

      <ArticleText>It's yours to create.</ArticleText>
    {/snippet}
  </Scroller>
</div>

<style>
  .orchid {
    width: 25%;
    margin: 0px auto;
  }
</style>
