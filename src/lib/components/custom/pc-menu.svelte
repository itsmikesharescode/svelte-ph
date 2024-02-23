<script lang="ts">
    import { toggleMode } from "mode-watcher";
    import { Label } from "$lib/components/ui/label";
    import { Switch } from "$lib/components/ui/switch";
	import Button from "../ui/button/button.svelte";

    let lightMode = false;

    $: lightMode ? toggleMode() : toggleMode();
</script>



<div class="flex gap-10">
    <div class="flex gap-5 items-center">
        <a href="/" class="text-xl text-muted-foreground">Home</a>
        <a href="/" class="text-xl text-muted-foreground">Blogs</a>
        <a href="/" class="text-xl text-muted-foreground">Projects</a>

        <div class="flex items-center gap-2">
            <Button> Log in</Button>

            <Button> Sign Up Free</Button>
        </div>
    </div>

    <div class="flex items-center space-x-2 justify-center ">
        <Switch id="theme" bind:checked={lightMode}/>
        <Label for="theme">{lightMode ? "Dark Mode" : "Light Mode"}</Label>
    </div>
</div>