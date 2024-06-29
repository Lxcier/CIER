<script>
import Glide from '@glidejs/glide';

import Button from '@/components/Global/Button.vue';

export default {
  name: 'MainGlide',
  components: {
    Button,
  },
  mounted() {
    new Glide('.glide', {
      type: 'carousel',
      startAt: 0,
      perView: 1,
      autoplay: 10000,
      animationDuration: 700,
      animationTimingFunc: 'ease'
    }).mount();
  }
};
</script>

<template>
  <div class="glide">
    <div class="glide__track" data-glide-el="track">
      <ul class="glide__slides">
        <li class="glide__slide">

          <img class="glide__image" src="@/assets/images/vetores/ux-ui.jpg" alt="ux/ui vetor">

          <div class="glide__text">
            <div class="headline">
              <h2 class="title-big text-highlight">ux/ui</h2>
              <p class="subtitle">O espirito do seu negócio virtual</p>
            </div>
            <p class="text">Seu site ou aplicativo é bonito, mas será que ele é realmente <span class="text-highlight">amigável</span>?</p>
            <p class="text">Com um serviço de <span class="text-highlight">ux/ui</span>, você pode:</p>

            <ul class="list">
              <li class="list-item text">Aumentar as taxas de conversão e vendas</li>
              <li class="list-item text">Melhorar a experiência do usuário e fidelizá-los</li>
              <li class="list-item text">Reduzir o número de desistências e não frustrar usuários</li>
              <li class="list-item text">Criar um produto intuitivo e eficaz</li>
            </ul>

            <Button class="slide__button" cta="Transformar experiência"/>
          </div>
        </li>
        <li class="glide__slide">

          <img class="glide__image" src="@/assets/images/vetores/edicao.jpg" alt="edição de vídeo/imagens vetor">

          <div class="glide__text">
            <div class="headline">
              <h2 class="title-big text-highlight">Edição</h2>
              <p class="subtitle">Dê um toque especial em seus conteúdos</p>
            </div>
            <p class="text">Seu site ou aplicativo é bonito, mas será que ele é realmente <span class="text-highlight">amigável</span>?</p>
            <p class="text">Com um serviço de <span class="text-highlight">ux/ui</span>, você pode:</p>

            <ul class="list">
              <li class="list-item text">Aumentar as taxas de conversão e vendas</li>
              <li class="list-item text">Melhorar a experiência do usuário e fidelizá-los</li>
              <li class="list-item text">Reduzir o número de desistências e não frustrar usuários</li>
              <li class="list-item text">Criar um produto intuitivo e eficaz</li>
            </ul>

            <Button class="slide__button" cta="Transformar experiência"/>
          </div>
        </li>
        <li class="glide__slide">

          <img class="glide__image" src="@/assets/images/vetores/web-design.jpg" alt="web design vetor">

          <div class="glide__text">
            <div class="headline">
              <h2 class="title-big text-highlight">Web Design</h2>
              <p class="subtitle">Dê um toque especial em seus conteúdos</p>
            </div>
            <p class="text">Seu site ou aplicativo é bonito, mas será que ele é realmente <span class="text-highlight">amigável</span>?</p>
            <p class="text">Com um serviço de <span class="text-highlight">ux/ui</span>, você pode:</p>

            <ul class="list">
              <li class="list-item text">Aumentar as taxas de conversão e vendas</li>
              <li class="list-item text">Melhorar a experiência do usuário e fidelizá-los</li>
              <li class="list-item text">Reduzir o número de desistências e não frustrar usuários</li>
              <li class="list-item text">Criar um produto intuitivo e eficaz</li>
            </ul>

            <Button class="slide__button" cta="Transformar experiência"/>
          </div>
        </li>
        <li class="glide__slide">

          <img class="glide__image" src="@/assets/images/vetores/seo.jpg" alt="SEO vetor">

          <div class="glide__text">
            <div class="headline">
              <h2 class="title-big text-highlight">SEO</h2>
              <p class="subtitle">Dê um toque especial em seus conteúdos</p>
            </div>
            <p class="text">Seu site ou aplicativo é bonito, mas será que ele é realmente <span class="text-highlight">amigável</span>?</p>
            <p class="text">Com um serviço de <span class="text-highlight">ux/ui</span>, você pode:</p>

            <ul class="list">
              <li class="list-item text">Aumentar as taxas de conversão e vendas</li>
              <li class="list-item text">Melhorar a experiência do usuário e fidelizá-los</li>
              <li class="list-item text">Reduzir o número de desistências e não frustrar usuários</li>
              <li class="list-item text">Criar um produto intuitivo e eficaz</li>
            </ul>

            <Button class="slide__button" cta="Transformar experiência"/>
          </div>
        </li>
        <li class="glide__slide">

          <img class="glide__image" src="@/assets/images/vetores/marketing-digital.jpg" alt="marketing digital vetor">

          <div class="glide__text">
            <div class="headline">
              <h2 class="title-big text-highlight">Marketing Digital</h2>
              <p class="subtitle">Dê um toque especial em seus conteúdos</p>
            </div>
            <p class="text">Seu site ou aplicativo é bonito, mas será que ele é realmente <span class="text-highlight">amigável</span>?</p>
            <p class="text">Com um serviço de <span class="text-highlight">ux/ui</span>, você pode:</p>

            <ul class="list">
              <li class="list-item text">Aumentar as taxas de conversão e vendas</li>
              <li class="list-item text">Melhorar a experiência do usuário e fidelizá-los</li>
              <li class="list-item text">Reduzir o número de desistências e não frustrar usuários</li>
              <li class="list-item text">Criar um produto intuitivo e eficaz</li>
            </ul>

            <Button class="slide__button" cta="Transformar experiência"/>
          </div>
        </li>
      </ul>

      <div class="glide__arrows" data-glide-el="controls">
        <button class="glide__arrow glide__arrow--left" data-glide-dir="<">
          <i class="fa-solid fa-chevron-left"></i>
        </button>
        <button class="glide__arrow glide__arrow--right" data-glide-dir=">">
          <i class="fa-solid fa-chevron-right"></i>
        </button>
      </div>
    </div>
  </div>
