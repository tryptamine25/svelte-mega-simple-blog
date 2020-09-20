<script lang="ts">
  const articles = [
    {
      id: 1,
      title: "Svelte 3: Rethinking reactivity",
      description:
        "After several months of being just days away, we are over the moon to announce the stable release of Svelte 3. This is a huge release representing hundreds of hours of work by many people in the Svelte community, including invaluable feedback from beta testers who have helped shape the design every step of the way. We think you're going to love it.",
      path: "#",
    },
    {
      id: 2,
      title: "Write less code",
      description:
        "All code is buggy. It stands to reason, therefore, that the more code you have to write the buggier your apps will be. Writing more code also takes more time, leaving less time for other things like optimisation, nice-to-have features, or being outdoors instead of hunched over a laptop.",
      path: "#",
    },
    {
      id: 3,
      title: "Svelte for new developers",
      description:
        "This short guide is designed to help you — someone who has looked at the tutorail and wants to start creating Svelte apps, but doesn't have a ton of experience using JavaScript build tooling — get up and running.",
      path: "#",
    },
    {
      id: 4,
      title: "Virtual DOM is pure overhead",
      description:
        "If you've used JavaScript frameworks in the last few years, you've probably heard the phrase 'the virtual DOM is fast', often said to mean that it's faster than the real DOM. It's a surprisingly resilient meme — for example people have asked how Svelte can be fast when it doesn't use a virtual DOM. It's time to take a closer look.",
      path: "#",
    },
  ];
</script>

<style>
  .articles {
    padding: 0px 100px;
  }
  @media (max-width: 768px) {
    .articles {
      padding: 0;
    }
  }
  .article-title {
    padding: 20px;
    font-size: 24px;
    font-family: "Courier New", Courier, monospace;
    text-decoration: underline;
  }
  .article-title a {
    color: black;
  }
  .article-description {
    font-size: 18px;
    font-family: "Courier New", Courier, monospace;
  }
</style>

<div class="articles">
  {#each articles as article}
    <p class="article-title"><a href={article.path}>{article.title}</a></p>
    <span class="article-description">{article.description}</span>
  {/each}
</div>
