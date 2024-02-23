<script lang="ts">
    import { AlignJustify } from 'lucide-svelte';
	import Button from "$lib/components/ui/button/button.svelte";
    import MobileMenu from "$lib/components/custom/mobile-menu.svelte";
	import SvelteIcon from './svelteicon.svelte';
	import PcMenu from './pc-menu.svelte';
</script>

<div class="w-full backdrop-blur-lg flex items-center justify-between p-2 "> 

    <button class="p-2 rounded-lg">
        <SvelteIcon />
    </button>
        
    <div class="md:hidden">
        <MobileMenu />
    </div>

    <div class="hidden md:flex">
        <PcMenu />
    </div>
</div>


