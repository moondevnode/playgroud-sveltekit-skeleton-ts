<script>
  import { Avatar } from '@skeletonlabs/skeleton';
  import { Accordion, AccordionItem } from '@skeletonlabs/skeleton';
</script>

<div class="container mx-auto p-8 space-y-8">
  <h1 class="h1">Hello Skeleton</h1>
  <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
  <section>
    <a class="btn variant-filled-primary" href="https://kit.svelte.dev/">SvelteKit</a>
    <a class="btn variant-filled-secondary" href="https://tailwindcss.com/">Tailwind</a>
    <a class="btn variant-filled-tertiary" href="https://github.com/">GitHub</a>
  </section>
  <Avatar src="https://i.pravatar.cc/" />
</div>

<Accordion>
  <AccordionItem open>
    <svelte:fragment slot="lead">(icon)</svelte:fragment>
    <svelte:fragment slot="summary">(summary)</svelte:fragment>
    <svelte:fragment slot="content">(content)</svelte:fragment>
  </AccordionItem>
  <AccordionItem>
    <svelte:fragment slot="lead">(icon)</svelte:fragment>
    <svelte:fragment slot="summary">(summary)</svelte:fragment>
    <svelte:fragment slot="content">(content)</svelte:fragment>
  </AccordionItem>
  <!-- ... -->
</Accordion>

<aside class="alert variant-filled-error">
  <i class="fa-solid fa-triangle-exclamation text-4xl" />
  <!-- <i class="fa-triangle-exclamation text-4xl" /> -->
  <div class="alert-message" data-toc-ignore>
    <h3 class="h3" data-toc-ignore>Warning</h3>
    <p>
      <i class="fa-brands fa-android fa-rotate-90" />
      Pariatur facere vel repellendus saepe. Vel sed et voluptas neque. Natus qui aperiam dolores quasi
      quae quas deleniti saepe.
    </p>
  </div>
  <div class="alert-actions">
    <button class="btn variant-filled">Action</button>
    <button class="btn-icon variant-filled"><i class="fa-solid fa-xmark" /></button>
  </div>
</aside>

<div class="w-full text-token card p-4 space-y-4">
  <ol class="list">
    <li>
      <span class="badge-icon p-4 variant-soft-primary">1</span>
      <span class="flex-auto">Skeleton</span>
    </li>
    <li>
      <span class="badge-icon p-4 variant-soft-primary">2</span>
      <span class="flex-auto">Svelte</span>
    </li>
  </ol>
</div>

<div
  class="previewer shadow-2xl shadow-surface-500/10 dark:shadow-black/10 rounded-container-token overflow-hidden"
