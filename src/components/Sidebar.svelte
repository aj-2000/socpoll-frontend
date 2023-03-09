
<script lang="ts">
import Icon from '@iconify/svelte';
</script>

<div class="col-span-1 bg-black text-white h-screen py-6 px-4">
    <div class="flex flex-col justify-between h-full ">
        <div class="flex flex-col gap-6 h-full">
            <div class="text-4xl font-bold italic py-6 cursor-pointer">
                SocPoll
            </div>
            <div class="flex gap-4 items-center cursor-pointer">
               <Icon class="text-4xl text"  icon="material-symbols:home" />
               <span class="text-md font-semibold">Home</span>
            </div>
            <div class="flex gap-4 items-center cursor-pointer">
               <Icon class="text-4xl text"  icon="material-symbols:explore" />
               <span class="text-md font-semibold">Explore</span>
            </div>
            <div class="flex gap-4 items-center cursor-pointer">
               <Icon class="text-4xl text"  icon="jam:messages-f" />
               <span class="text-md font-semibold">Messages</span>
            </div>
            <div class="flex gap-4 items-center cursor-pointer">
               <Icon class="text-4xl text"  icon="system-uicons:create" />
               <span class="text-md font-semibold">Create</span>
            </div>
            <div class="flex gap-4 items-center cursor-pointer">
               <Icon class="text-4xl text"  icon="gg:profile" />
               <span class="text-md font-semibold">Profile</span>
            </div>
         </div>
        <div class="flex gap-4 items-center cursor-pointer">
            <Icon class="text-4xl text"  icon="charm:menu-hamburger" />
            <span class="text-md font-semibold">More</span>
        </div>
    </div>
</div>