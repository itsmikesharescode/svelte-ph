<script lang="ts">
    import { Separator } from "$lib/components/ui/separator";
    import * as Card from "$lib/components/ui/card";
    import { Badge } from "$lib/components/ui/badge";
    import * as Avatar from "$lib/components/ui/avatar";
    import { MessageSquare, ArrowUp } from 'lucide-svelte';
	import Button from "$lib/components/ui/button/button.svelte";
</script>

<div class="mt-5">
    <h1 class="scroll-m-20 text-4xl font-extrabold tracking-tight lg:text-5xl ">
        Svelte PH 
    </h1>

    <h2 class="text-xl text-muted-foreground">
        Is Home for web developers.
    </h2>
</div>

<Separator class="mt-5"/>

<div class="mt-5">
    <h4 class="scroll-m-20 text-xl font-semibold tracking-tight">
        Recent blog posts
    </h4>

    <div class="mt-5 flex flex-col gap-4">
        <div class="">
            <Card.Root class="">
                <Card.Header>

                    <div class="flex items-center gap-4">
                        <Avatar.Root class="">
                            <Avatar.Image src="https://github.com/shadcn.png" alt="@shadcn" />
                            <Avatar.Fallback>CN</Avatar.Fallback>
                        </Avatar.Root>
                        
                        <div class="">
                            <p class="font-bold">Thomas Edison</p>
                            <p class="text-muted-foreground font-thin">Posted 5 hours ago.</p>
                        </div>
                    </div>

                </Card.Header>
        
                <Card.Content>
                    <div class="line-clamp-6 overflow-hidden">
                        <p class="leading-7 [&:not(:first-child)]:mt-6">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Qui, vero. Quasi eos ipsum minus provident dolorum recusandae natus id omnis, eligendi, sed quae possimus dolores nobis? Ratione, ipsum sed voluptate asperiores minus cupiditate maxime ad facilis provident illum officiis, eum vitae voluptatum nostrum id eos! Sit atque nesciunt eius facilis minus quis distinctio minima, reprehenderit officiis accusantium qui adipisci ipsum aliquid soluta corporis nulla asperiores temporibus suscipit, beatae illum libero, eaque in. Possimus velit vitae numquam blanditiis molestias sed, magnam architecto ipsum sunt, consequuntur consequatur distinctio tempora illum minus neque suscipit et culpa laboriosam nam nulla temporibus quod sint fuga a? Cupiditate impedit aspernatur maiores aliquam. Dolorum officia inventore minus sit repudiandae sapiente ratione molestiae, labore atque suscipit quibusdam odio aspernatur ea sunt error non porro quos a. Quas eum, cum blanditiis veritatis nostrum quia totam, corporis alias minus cumque et ex placeat, vel consequuntur nobis nam sint quod. Ex dolorem sit expedita, nihil est non earum alias recusandae commodi nemo! Omnis quod vel, amet debitis eius sapiente asperiores porro hic voluptatibus mollitia. Illo, esse necessitatibus nobis voluptates aliquid unde doloremque omnis cumque. Quisquam iure inventore maxime neque hic amet non quae dignissimos. Mollitia eum, dicta quibusdam quaerat veritatis amet at perferendis asperiores quae! Similique, in impedit eveniet odio error nobis excepturi, amet rem voluptas ex incidunt! Exercitationem iure sint ex illo molestias eos, rerum asperiores inventore temporibus voluptate repudiandae, saepe ullam voluptates! Iusto ad blanditiis, consequatur recusandae odio similique numquam ipsum sunt, deleniti exercitationem atque? Voluptas consequatur itaque molestiae alias doloremque tempora animi laudantium ex dolor placeat quam illum quasi libero quo quidem sed, sapiente aliquid odio iusto inventore. Magni voluptatum enim numquam adipisci reiciendis ex perferendis odit laudantium totam, quibusdam blanditiis veritatis sunt vero commodi necessitatibus dolorem unde porro atque pariatur similique ab iusto? Obcaecati voluptate cupiditate pariatur officia, veniam aliquam est reprehenderit cum quia iure sed assumenda quaerat? Et neque, incidunt dolorem consequuntur facilis autem mollitia quisquam atque, eligendi maiores eum ab velit. Numquam tempora mollitia facilis, delectus illo obcaecati facere. Vel architecto praesentium quis aut explicabo. Similique praesentium assumenda porro non totam magnam, molestiae rerum veniam corporis distinctio fuga, sunt tenetur aut nihil ad consequatur quae atque laudantium facere repellat quo odit consectetur! Exercitationem tenetur ipsam consequatur? Veritatis praesentium et incidunt modi, iusto rerum inventore pariatur, dolore doloribus at sunt! Consectetur dolorem voluptate molestias nam voluptas quasi nesciunt debitis. Deserunt, sint! Neque maxime fugit eum. Eius hic id a cupiditate. Perferendis laborum expedita nemo porro! Nulla enim cumque odit repudiandae accusantium totam, eveniet labore temporibus nam inventore aspernatur? Ut magni, beatae rerum error corrupti ducimus impedit inventore unde voluptates voluptate. Aperiam dolores cum praesentium consequatur iure placeat inventore quia maiores fugiat eos! Veniam officiis ab aliquam modi ipsum dolorem dignissimos numquam voluptatibus? Quos, et magni omnis voluptatum hic ipsa at possimus? Tempore velit ex expedita in aperiam, doloremque unde laudantium iusto deleniti blanditiis saepe nihil fugit nostrum corporis architecto totam iste accusamus, sit minima eius eos nisi. Corrupti cumque sunt voluptatibus cum veniam hic reprehenderit deleniti!</p>
                    </div>
                </Card.Content>
                
                <Card.Footer class="flex justify-end">
                    <Button size="sm" variant="ghost" class="flex items-center gap-2">
                        <ArrowUp size="25px" />
                        1008
                    </Button>

                    <Button size="sm" variant="ghost" class="flex items-center gap-2">
                        <MessageSquare size="25px" />
                        60
                    </Button>
                </Card.Footer>
            </Card.Root>
        </div>

        <div class="flex gap-2 items-center">
            <Badge>Latest News</Badge>
            <Badge>Programming</Badge>
            <Badge>Personal</Badge>
        </div>

        <div class="h-[250px] overflow-y-auto overflow-x-hidden flex flex-col gap-2">
            {#each ["", "","", "","", "","", "",] as sample }
                <Card.Root class="">
                    <Card.Header>

                        <div class="flex items-center gap-4">
                            <Avatar.Root>
                                <Avatar.Image src="https://github.com/shadcn.png" alt="@shadcn" />
                                <Avatar.Fallback>CN</Avatar.Fallback>
                            </Avatar.Root>
                            
                            <div class="">
                                <p class="font-bold">Thomas Edison</p>
                                <p class="text-muted-foreground font-thin">Posted 5 hours ago.</p>
                            </div>
                        </div>

                    </Card.Header>
            
                    <Card.Content>
                        <div class="line-clamp-1 overflow-hidden">
                            <p class="leading-7 [&:not(:first-child)]:mt-6">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Qui, vero. Quasi eos ipsum minus provident dolorum recusandae natus id omnis, eligendi, sed quae possimus dolores nobis? Ratione, ipsum sed voluptate asperiores minus cupiditate maxime ad facilis provident illum officiis, eum vitae voluptatum nostrum id eos! Sit atque nesciunt eius facilis minus quis distinctio minima, reprehenderit officiis accusantium qui adipisci ipsum aliquid soluta corporis nulla asperiores temporibus suscipit, beatae illum libero, eaque in. Possimus velit vitae numquam blanditiis molestias sed, magnam architecto ipsum sunt, consequuntur consequatur distinctio tempora illum minus neque suscipit et culpa laboriosam nam nulla temporibus quod sint fuga a? Cupiditate impedit aspernatur maiores aliquam. Dolorum officia inventore minus sit repudiandae sapiente ratione molestiae, labore atque suscipit quibusdam odio aspernatur ea sunt error non porro quos a. Quas eum, cum blanditiis veritatis nostrum quia totam, corporis alias minus cumque et ex placeat, vel consequuntur nobis nam sint quod. Ex dolorem sit expedita, nihil est non earum alias recusandae commodi nemo! Omnis quod vel, amet debitis eius sapiente asperiores porro hic voluptatibus mollitia. Illo, esse necessitatibus nobis voluptates aliquid unde doloremque omnis cumque. Quisquam iure inventore maxime neque hic amet non quae dignissimos. Mollitia eum, dicta quibusdam quaerat veritatis amet at perferendis asperiores quae! Similique, in impedit eveniet odio error nobis excepturi, amet rem voluptas ex incidunt! Exercitationem iure sint ex illo molestias eos, rerum asperiores inventore temporibus voluptate repudiandae, saepe ullam voluptates! Iusto ad blanditiis, consequatur recusandae odio similique numquam ipsum sunt, deleniti exercitationem atque? Voluptas consequatur itaque molestiae alias doloremque tempora animi laudantium ex dolor placeat quam illum quasi libero quo quidem sed, sapiente aliquid odio iusto inventore. Magni voluptatum enim numquam adipisci reiciendis ex perferendis odit laudantium totam, quibusdam blanditiis veritatis sunt vero commodi necessitatibus dolorem unde porro atque pariatur similique ab iusto? Obcaecati voluptate cupiditate pariatur officia, veniam aliquam est reprehenderit cum quia iure sed assumenda quaerat? Et neque, incidunt dolorem consequuntur facilis autem mollitia quisquam atque, eligendi maiores eum ab velit. Numquam tempora mollitia facilis, delectus illo obcaecati facere. Vel architecto praesentium quis aut explicabo. Similique praesentium assumenda porro non totam magnam, molestiae rerum veniam corporis distinctio fuga, sunt tenetur aut nihil ad consequatur quae atque laudantium facere repellat quo odit consectetur! Exercitationem tenetur ipsam consequatur? Veritatis praesentium et incidunt modi, iusto rerum inventore pariatur, dolore doloribus at sunt! Consectetur dolorem voluptate molestias nam voluptas quasi nesciunt debitis. Deserunt, sint! Neque maxime fugit eum. Eius hic id a cupiditate. Perferendis laborum expedita nemo porro! Nulla enim cumque odit repudiandae accusantium totam, eveniet labore temporibus nam inventore aspernatur? Ut magni, beatae rerum error corrupti ducimus impedit inventore unde voluptates voluptate. Aperiam dolores cum praesentium consequatur iure placeat inventore quia maiores fugiat eos! Veniam officiis ab aliquam modi ipsum dolorem dignissimos numquam voluptatibus? Quos, et magni omnis voluptatum hic ipsa at possimus? Tempore velit ex expedita in aperiam, doloremque unde laudantium iusto deleniti blanditiis saepe nihil fugit nostrum corporis architecto totam iste accusamus, sit minima eius eos nisi. Corrupti cumque sunt voluptatibus cum veniam hic reprehenderit deleniti!</p>
                        </div>
                    </Card.Content>
                    
                    <Card.Footer class="flex justify-end">
                        <Button size="sm" variant="ghost" class="flex items-center gap-2">
                            <ArrowUp size="25px" />
                            1008
                        </Button>

                        <Button size="sm" variant="ghost" class="flex items-center gap-2">
                            <MessageSquare size="25px" />
                            60
                        </Button>
                    </Card.Footer>
                </Card.Root>
            {/each}
        </div>

        
    </div>
</div>