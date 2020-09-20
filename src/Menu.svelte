<script lang="ts">
  const menuItems = [
    { id: 1, text: "Home", path: "#" },
    { id: 2, text: "News", path: "#" },
    { id: 3, text: "About", path: "#" },
  ];
</script>

<style>
  ul {
    padding: 10px 20px 10px 20px;
  }
  ul li {
    display: inline;
  }
  ul li a {
    padding: 0px 20px 0px 20px;
    font-family: "Courier New", Courier, monospace;
    font-size: 24px;
    color: black;
    text-emphasis: none;
  }
</style>

<ul>
  {#each menuItems as menuItem}
    <li><a href={menuItem.path}>{menuItem.text}</a></li>
  {/each}
</ul>
