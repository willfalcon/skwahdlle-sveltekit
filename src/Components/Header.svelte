
<header class="header">
  <h1 class="title">Skwahdle</h1>
</header>

<style>
  .header {
    display: flex;
  justify-content: center;
  display: grid;
  column-gap: 1rem;
  align-items: center;
  grid-template-columns: repeat(7, 1fr);
  grid-template-rows: auto 30px;
  padding: 2rem 1rem;
  max-width: 100%;
  /* color: ${({ theme }) => theme.heading}; */
  color: var(--heading);
  }

  .title {
    text-align: center;
    text-transform: uppercase;
    grid-column: 1 / -1;
    /* border-bottom: 1px solid ${({ theme }) => theme.light}; */
    border-bottom: 1px solid var(--lightgrey);

    margin: 0 0 1rem;
  }
  @media (min-width: 375px) {
    .title {
      grid-column: 3 / 4;
      padding-bottom: 1rem;
      margin-bottom: 0;
      padding-bottom: 0;
    }
    .header {
      grid-template-columns: 30px 30px 1fr 30px 30px;
      grid-template-rows: auto;
    }
  }
</style>