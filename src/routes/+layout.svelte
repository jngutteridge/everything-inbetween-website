<script lang="ts">
	import '../app.css';
	
	let { children } = $props();
</script>

<div class="bg-[url(/images/stage-smoke-background.jpg)] bg-purple-900 bg-cover bg-center h-screen w-screen grid grid-rows-[auto_1fr_auto]">
  <header class="flex flex-col justify-center items-center pt-8 pb-8">
    <h2>
      <img src="/images/everything-inbetween-logo.png" alt="Everything In-between logo" class="w-58 max-w-[40vw]" />
      <span class="hidden">Everything In-between</span>
    </h2>
    <ul class="flex flex-row gap-4 justify-center items-center pt-4">
      <li class="bg-white/85 rounded-2xl shadow-md shadow-black/85">
        <a href="https://www.facebook.com/profile.php?id=61576269112129" target="_blank">
          <img src="/icons/facebook.svg" alt="Facebook icon" class="w-20" />
          <span class="hidden">Facebook</span>
        </a>
      </li>
      <li class="bg-white/85 rounded-2xl shadow-md shadow-black/85">
        <a href="https://www.instagram.com/everything.in.between.band/" target="_blank">
          <img src="/icons/instagram.svg" alt="Instagram icon" class="w-20" />
          <span class="hidden">Instagram</span>
        </a>
      </li>
    </ul>
  </header>

  <main class="overflow-y-auto">
	  {@render children()}
  </main>

  <footer class="text-center text-white p-4">
    <p>Website by <a href="https://www.bespokemedia.net/" target="_blank" class="underline">Bespoke Media</a></p>
  </footer>
</div>

<svelte:head>
  <meta name="description" content="5-piece party and function band, crossing through all genres, made to fill the dance floor" />
  <meta name="theme-color" content="#b918e5" />
  <link rel="icon" type="image/png" href="/images/everything-inbetween-logo.png" />
</svelte:head>