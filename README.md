# create skeleton-app

## References

- [Skeleton Home](https://www.skeleton.dev/)
- [Skeleton Docs](https://www.skeleton.dev/docs/introduction)
- [Skeleton Theme](https://www.skeleton.dev/docs/generator)
- [Skeleton Github](https://github.com/skeletonlabs/skeleton)


## Installation

```bash
# boot app(setup github repo & install modules)
bootapp -u moondevnode -n playgroud-sveltekit-skeleton-ts -d "SvelteKit with Skeleton UI" -t sveltekit-skeleton-ts
```


## Developing

```bash
# start the server and open the app in a new browser tab
npm run dev -- --open
```


## Building

```sh
npm run build
```


# Genertate Theme

## [Skeleton Theme](https://www.skeleton.dev/docs/generator)

> Switch on `Enable Preview`
> Click `Randomize Colors`
> Click `Show Theme CSS`
> Click `Copy` in CSS code block
> Paste to `/src/app.postcss`

> Check in browser `http://localhost:5173/`


# Add Appshell

## Add Sidebar Navigation
> `/src/routes/+layout.svelte`

```svelte
<script lang="ts">
 ...
  import { AppShell, AppBar } from '@skeletonlabs/skeleton';
</script>

<AppShell slotSidebarLeft="bg-surface-500/5 w-56 p-4">
  <svelte:fragment slot="sidebarLeft">
    <!-- Insert the list: -->
    <nav class="list-nav">
      <ul>
        <li><a href="/">Home</a></li>
        <li><a href="/about">About</a></li>
      </ul>
    </nav>
    <!-- --- -->
  </svelte:fragment>
  <slot />
</AppShell>
```

## Page Setup
> `/src/routes/+page.svelte`

```svelte
<div class="container mx-auto p-8 space-y-8">
	<h1 class="h1">Hello Skeleton</h1>
	<p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
	<section>
		<a class="btn variant-filled-primary" href="https://kit.svelte.dev/">SvelteKit</a>
		<a class="btn variant-filled-secondary" href="https://tailwindcss.com/">Tailwind</a>
		<a class="btn variant-filled-tertiary" href="https://github.com/">GitHub</a>
	</section>
</div>
```

## Add a Component
> `/src/routes/+page.svelte`

```svelte
<script>
	import { Avatar } from '@skeletonlabs/skeleton';
</script>

<Avatar src="https://i.pravatar.cc/" />
```