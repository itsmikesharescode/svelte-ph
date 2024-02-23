<script lang="ts">
    import { AlignJustify } from 'lucide-svelte';
    import Button from "$lib/components/ui/button/button.svelte";
    import * as Sheet from "$lib/components/ui/sheet";
	import SvelteIcon from './svelteicon.svelte';
    import { Label } from "$lib/components/ui/label";
    import { Switch } from "$lib/components/ui/switch";
    import { toggleMode } from "mode-watcher";


    let lightMode = false;

    $: lightMode ? toggleMode() : toggleMode();

    
</script>

<Sheet.Root>

    <Sheet.Trigger>
        <Button size="icon" variant="ghost">
            <AlignJustify />
        </Button>
    </Sheet.Trigger>

    <Sheet.Content side="left" class="pt-[10dvh] md:hidden">
        <Sheet.Header>
            <div class="">
                <SvelteIcon />
            </div>
            <Sheet.Title>How are you today?</Sheet.Title>

            <Sheet.Description>
                Svelte PH is home for svelte developers.
            </Sheet.Description>

            <div class="pt-[5dvh] flex flex-col gap-3">
                <a href="/" class="text-2xl text-muted-foreground">Home</a>
                <a href="/" class="text-2xl text-muted-foreground">Blogs</a>
                <a href="/" class="text-2xl text-muted-foreground">Projects</a>
            </div>

            <div class="flex flex-col gap-2 pt-5">
                <Button size="sm"> Log in</Button>
                <Button size="sm"> Sign Up Free</Button>
            </div>

            <div class="absolute w-full bottom-0 left-0 p-4">
                <div class="flex items-center space-x-2 justify-center ">
                    <Switch id="theme" bind:checked={lightMode}/>
                    <Label for="theme">{lightMode ? "Dark Mode" : "Light Mode"}</Label>
                </div>
            </div>

        </Sheet.Header>
    </Sheet.Content>
</Sheet.Root>