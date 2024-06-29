<script>
import Glide from '@glidejs/glide';

import Button from '@/components/Global/Button.vue';

import Image1 from '@/assets/images/vetores/ux-ui.jpg';
import Image2 from '@/assets/images/vetores/edicao.jpg';

export default {
  name: 'MainGlide',
  components: {
    Button
  },
  data() {
    return {
      slides: [
        {
          id: 1,
          image: Image1,
          title: 'Ux/Ui',
          subtitle: 'O espirito do seu negócio virtual',
          paragraph: 'Seu site ou aplicativo é bonito, mas será que ele é realmente amigável?',
          paragraph1: 'Com um serviço de ux/ui, você pode:',
          listItem: [
            {
              item1: 'Aumentar as taxas de conversão e vendas',
              item2: 'Melhorar a experiência do usuário e fidelizá-los',
              item3: 'Reduzir o número de desistências e frustrar usuários',
              item4: 'Criar um produto intuitivo e eficaz'
            }
          ]
        },
        {
          id: 2,
          image: Image2,
          title: 'Edição',
          subtitle: 'Dê um toque especial nos seus conteúdos',
          paragraph: 'Seu site ou aplicativo é bonito, mas será que ele é realmente amigável?',
          paragraph1: 'Com um serviço de ux/ui, você pode:',
          listItem: [
            {
              item1: 'Aumentar as taxas de conversão e vendas',
              item2: 'Melhorar a experiência do usuário e fidelizá-los',
              item3: 'Reduzir o número de desistências e frustrar usuários',
              item4: 'Criar um produto intuitivo e eficaz'
            }
          ]
        }
      ]
    };
  },
  mounted() {
    new Glide('.glide', {
      type: 'carousel',
      startAt: 0,
      perView: 1,
      autoplay: 3000,
      animationDuration: 1000,
      animationTimingFunc: 'ease-in-out'
    }).mount();
  }
};
</script>

<template>
  <div class="glide">
    <div class="glide__track" data-glide-el="track">
      <ul class="glide__slides">
        <li class="glide__slide" v-for="slide in slides" :key="slide.id">
          <img class="glide__image" :src="slide.image" :alt="slide.title" />
          <div class="headline">
            <h2 class="title-big text-highlight">{{ slide.title }}</h2>
            <p class="subtitle">{{ slide.subtitle }}</p>
          </div>
          <p class="text">{{ slide.paragraph }}</p>
          <p class="text">{{ slide.paragraph1 }}</p>
        </li>
      </ul>
    </div>
  </div>
</template>

<style scoped>
  .glide {
    padding: 0.8rem;
    margin-top: 3.3rem;
  }

  .glide__track {
    margin: 0 auto;
    width: calc(100% - 10rem)
  }
  
  .glide__image {
    width: 50rem;
    height: 50rem;
  }

  .glide__slide {
    background: var(--branco);
    width: fit-content;

    display: flex;
    align-items: center;
    gap: 3.2rem;

    border-radius: 5rem;

  }

  .title-big {
    text-transform: uppercase;
  }

  .subtitle {
    color: var(--cor-secundaria);
    font-weight: 600;
  }
</style>