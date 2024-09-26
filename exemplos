
Aqui estão exemplos práticos de algumas das principais funções (diretivas) que mencionei anteriormente no contexto do Vue.js, para que você possa ver como elas funcionam na prática.

1. v-bind
Vincula um atributo HTML a uma expressão Vue.


<template>
  <div>
        <img v-bind:src="imagemURL" alt="Imagem dinâmica">
    <!-- Atributo dinâmico para o `src` da imagem -->
    <img v-bind:src="imagemURL" alt="Imagem dinâmica">
    <!-- Ou simplesmente :src="imagemURL" -->
  </div>
</template>

<script>
export default {
  data() {
    return {
      imagemURL: 'https://example.com/imagem.jpg'
    };
  }
};
</script>


=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=

2. v-model
Cria uma ligação bidirecional entre a entrada de um formulário e os dados.

vue
Copiar código
<template>
  <div>
    <input v-model="nome" placeholder="Digite seu nome">
    <p>Seu nome é: {{ nome }}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      nome: ''
    };
  }
};
</script>


=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=


3. v-if e v-else
Renderiza ou remove elementos do DOM com base em condições.

vue
Copiar código
<template>
  <div>
    <p v-if="mostrar">Este parágrafo aparece se 'mostrar' for true</p>
    <p v-else>Este parágrafo aparece se 'mostrar' for false</p>
    <button @click="toggleMostrar">Alternar Mostrar</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      mostrar: true
    };
  },
  methods: {
    toggleMostrar() {
      this.mostrar = !this.mostrar;
    }
  }
};
</script>

=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=


4. v-for
Itera sobre arrays e objetos.

vue
Copiar código
<template>
  <div>
    <ul>
      <li v-for="(item, index) in lista" :key="index">
        {{ item }}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      lista: ['Item 1', 'Item 2', 'Item 3']
    };
  }
};
</script>


=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=


5. v-on (ou @)
Associa eventos do DOM a métodos do Vue.

vue
Copiar código
<template>
  <div>
    <button v-on:click="dizerOla">Clique para dizer Olá</button>
    <!-- Ou simplesmente @click="dizerOla" -->
  </div>
</template>

<script>
export default {
  methods: {
    dizerOla() {
      alert('Olá!');
    }
  }
};
</script>


=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=


6. v-show
Mostra ou esconde um elemento, mas o mantém no DOM.

vue
Copiar código
<template>
  <div>
    <p v-show="mostrarTexto">Este texto está visível quando 'mostrarTexto' é true</p>
    <button @click="toggleMostrar">Alternar Visibilidade</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      mostrarTexto: true
    };
  },
  methods: {
    toggleMostrar() {
      this.mostrarTexto = !this.mostrarTexto;
    }
  }
};
</script>


=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=


7. v-pre
Impede a renderização do Vue dentro de um bloco específico.

vue
Copiar código
<template>
  <div>
    <p v-pre>{{ istoNaoSeraProcessado }}</p>
    <p>{{ istoSeraProcessado }}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      istoNaoSeraProcessado: 'Texto que não será processado pelo Vue',
      istoSeraProcessado: 'Texto que será processado pelo Vue'
    };
  }
};
</script>


=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=


8. v-cloak
Garante que os elementos só sejam exibidos quando o Vue tiver sido completamente carregado.

vue
Copiar código
<template>
  <div v-cloak>
    {{ mensagem }}
  </div>
</template>

<script>
export default {
  data() {
    return {
      mensagem: 'Carregado!'
    };
  }
};
</script>

<style>
[v-cloak] {
  display: none;
}
</style>


=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=


9. v-once
Renderiza o conteúdo apenas uma vez e nunca mais o re-renderiza.

vue
Copiar código
<template>
  <div>
    <p v-once>{{ mensagem }}</p>
    <button @click="atualizarMensagem">Atualizar Mensagem</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      mensagem: 'Este texto nunca será atualizado após a renderização inicial'
    };
  },
  methods: {
    atualizarMensagem() {
      this.mensagem = 'Nova mensagem, mas o Vue não atualizará isso';
    }
  }
};
</script>


=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=


Esses exemplos mostram como você pode utilizar as diretivas v- no Vue.js para manipular dinamicamente o DOM de acordo com o estado reativo dos dados do componente.
