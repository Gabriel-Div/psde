<template>
    <div class="min-h-screen bg-white">
        <div class="w-full text-center">
            <img class="w-full" alt="Header" src="../../images/8.png" />
        </div>
        <div class="w-full flex justify-center items-center text-center hidden lg:block">
            <a href="#content">
                <svg class="animation-down" width="124" height="110" viewBox="0 0 24 24" fill="none"
                    xmlns="http://www.w3.org/2000/svg" style="margin-top: -20px;">
                    <path d="M6 10L12 16L18 10H6Z" fill="blue" />
                </svg>
            </a>

        </div>
        <div class="relative overflow-hidden px-6 py-6 lg:px-8 mt-3" id="content">
            <div class="mx-auto max-w-7xl grid grid-cols-1 gap-16 lg:grid-cols-2">
                <div class="max-w-lg">
                    <h1 class="mt-2 text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl">
                        Construindo um Futuro Melhor para o Brasil
                    </h1>
                    <p class="mt-6 text-xl leading-8 text-gray-700">
                        O PSDE está comprometido com a promoção do crescimento econômico, inclusão social e
                        fortalecimento das instituições. Junte-se a nós na criação de um futuro mais brilhante e
                        sustentável.
                    </p>
                </div>

                <div class="relative lg:-ml-12 w-full">
                    <img class="w-full max-w-none rounded-xl bg-gray-900 shadow-xl ring-1 ring-gray-400/10"
                        src="../../images/goiania.jpg" alt="Cidade Sustentável">
                </div>
                <div>
                    <div class="max-w-lg">
                        <p class="text-base leading-7 text-gray-700">
                            O PSDE é um projeto visionário que busca equilibrar o progresso econômico com a equidade
                            social. Acreditamos em um Brasil onde as instituições sejam fortalecidas e todos os cidadãos
                            tenham a oportunidade de prosperar.
                        </p>
                        <ul role="list" class="mt-8 space-y-8 text-gray-600">
                            <li class="flex gap-x-3">
                                <svg class="h-6 w-6 text-green-600" fill="currentColor" viewBox="0 0 24 24">
                                    <path
                                        d="M12 2a10 10 0 100 20 10 10 0 000-20zm-1 14.93V13H7.07A8.025 8.025 0 0111 4.07v7.86h7.93A8.025 8.025 0 0111 16.93z">
                                    </path>
                                </svg>
                                <span><strong class="font-semibold text-gray-900">Desenvolvimento Sustentável</strong>
                                    Priorizamos políticas ecológicas que garantam o crescimento econômico sem
                                    comprometer o meio ambiente.</span>
                            </li>
                            <li class="flex gap-x-3">
                                <svg class="h-6 w-6 text-blue-600" fill="currentColor" viewBox="0 0 24 24">
                                    <path d="M12 2a10 10 0 100 20 10 10 0 000-20zm0 18a8 8 0 110-16 8 8 0 010 16z">
                                    </path>
                                    <path d="M13 7h-2v6h6v-2h-4z"></path>
                                </svg>
                                <span><strong class="font-semibold text-gray-900">Inclusão Social</strong> Nossa missão
                                    é criar políticas inclusivas que unam todos os brasileiros, garantindo oportunidades
                                    iguais para todos.</span>
                            </li>
                            <li class="flex gap-x-3">
                                <svg class="h-6 w-6 text-yellow-600" fill="currentColor" viewBox="0 0 24 24">
                                    <path
                                        d="M12 2a10 10 0 100 20 10 10 0 000-20zM12 4c1.1046 0 2 .8954 2 2s-.8954 2-2 2-2-.8954-2-2 .8954-2 2-2zm0 14c-2.6667 0-5.2-1.3333-6.67-3.667C6.44 13.18 7.18 12 12 12s5.56 1.18 6.67 2.333C17.2 16.667 14.6667 18 12 18z">
                                    </path>
                                </svg>
                                <span><strong class="font-semibold text-gray-900">Fortalecimento Institucional</strong>
                                    Trabalhamos para instituições públicas robustas que possam servir e proteger
                                    efetivamente o povo brasileiro.</span>
                            </li>
                        </ul>
                        <p class="mt-8 text-base leading-7 text-gray-700">
                            Junte-se a nós em nossa jornada para construir um Brasil próspero, inclusivo e sustentável.
                        </p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style>
body,
html {
    scroll-behavior: smooth;
}


@keyframes GoUpDown {
    0% {
        transform: translateY(-10%);
    }

    50% {
        transform: translateY(10%);
    }

    100% {
        transform: translateY(-10%);
    }
}

.animation-down {
    display: inline-block;
    animation: GoUpDown 1s infinite;
    cursor: pointer;
}
</style>