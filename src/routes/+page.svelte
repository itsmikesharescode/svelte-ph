<script lang="ts">
	import Button from "$lib/components/ui/button/button.svelte";
    import * as Avatar from "$lib/components/ui/avatar";
    import { RadioTower, Home, Settings} from 'lucide-svelte';
    import { ArrowUp } from 'lucide-svelte';
    import { MessageSquare } from 'lucide-svelte';
</script>

<div class="flex flex-col gap-4">
    <div class="flex items-center justify-between">
        <h1 class="text-3xl font-bold">Svelte PH</h1>
        <Button class="flex gap-2 items-center">
            <RadioTower size="18px"/>
            <span>New Post</span>
        </Button>
    </div>

    {#each ["", "","", "","", "","", "","", "","", "","", "",] as test }
        <div class=" border-2 p-4 rounded-xl dark:bg-[#242526] flex flex-col gap-2">
        <div class="flex items-center gap-2">
            <Avatar.Root>
                <Avatar.Image src="https://github.com/shadcn.png" alt="@shadcn" />
                <Avatar.Fallback>CN</Avatar.Fallback>
            </Avatar.Root>

            <p class="leading-7 font-bold">Lil Bob Mar</p>
            <p class="text-sm text-muted-foreground">Posted 4 hours ago</p>

        </div>

        <h3 class="scroll-m-20 text-2xl font-semibold tracking-tight">Why Choose Svelte in 2024?</h3>

        <div class="">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Eligendi deserunt animi explicabo omnis a sit sequi. Pariatur quas molestias blanditiis tempore cumque voluptates ex ullam expedita corrupti veritatis harum, consequuntur nam sunt quaerat voluptatum repudiandae porro corporis saepe ducimus quam non commodi? Quibusdam minima sequi, saepe in quas quasi! Repellat, placeat qui numquam odio ex molestias consequuntur dolor, in, eum illo et ullam eaque. Ducimus vel fugiat recusandae tempore iure esse quisquam a odio laudantium. Recusandae sunt illum, excepturi aliquid iste velit quo ut, eos veniam totam voluptatum facilis tempora. Tempore molestiae dolores cumque tempora commodi. Laboriosam maiores similique corrupti dolores perspiciatis quasi velit dolorem neque perferendis ducimus modi, adipisci facere in porro dolor. Omnis tempore nihil hic maiores quasi facere iusto alias nam at, nostrum ipsam eum necessitatibus, asperiores qui excepturi. Dolorum commodi, adipisci voluptatibus accusantium odit hic sint sit ad, enim saepe illum! Esse, necessitatibus? Doloremque saepe architecto veritatis, dolore nulla adipisci placeat sequi temporibus enim quisquam mollitia doloribus numquam in, iste nam porro quos sapiente possimus vero fugiat totam provident quo. Libero voluptatum corporis sunt nihil veniam ut voluptatibus esse numquam aliquam laboriosam amet nesciunt, error magnam repellendus delectus, recusandae eveniet consequatur! Necessitatibus quisquam inventore non! Eos.
        </div>
        

        <div class="flex items-center gap-2 justify-end">
            <div class="flex items-center gap-1">
                <p class="font-bold">50</p>
                <ArrowUp size="20px"/>
                
            </div>
    
            <div class="flex items-center gap-1">
                <p class="font-bold">20</p>
                <MessageSquare size="20px"/>
                
            </div>
        </div>
    </div>
    {/each}
</div>