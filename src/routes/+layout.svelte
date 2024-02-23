<script lang="ts">
	
    import "../app.pcss";
    import Nav from "$lib/components/custom/nav.svelte";
    import { ModeWatcher } from "mode-watcher";
    import LightSwitch from "$lib/components/custom/lightswitch.svelte";
    import { AlignJustify } from 'lucide-svelte';
    import { Search } from 'lucide-svelte';
    import { RadioTower, Home, Settings} from 'lucide-svelte';
    import sphIcon from "$lib/icons/VELTE PH.svg";
    import * as Sheet from "$lib/components/ui/sheet";
	import { Button } from "$lib/components/ui/button";

</script>

<ModeWatcher />



<div class="md:flex h-screen">

    <div class="hidden md:flex flex-col md:w-[300px] border-r-2 gap-4 dark:bg-[#242526] ">

            <div class="mt-[200px] flex flex-col gap-4">
                <button class="flex items-center gap-4 p-4  ">
                    <RadioTower />
                    <span class="text-3xl">Forum</span>
                </button>

                <button class="flex items-center gap-4 p-4 ">
                    <Home />
                    <span class="text-3xl">Community</span>
                </button>
    
                <button class="flex items-center gap-4 p-4 ">
                    <Settings />
                    <span class="text-3xl">Account</span>
                </button>
    
                
            </div>
    </div>

    <div class="w-full relative ">
        <nav class="border-b-2 w-full h-[10dvh] p-2  flex items-center justify-between backdrop-blur-sm  ">
            <div class="p-2 bg-[#000000] rounded-xl">
                <img src={sphIcon} class="w-16  " alt="sph-icon" />
            </div>
        
            <div class="flex items-center gap-2"> 
                <Button variant="ghost" size="icon">
                    <Search />
                </Button>
        
                <Sheet.Root>
                    <Sheet.Trigger class="md:hidden">
                        <Button variant="ghost" size="icon">
                            <AlignJustify />
                        </Button>
                    </Sheet.Trigger>
                    
                    <Sheet.Content class="pt-[10dvh] flex flex-col gap-2 justify-center md:hidden" side="left">
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
        
        <div class="flex gap-2 p-2 h-[90dvh]">
            <div class="w-full overflow-auto p-4">
                <slot/>
            </div>

            
                <div class="hidden sticky top-20 md:block w-[300px] border-l-2  h-[500px] p-4 overflow-auto">
                    Lorem ipsum dolor sit amet consectetur, adipisicing elit. Nesciunt ex quae perspiciatis hic iste, voluptatum odio. Ex dolor, ipsa sint sequi quam alias. Nulla nostrum molestias atque incidunt, temporibus magni est minus odit. Repudiandae enim tempora fugiat maiores laborum error, accusamus natus cumque quis! Ipsam reprehenderit accusamus in corrupti ducimus error. Commodi laudantium, delectus dignissimos tempore cum voluptatem quo adipisci eaque non molestiae in dolores quibusdam cumque perspiciatis voluptatibus consectetur nulla! Quasi ex cumque voluptates eum vel molestiae, deserunt, numquam corporis repellat quod ullam atque velit alias vero similique ut suscipit, voluptatum quae omnis. Possimus eveniet repellat molestiae libero quae omnis ipsum! Modi, magni repudiandae? Aliquam optio qui exercitationem aperiam nihil accusantium at molestias neque repellendus corporis velit illo earum consequatur amet dolore est, praesentium ipsum? Enim perferendis quisquam dolor aspernatur! Voluptatum, dolores deserunt. Cum sint adipisci maiores, perspiciatis dolorum labore eius, beatae, vero placeat velit quod? Optio voluptate tempora quo reprehenderit dignissimos provident officia in voluptatibus natus. Placeat earum facere molestiae assumenda nemo ex laboriosam, ea odit dignissimos non eos magnam commodi repellendus iusto possimus accusantium itaque deleniti quae ab reprehenderit architecto totam eius. Aperiam consequuntur nulla modi ipsam quam harum! Quasi, a velit! Dignissimos nam dolores distinctio, et quod exercitationem eaque. Optio magnam numquam at accusantium, possimus corrupti consequatur unde quo nulla, vel, natus rerum provident tenetur similique sapiente sunt voluptatum harum soluta sed fugiat et tempora aliquid facilis hic? Illum eligendi ratione consectetur quam dolore odio quaerat itaque saepe. Asperiores vero eos temporibus facilis a beatae earum dolor necessitatibus eum fuga quos quo commodi ut, tempore pariatur aut modi sit! Soluta incidunt alias at exercitationem fuga ratione odit accusamus perferendis praesentium earum quae laboriosam fugit quis blanditiis, ipsa consequuntur, reprehenderit dolorem illum. Laboriosam, ad optio. Cum, autem unde. Autem, fugit. Optio enim adipisci atque, dolorem qui veritatis, doloremque, modi aliquam autem debitis consequatur recusandae ratione quasi excepturi voluptatibus consequuntur! Officiis explicabo corporis suscipit nulla optio tempora recusandae animi excepturi perspiciatis culpa omnis nobis aliquid officia quas molestiae quos commodi reprehenderit veritatis eius laborum, quia inventore aut aspernatur fugit. Ratione magnam porro optio animi quo laudantium praesentium sunt asperiores doloribus. Mollitia, molestias! Libero maxime, officia earum suscipit atque quidem tempora perferendis natus placeat adipisci unde soluta eius tempore obcaecati recusandae animi saepe, sint dicta at aperiam, ea eligendi! Ut in iusto harum rem dolores repudiandae sed, qui repellat eum culpa? Neque odio repellendus molestias, consequatur provident ducimus dolor a impedit laudantium ea nihil. Nam nulla soluta consectetur sequi est totam earum, doloribus quaerat blanditiis facere facilis cumque asperiores magni excepturi molestiae. Repudiandae autem esse culpa, nesciunt voluptatum sunt sapiente expedita omnis, beatae molestiae sed explicabo animi perferendis, unde voluptatem asperiores harum! Veritatis eligendi in aspernatur amet voluptatum tempora temporibus quia maiores dignissimos! Dignissimos reiciendis similique quos a dolore error vero quasi commodi sed vel aperiam maxime blanditiis fuga distinctio nihil quo fugit, eius at eum! Fugiat, nesciunt voluptate. Aperiam veritatis voluptatem assumenda, magni unde laboriosam reprehenderit delectus laborum facilis ex sapiente quia inventore ipsa dolorum? Voluptatem, tempore labore consequuntur voluptate sed quo iste deserunt omnis rem magnam tempora sint quibusdam possimus rerum sapiente, aperiam neque, debitis impedit optio ea! Sunt hic esse temporibus, praesentium porro minima illo nihil natus ipsum? Atque tempora facere facilis itaque laborum, sequi quod obcaecati hic eligendi tempore quas perferendis, exercitationem laudantium eveniet dolore vel incidunt quam a. Sint a recusandae blanditiis illum delectus libero quos quas adipisci sit dicta fuga quam natus perferendis minima qui impedit corrupti, distinctio dolorem exercitationem aspernatur voluptas, doloribus vero iure? Harum cumque aliquam sunt obcaecati quam laboriosam cupiditate, sapiente quibusdam suscipit tenetur illo nisi excepturi quidem corporis minima, quis totam placeat ipsam sed magni! Commodi minima delectus harum in obcaecati cupiditate laboriosam nulla reprehenderit eius. Cumque, dicta pariatur qui ut natus necessitatibus repudiandae et porro a alias, illum temporibus quas ipsum eveniet officiis, recusandae fugit corporis quidem vitae ratione maxime reiciendis nemo dolore. Iste, aut quaerat. Aut delectus molestiae est officiis, at placeat deleniti fuga beatae quisquam animi quidem, dignissimos, eveniet reiciendis voluptatem. Voluptatibus accusantium at odit a quos aliquam itaque quisquam eum earum quaerat doloribus est quia quod, debitis cupiditate ex quam aliquid molestias soluta voluptas accusamus rerum? Iure magnam in impedit eveniet architecto assumenda nulla ad nostrum animi! Non numquam qui tempore dignissimos dolores excepturi quod cupiditate dolorem adipisci recusandae architecto consectetur quidem nobis dolore odio perspiciatis quia id molestiae nisi porro fugit, labore praesentium hic temporibus. Nulla corporis iusto neque quis animi. Eos debitis odio quis illo, maxime dignissimos aperiam fugit aspernatur soluta ipsam minima beatae quia expedita unde eveniet iusto suscipit vero facere iure nesciunt magnam commodi quam. Odio consequatur optio impedit ducimus dignissimos nisi amet esse dolores corporis maiores. Ea cumque perferendis natus officia iusto soluta et autem odio aspernatur? Delectus distinctio tempore eius, asperiores voluptatem incidunt, sunt natus ex sed quia minus voluptate odit, rem saepe? Et aperiam sed, dolore in ad atque iusto quaerat. Laudantium, cum cumque.
                </div>
            
        </div>
    </div>
</div>
            
        
            


