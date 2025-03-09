<script lang="ts">
	import { i18n } from '$lib/i18n.js';
	import { ParaglideJS } from '@inlang/paraglide-sveltekit';
	import '../app.css';
	let { children } = $props();
</script>


<nav class="bg-gray-800">
    <div class="mx-auto max-w-7xl px-2 sm:px-6 lg:px-8">
      <div class="relative flex h-16 items-center justify-between">
        <div class="flex flex-1 items-center justify-center sm:items-stretch sm:justify-start">
			<div class="flex shrink-0 items-center">
				<span class="text-white mr-2">Computer Algorithms</span>
			  </div>
          <div class="hidden sm:ml-6 sm:block">
            <div class="flex space-x-4">
              <a href="#user" class="rounded-md bg-gray-900 px-3 py-2 text-sm font-medium text-white" aria-current="page">User</a>
			  <a href="#about" class="rounded-md bg-gray-900 px-3 py-2 text-sm font-medium text-white" aria-current="page">About</a>
			</div>
          </div>
        </div>
      </div>
    </div>
  </nav>


<ParaglideJS {i18n}>
	{@render children()}
</ParaglideJS>
