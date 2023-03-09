<script lang="ts">
    import Icon from '@iconify/svelte';
    export let icon = ""
    export let title = ""
</script>

<div class="flex gap-4 items-center cursor-pointer">
    <Icon class="text-4xl text"  icon={icon} />
    <span class="text-md font-semibold">{title}</span>
</div>