</template>

<style scoped>
  .glide {
    margin-top: 3.3rem;
  }

  .glide__track {
    margin: 0 auto;
    width: calc(100% - 10rem);
    border-radius: 2.0rem;
  }

  .glide__slide {
    background: var(--branco);
    width: fit-content;
    
    display: flex;
    justify-content: space-around;
    
    border-radius: 2.0rem;
    padding: 1.8rem 3.2rem;
  }

  .glide__arrow {
    background: transparent;
    border: none;
    cursor: pointer;

    color: var(--cor-principal);
    font-size: 2rem;

    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    transition: all ease-in-out .23s;

    &:hover {
      background-color: var(--cor-secundaria);
      padding: .4rem .9rem;
      border-radius: 100px;
    }
  }

  .glide__arrow--left {
    left: 2%;

    &:hover {
      transform: translateY(-50%) translateX(-60%);
      font-size: 2.2rem;
    }
  }

  .glide__arrow--right {
    right: 2%;

    &:hover {
      transform: translateY(-50%) translateX(60%);
      font-size: 2.2rem;
    }
  }
  
  .glide__image {
    width: 40rem;
    height: 40rem;
    max-width: 40rem;
    max-height: 40rem;
  }

  .glide__text {
    display: flex;
    flex-direction: column;
    margin-top: 2.8rem;

    gap: 1.2rem;
  }

  .title-big {
    font-size: 3.8rem;
    text-transform: uppercase;
  }

  .subtitle {
    color: var(--cor-secundaria);
    font-weight: 600;
    font-size: 1.8rem;
  }

  .text {
    color: #010101;
  }

  .list {
    list-style: inside;
    display: flex;
    flex-direction: column;
    gap: 1.2rem;
  }

  .list-item {
		color: var(--cor-principal);
    font-weight: 600;
	}

  .slide__button {
    margin-top: 2.4rem;

    &:hover {
      color: var(--cor-secundaria)
    }
  }
</style>