>
  <header
    class="previewer-header bg-surface-200-700-token p-4 flex justify-between items-center gap-4"
  >
    <div
      class="radio-group p-1 inline-flex bg-surface-200-700-token border-token border-surface-400-500-token space-x-1 rounded-token"
      data-testid="radio-group"
      role="radiogroup"
      aria-labelledby=""
    >
      <label
        ><div
          class="radio-item flex-auto text-base text-center cursor-pointer px-4 py-1 rounded-token variant-filled"
          data-testid="radio-item"
          role="radio"
          aria-checked="true"
          aria-label=""
          tabindex="0"
          title="Preview"
        >
          <div class="h-0 w-0 overflow-hidden">
            <input type="radio" name="view" value="preview" tabindex="-1" />
          </div>
          <i class="fa-solid fa-eye text-sm" />
        </div></label
      >
      <label
        ><div
          class="radio-item flex-auto text-base text-center cursor-pointer px-4 py-1 rounded-token hover:variant-soft"
          data-testid="radio-item"
          role="radio"
          aria-checked="false"
          aria-label=""
          tabindex="0"
          title="Code"
        >
          <div class="h-0 w-0 overflow-hidden">
            <input type="radio" name="view" value="code" tabindex="-1" />
          </div>
          <i class="fa-solid fa-code text-sm" />
        </div></label
      >
    </div>
    <div class="flex justify-between gap-4">
      <button class="btn-icon variant-soft" title="Backgrounds"
        ><i class="fa-solid fa-swatchbook text-sm" /></button
      >
    </div>
  </header>
  <div
    class="previewer-viewport p-4 md:p-10 space-y-4 bg-gradient-to-br variant-gradient-primary-secondary"
  >
    <div
      class="previewer-preview flex justify-center items-center mx-auto transition-[width] duration-200 w-full"
    >
      <div class="w-full text-token grid grid-cols-1 md:grid-cols-2 gap-4">
        <div class="card bg-initial p-4 flex justify-center items-center"><span>Minimal</span></div>
        <a class="card bg-initial card-hover overflow-hidden" href="/elements/cards"
          ><header>
            <img
              src="https://images.unsplash.com/photo-1620562303747-ba21ca6f1530?ixid=M3w0Njc5ODF8MHwxfGFsbHx8fHx8fHx8fDE2ODc5NzY2MjR8&amp;ixlib=rb-4.0.3&amp;w=400&amp;h=175&amp;auto=format&amp;fit=crop"
              class="bg-black/50 w-full aspect-[21/9]"
              alt="Post"
            />
          </header>
          <div class="p-4 space-y-4">
            <h6 class="h6">Announcements</h6>
            <h3 class="h3" data-toc-ignore="">Skeleton is Awesome!</h3>
            <article>
              <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Numquam aspernatur
                provident eveniet eligendi cumque consequatur tempore sint nisi sapiente. Iste
                beatae laboriosam iure molestias cum expedita architecto itaque quae rem.
              </p>
            </article>
          </div>
          <hr class="opacity-50" />
          <footer class="p-4 flex justify-start items-center space-x-4">
            <figure
              class="avatar flex aspect-square text-surface-50 font-semibold justify-center items-center overflow-hidden isolate bg-surface-400-500-token w-8 rounded-full"
              data-testid="avatar"
            >
              <img
                class="avatar-image w-full h-full object-cover"
                src="https://images.unsplash.com/photo-1617296538902-887900d9b592?ixid=M3w0Njc5ODF8MHwxfGFsbHx8fHx8fHx8fDE2ODc5NzExMDB8&amp;ixlib=rb-4.0.3&amp;w=32&amp;h=32&amp;auto=format&amp;fit=crop"
                alt=""
                style=""
              />
            </figure>
            <div class="flex-auto flex justify-between items-center">
              <h6 class="font-bold">By Alex</h6>
              <small>On 2023. 7. 5.</small>
            </div>
          </footer></a
        >
      </div>
    </div>
  </div>
  <footer class="previewer-footer variant-soft p-4">
    <div class="flex justify-center gap-4">
      <select class="select w-auto"
        ><optgroup label="Utility Classes"
          ><option value="bg-initial">bg-initial</option><option value="!bg-transparent"
            >!bg-transparent</option
          ></optgroup
        ><optgroup label="Filled Variants"
          ><option value="variant-filled">variant-filled</option><option
            value="variant-filled-surface">variant-filled-surface</option
          ><option value="variant-filled-primary">variant-filled-primary</option><option
            value="variant-filled-secondary">variant-filled-secondary</option
          ><option value="variant-filled-tertiary">variant-filled-tertiary</option><option
            value="variant-filled-success">variant-filled-success</option
          ><option value="variant-filled-warning">variant-filled-warning</option><option
            value="variant-filled-error">variant-filled-error</option
          ></optgroup
        ><optgroup label="Ghost Variants"
          ><option value="variant-ghost">variant-ghost</option><option value="variant-ghost-surface"
            >variant-ghost-surface</option
          ><option value="variant-ghost-primary">variant-ghost-primary</option><option
            value="variant-ghost-secondary">variant-ghost-secondary</option
          ><option value="variant-ghost-tertiary">variant-ghost-tertiary</option><option
            value="variant-ghost-success">variant-ghost-success</option
          ><option value="variant-ghost-warning">variant-ghost-warning</option><option
            value="variant-ghost-error">variant-ghost-error</option
          ></optgroup
        ><optgroup label="Soft Variants"
          ><option value="variant-soft">variant-soft</option><option value="variant-soft-surface"
            >variant-soft-surface</option
          ><option value="variant-soft-primary">variant-soft-primary</option><option
            value="variant-soft-secondary">variant-soft-secondary</option
          ><option value="variant-soft-tertiary">variant-soft-tertiary</option><option
            value="variant-soft-success">variant-soft-success</option
          ><option value="variant-soft-warning">variant-soft-warning</option><option
            value="variant-soft-error">variant-soft-error</option
          ></optgroup
        ><optgroup label="Ringed Variants"
          ><option value="variant-ringed">variant-ringed</option><option
            value="variant-ringed-surface">variant-ringed-surface</option
          ><option value="variant-ringed-primary">variant-ringed-primary</option><option
            value="variant-ringed-secondary">variant-ringed-secondary</option
          ><option value="variant-ringed-tertiary">variant-ringed-tertiary</option><option
            value="variant-ringed-success">variant-ringed-success</option
          ><option value="variant-ringed-warning">variant-ringed-warning</option><option
            value="variant-ringed-error">variant-ringed-error</option
          ></optgroup
        ><optgroup label="Gradient Variants"
          ><option value="bg-gradient-to-br variant-gradient-primary-secondary"
            >bg-gradient-to-br variant-gradient-primary-secondary</option
          ><option value="bg-gradient-to-br variant-gradient-secondary-tertiary"
            >bg-gradient-to-br variant-gradient-secondary-tertiary</option
          ><option value="bg-gradient-to-br variant-gradient-tertiary-primary"
            >bg-gradient-to-br variant-gradient-tertiary-primary</option
          ><option value="bg-gradient-to-br variant-gradient-secondary-primary"
            >bg-gradient-to-br variant-gradient-secondary-primary</option
          ><option value="bg-gradient-to-br variant-gradient-tertiary-secondary"
            >bg-gradient-to-br variant-gradient-tertiary-secondary</option
          ><option value="bg-gradient-to-br variant-gradient-primary-tertiary"
            >bg-gradient-to-br variant-gradient-primary-tertiary</option
          ><option value="bg-gradient-to-br variant-gradient-success-warning"
            >bg-gradient-to-br variant-gradient-success-warning</option
          ><option value="bg-gradient-to-br variant-gradient-warning-error"
            >bg-gradient-to-br variant-gradient-warning-error</option
          ><option value="bg-gradient-to-br variant-gradient-error-success"
            >bg-gradient-to-br variant-gradient-error-success</option
          ><option value="bg-gradient-to-br variant-gradient-warning-success"
            >bg-gradient-to-br variant-gradient-warning-success</option
          ><option value="bg-gradient-to-br variant-gradient-error-warning"
            >bg-gradient-to-br variant-gradient-error-warning</option
          ><option value="bg-gradient-to-br variant-gradient-success-error"
            >bg-gradient-to-br variant-gradient-success-error</option
          ></optgroup
        ></select
      >
    </div>
  </footer>
</div>

<button type="button" class="btn variant-filled">Button</button>
