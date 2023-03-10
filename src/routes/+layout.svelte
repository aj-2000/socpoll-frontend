<script>
  import "../app.css";
  import { applyAction, enhance } from '$app/forms'
  import { invalidateAll } from '$app/navigation'
  import { page } from '$app/stores'
  import Sidebar from "../components/Sidebar.svelte";
</script>

<nav>
  {#if !$page.data.user}
    <a href="/login">Login</a>
    <a href="/register">Register</a>
  {/if}

  {#if $page.data.user}
    <a href="/admin">Admin</a>

<form
  action="/logout"
  method="POST"
  use:enhance={() => {
    return async ({ result }) => {
      invalidateAll()
      await applyAction(result)
    }
  }}
>
      <button type="submit">Log out</button>
    </form>
  {/if}
</nav>

<div class="grid grid-cols-6" >
  <Sidebar/>
  <div class="col-span-5 bg-[#141414] h-screen">
    <slot />
  </div>
</div>


