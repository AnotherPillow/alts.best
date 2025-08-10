<script lang="ts">
    let { url, img, title, small = undefined } = $props();
</script>

<a
    class="w-72 h-72 bg-zinc-800 rounded-md border-zinc-700 border-6 filter hover:brightness-80 cursor-pointer p-4 relative overflow-hidden"
    href={url}
    target="_blank"
>
    <div
        class="absolute inset-0 hover:mt-[-16px] bg-no-repeat bg-cover bg-top transition-all"
        style={`background-image: url(${img});`}
    ></div>

    <div
        class="bg-zinc-700 z-20 absolute left-0 bottom-0 right-0 h-20 flex justify-center flex-col"
    >
        <h2 class="text-xl font-bold text-center">{title}</h2>
        {#if small}
            <p class="text-center text-xm text-neutral-400">{small}</p>
        {/if}
    </div>
</a>