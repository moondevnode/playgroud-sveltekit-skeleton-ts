<script lang="ts">
  import { faker } from '@faker-js/faker';

  // Local
  let currentVariant = 'variant-filled-error';
  const message = faker.lorem.paragraph();
  // Functions
  function triggerAction(): void {
    alert('The "Action" button was pressed!');
  }
</script>

<div class="container p-4 space-y-4">
  <aside class="alert variant-ghost-surface">
    <i class="fa-solid fa-triangle-exclamation text-4xl" />
    <div class="alert-message" data-toc-ignore="">
      <h3 class="h3" data-toc-ignore="">Warning</h3>
      <p>
        Exercitationem odit recusandae libero laudantium explicabo. Voluptates nulla ipsum saepe
        velit. Ab facilis ullam asperiores.
      </p>
    </div>
    <div class="alert-actions">
      <button class="btn variant-filled">Action</button>
      <button class="btn-icon variant-filled" on:click={triggerAction}
        ><i class="fa-solid fa-xmark" /></button
      >
    </div>
  </aside>
</div>
