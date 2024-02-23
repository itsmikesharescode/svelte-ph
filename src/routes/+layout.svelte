<script lang="ts">
	
    import "../app.pcss";
    import Nav from "$lib/components/custom/nav.svelte";
    import { ModeWatcher } from "mode-watcher";
    import { AlignJustify } from 'lucide-svelte';
    import { Search } from 'lucide-svelte';
    import { RadioTower, Home, Settings} from 'lucide-svelte';
    import sphIcon from "$lib/icons/VELTE PH.svg";
    import * as Sheet from "$lib/components/ui/sheet";
	import { Button } from "$lib/components/ui/button";

</script>

<ModeWatcher />

<div class="md:max-w-[85%] mx-auto ">
    <div class="sticky top-0 z-10">
        <Nav />
    </div>
    
    <div class="p-4">
        <slot />
    </div>
</div>
            
        
            


