<script setup lang="ts">

    import './OrientationPage.css'

    import { createScrollRevealDirective } from 'vue-scroll-reveal'; 
        const vScrollReveal = createScrollRevealDirective({
        delay: 1000,
        duration: 150,
    });

</script>

<template>
    <div id="container_OrientationPage">
        <main>
            <article v-scroll-reveal="{delay: 200, duration: 1000, distance: '150px', origin: 'left', scale: 1.2}">
                <div class="titles">
                    <h1>Como posso fazer o descarte consiente dos meus <span>sabonetes</span>.</h1>
                </div>
                <div id="description">
                    <p>Uma iniciativa da <span>ARTSABOARIA LTDA</span>, com o proposito de diminuir o descarte incorreto dos sabonetes que provoca danos para o meio ambiente</p>
                </div>
                <div class="titles">
                    <h1>Formas devidas</h1>
                </div>
                <ol start="1">
                    <li>Usar o sabonete até o fim</li>
                    <li>Reciclar o sabonete</li>
                    <li>Compostagem</li>
                    <li>Reutilização criativa</li>
                    <li>Evite embalagens desnecessárias</li>
                </ol>
            </article>
            <aside v-scroll-reveal="{delay: 200, duration: 1000, distance: '150px', origin: 'right', scale: 1.2}">
                <img src="../../assets/images/Imagem ilustrativa.svg" alt="">
            </aside>
        </main>
    </div>
</template>