<script>
     import { SearchIcon } from 'svelte-feather-icons'
     let shopeeUrlValue = "https://s.shopee.com.br/"; 
     let shopeeInputValue = ""
     let amazonUrlValue = "https://amzn.to/"; 
     let amazonInputValue = ""
     let mlUrlValue = "https://mercadolivre.com/"; 
     let mlInputValue = ""
</script>

<div id="top" class="pt-20 flex flex-col justify-center items-center mb-20 gap-20">
    <h2 class="text-2xl font-highlight text-center p-5">Prourar produtos por id de url <br> <div class="p-5 text-[10px]" >O que é id de url? <br><br> Um id de url é o número ou código que vêm depois de uma rota base <br><br> Ex.: https://amzn.to/ <b class="text-[8px]" >d3f5E1</b></div></h2>
    <div class="flex  flex-col justify-center items-center gap-[5px] w-full max-w-sm min-w-[200px]">
        <p class="text-xl">Encontre um produto da shopee:</p>
        <img src="https://res.cloudinary.com/dhxmysk03/image/upload/v1741618187/shopee_ixwso8.png" alt="img" class="w-50">
        <input bind:value="{shopeeInputValue}" type="email" class="max-w-80 bg-transparent placeholder:text-slate-400 text-slate-700 text-sm border border-slate-200 rounded-md pl-3 pr-16 py-2 transition duration-300 ease focus:outline-none focus:border-slate-400 hover:border-slate-300 shadow-sm focus:shadow" placeholder="Insira o id aqui" />
        <button class="p-3 underline mt-5 bg-gray rounded-xl animate-pulse">
            <a target="_blank"  href="{shopeeUrlValue + shopeeInputValue}" class="flex justufy-center items-center gap-[5px]"   >
                <p class="">Buscar</p>
                <SearchIcon size="20" />
            </a>
        </button>
    </div>
    <div class="flex  flex-col justify-center items-center gap-[5px] w-full max-w-sm min-w-[200px]">
        <p class="text-xl">Encontre um produto da amazon:</p>
        <img src="https://res.cloudinary.com/dhxmysk03/image/upload/v1741618188/amazon_ly3izq.png" alt="img" class="w-35">
        <input bind:value="{amazonInputValue}" type="email" class="max-w-80 bg-transparent placeholder:text-slate-400 text-slate-700 text-sm border border-slate-200 rounded-md pl-3 pr-16 py-2 transition duration-300 ease focus:outline-none focus:border-slate-400 hover:border-slate-300 shadow-sm focus:shadow" placeholder="Insira o id aqui" />
        <button class="p-3 underline mt-5 bg-gray rounded-xl animate-pulse">
            <a  target="_blank"  href="{amazonUrlValue + amazonInputValue}" class="flex justufy-center items-center gap-[5px]"   >
                <p class="">Buscar</p>
                <SearchIcon size="20" />
            </a>
        </button>
    </div>
    <div class="flex  flex-col justify-center items-center gap-[5px] w-full max-w-sm min-w-[200px]">
        <p class="text-xl">Encontre um produto do mercado livre:</p>
        <img src="https://res.cloudinary.com/dhxmysk03/image/upload/v1741618188/ml_xkyuft.png" alt="img" class="w-40">
        <input bind:value="{mlInputValue}" type="email" class="max-w-80 bg-transparent placeholder:text-slate-400 text-slate-700 text-sm border border-slate-200 rounded-md pl-3 pr-16 py-2 transition duration-300 ease focus:outline-none focus:border-slate-400 hover:border-slate-300 shadow-sm focus:shadow" placeholder="Insira o id aqui" />
        <button class="p-3 underline mt-5 bg-gray rounded-xl animate-pulse">
            <a  target="_blank"  href="{mlUrlValue + mlInputValue}" class="flex justufy-center items-center gap-[5px]"   >
                <p class="">Buscar</p>
                <SearchIcon size="20" />
            </a>
        </button>
    </div>
</div>

