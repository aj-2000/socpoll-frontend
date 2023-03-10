<script>
  import "../app.css";
  import Sidebar from "../components/Sidebar.svelte";
</script>


<div class="grid grid-cols-6" >
  <Sidebar/>
  <div class="col-span-5 bg-[#141414] h-screen">
    <slot />
  </div>
</div>


