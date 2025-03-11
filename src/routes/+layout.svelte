<script>
	import { InfoIcon,ArrowUpRightIcon } from 'svelte-feather-icons'
	import '../app.css';
	let { children } = $props();
</script>


<div  class="text-black font-base">
	<header class="w-full flex flex-col justify-center items-center gap-10 rounded-b-xl p-20">
		<a href="/">
			<h1 class="font-highlight text-4xl">getachados</h1>
		</a>
		<p class="bg-white text-center" >Produtos internacionais com as menores taxas</p>
		<a href="/id-finder/#top" class="bg-gray px-10 py-5 rounded-xl underline animate-pulse text-center">
			Encontrar produtos por id
		</a>
		<div class="w-full flex justify-center gap-5 items-center">
			<div class="w-40 h-[2px] bg-gray"></div>
			<p>OU</p>
			<div class="w-40 h-[2px] bg-gray"></div>
		</div>
		<p>Acesse diretamente nas lojas:</p>
		<div class="flex flex-wrap justify-center items-center gap-5">
			<a target="_blank" href="https://s.shopee.com.br/9zjW4Pi6uf" class="p-2 border-gray border-5 rounded-xl animate-pulse">
				<img src="https://res.cloudinary.com/dhxmysk03/image/upload/v1741618187/shopee_ixwso8.png" alt="img" class="h-20">
			</a>
			<!-- <a target="_blank"  href="/find/mercado-livre" class="z-40 p-2 border-gray border-5 rounded-xl animate-pulse">
				<img src="https://res.cloudinary.com/dhxmysk03/image/upload/v1741618188/ml_xkyuft.png" alt="img" class="h-20">
			</a> -->
			<a target="_blank" href="/find/amazon" class="p-5 border-gray border-5 rounded-xl ">
				<img src="https://res.cloudinary.com/dhxmysk03/image/upload/v1741618188/amazon_ly3izq.png" alt="img" class="h-14 animate-pulse">
			</a>
		</div>
	</header>
</div>
<main class="font-base w-full h-full">
	{@render children()}
</main>
<footer class="flex flex-col justify-center items-center p-10 text-[15px] w-full gap-5" >
    <div class="flex gap-5 justify-center items-center">
        <a  target="_blank" href="" class="flex justify-center items-center gap-[5px] underline">Acesse o perfil do tiktok<ArrowUpRightIcon size="18" /></a>
    </div>
</footer>




