<script>
    import Moon from "lucide-svelte/icons/moon";
    import Sun from "lucide-svelte/icons/sun";
    import { toggleMode } from "mode-watcher";

    import Button from "./button.svelte";
</script>

<Button
    on:click={toggleMode}
    class="fixed right-3 bottom-3 z-50"
    variant="outline"
    size="icon"
>
    <Sun
        class="h-[1.2rem] w-[1.2rem] rotate-0 scale-100 transition-all dark:-rotate-90 dark:scale-0"
    />
    <Moon
        class="absolute h-[1.2rem] w-[1.2rem] rotate-90 scale-0 transition-all dark:rotate-0 dark:scale-100"
    />
    <span class="sr-only">Toggle theme</span>
</Button>
