
<script>
    import Card from "$lib/components/Card.svelte";
    import SaleBanner from "$lib/components/SaleBanner.svelte";
</script>


<main class="relative w-full min-h-screen font-[Lato] bg-gradient-to-br from-pink-800 via-fuchsia-900 to-purple-950">
    <div class="absolute inset-0 bg-black/70 z-10"></div>    
    <SaleBanner />
    
    <div class="relative z-50 text-white w-full min-h-screen flex justify-center items-center flex-col py-12">
        <a href="/" target="_self" class="hover:text-decoration-line filter hover:brightness-80">
            <h1 class="text-6xl font-bold mb-12">alts.<span class="text-rose-300">best</span></h1>
        </a>

        <div class="flex justify-center items-center gap-8 flex-wrap max-w-6xl px-4">
            <Card 
                url="https://www.minecraft.net/store/minecraft-java-bedrock-edition-pc"
                img="https://www.minecraft.net/content/dam/minecraftnet/games/minecraft/key-art/PDP-Hero_OV-Standard_16x9.jpg"
                title="Minecraft Java & Bedrock"
                small="Full MSA OGI & TID."
            />
            <Card 
                url="https://feverup.com/m/282847"
                img="https://minecraft.wiki/images/Minecraft_Experience_Key_Art.jpg"
                small="From £22"
                title="MCE Villager Rescue Cape"
            />
            <Card 
                url="https://www.ticketek.com.ar/minecraft-experience/ciudad-universitaria"
                img="https://minecraft.wiki/images/thumb/Minecraft_Experience_Moonlight_Trail_Key_Art.jpg/300px-Minecraft_Experience_Moonlight_Trail_Key_Art.jpg?afe94"
                title="MCE Moonlight Trail Cape"
            />
            <!-- yes i'm aware it's on variety.com if you have the original source/one from xbox just tell me -->
            <Card 
                url="https://www.xbox.com/en-US/xbox-game-pass"
                img="https://variety.com/wp-content/uploads/2021/06/Game-Pass.jpg" 
                small="No name set. Full access. From $1"
                title="Xbox Game Pass"
            />
        </div>
    </div>
</main>