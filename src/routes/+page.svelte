<script lang="ts">
  import banner from '$lib/assets/images/illustration-article.svg'
  import avatar from '$lib/assets/images/image-avatar.webp'
</script>

<main>
  <img class="banner" src={banner} alt="banner" >
  <header>
    <span class="tag bold">Learning</span>
    <p class="small">Publised 21 Dec 2023</p>
  </header>
  <section class="description">
    <h3>HTML & CSS foundations</h3>
    <p class="gray">These languages are the backbone of every website, defining structure, content, and presentation</p>
  </section>
    <footer>
    <img src={avatar} alt="avatar" class="avatar">
    <p class="bold">Greg Hooper</p>
  </footer>
</main>

<style>
  main {
    background-color: var(--clr-neutral-1);
    border-radius: 1rem;
    margin-inline: 1.5rem;
    padding: 1.5rem;
    box-shadow: 0.5rem 0.5rem 0 0 black;
    max-width: 25rem;
  }

  header {
    display: grid;
    gap: 1rem;
    margin-block: 1rem;
  }

  .banner {
    width: 100%;
    object-fit: cover;
    border-radius: 0.5rem;
  }

  .tag {
    background-color: var(--clr-primary-1);
    padding-block: 0.5rem;
    padding-inline: 1rem;
    border-radius: 0.5rem;
    margin-right: auto;
  }

  .description {
    display: grid;
    gap: 1rem;
  }

  footer {
    display: grid;
    grid-template-columns: auto 1fr;
    gap: 1rem;
    align-items: center;
    margin-top: 1rem;
  }

  .avatar {
    width: 2rem;
  }

  /* typography */

  p {
    line-height: 1.5rem;
  }

  .bold {
    font-weight: var(--fw-bold);
  }

  .small {
    font-size: small;
  }

  .gray {
    color: var(--clr-neutral-2);
  }

</style>