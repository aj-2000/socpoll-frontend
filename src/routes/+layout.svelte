<script>
  import "../app.css";
  import { applyAction, enhance } from '$app/forms'
  import { invalidateAll } from '$app/navigation'
  import { page } from '$app/stores'
  import Sidebar from "../components/Sidebar.svelte";
</script>

  {#if !$page.data.user}
     <slot />
  {/if}

{#if $page.data.user}
<div class="grid grid-cols-6" >
  <Sidebar/>
  <div class="col-span-5 bg-[#141414] h-screen">
    <slot />
  </div>
</div>
{/if}


