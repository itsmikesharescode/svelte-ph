<script lang="ts">
    import { AlignJustify } from 'lucide-svelte';
    import { Search } from 'lucide-svelte';
    import { RadioTower, Home, Settings} from 'lucide-svelte';
    import sphIcon from "$lib/icons/VELTE PH.svg";
	import LightSwitch from './lightswitch.svelte';
	import Button from '../ui/button/button.svelte';
    import * as Sheet from "$lib/components/ui/sheet";
</script>

<!--Will Download If the User Uses Mobile-->
<nav class="fixed w-full p-2 backdrop:blur-sm flex items-center justify-between sm:hidden">
    <div class="p-2 bg-[#000000] rounded-xl">
        <img src={sphIcon} class="w-16  " alt="sph-icon" />
    </div>

    <div class="flex items-center gap-2"> 
        <Button variant="ghost" size="icon">
            <Search />
        </Button>

        <Sheet.Root>
            <Sheet.Trigger>
                <Button variant="ghost" size="icon">
                    <AlignJustify />
                </Button>
            </Sheet.Trigger>
            
            <Sheet.Content class="pt-[10dvh] flex flex-col gap-2 justify-center sm:hidden" side="left">
                <Sheet.Header>

                    <Sheet.Title class="p-2 text-2xl flex items-center gap-4">
                        <RadioTower />
                        <span>Forum</span>
                    </Sheet.Title>

                    <Sheet.Title class="p-2 text-2xl flex items-center gap-4">
                        <Home />
                        <span>Community</span>
                    </Sheet.Title>

                    <Sheet.Title class="p-2 text-2xl flex items-center gap-4">
                        <Settings />
                        <span>Account</span>
                    </Sheet.Title>
                </Sheet.Header>
            </Sheet.Content>
        </Sheet.Root>

        <LightSwitch />
       
    </div>
</nav>

<!--Will Download If the User Uses Desktop-->
<nav class="fixed w-full p-2 backdrop:blur-sm  hidden sm:flex items-center justify-between ">
    

    <div class="flex items-center gap-2"> 
        <Button variant="ghost" size="icon">
            <Search />
        </Button>

        <LightSwitch />
       
    </div>
</nav>