# Intro.js PT-BR

Este é um fork do projeto [Intro.js](https://introjs.com/) que foi personalizado e traduzido para português brasileiro. O Intro.js PT-BR é uma biblioteca JavaScript leve e fácil de usar para criar guias interativos e dicas passo a passo para suas páginas web.

## Instalação

Adicione os seguintes links no cabeçalho do seu HTML:

```html
<link
  rel="stylesheet"
  href="https://cdn.jsdelivr.net/gh/ReisLucasF/intro/intro.css"
/>
<script src="https://cdn.jsdelivr.net/gh/ReisLucasF/intro/intro.js"></script>
```

## Uso Básico

```javascript
// Iniciar o guia passo a passo
introJs().start();
```

## Exemplos de Uso

### Exemplo Básico

```html
<div
  class="elemento"
  data-intro="Esta é uma dica explicativa sobre este elemento."
  data-step="1"
>
  Conteúdo do elemento
</div>

<button
  class="botao"
  data-intro="Este botão realiza uma ação importante."
  data-step="2"
>
  Clique Aqui
</button>

<script>
  // Iniciar o tour quando a página carregar
  document.addEventListener("DOMContentLoaded", function () {
    introJs().start();
  });
</script>
```

### Configurações Personalizadas

```javascript
introJs()
  .setOptions({
    nextLabel: "Próximo",
    prevLabel: "Anterior",
    skipLabel: "Pular",
    doneLabel: "Concluir",
    hidePrev: true,
    hideNext: false,
    tooltipPosition: "bottom",
    tooltipClass: "minha-classe-personalizada",
    highlightClass: "minha-classe-destaque",
    exitOnOverlayClick: false,
    showStepNumbers: true,
    keyboardNavigation: true,
    showButtons: true,
    showBullets: true,
    showProgress: false,
    scrollToElement: true,
    overlayOpacity: 0.8,
    disableInteraction: false,
  })
  .start();
```

## Características

- ✅ Design responsivo
- ✅ Totalmente traduzido para português brasileiro
- ✅ Compatível com dispositivos móveis e desktop
- ✅ Sem dependências externas
- ✅ Personalizável via CSS
- ✅ Controle de teclado (setas esquerda/direita para navegação)
- ✅ API fácil de usar

## Métodos Disponíveis

| Método                     | Descrição                                |
| -------------------------- | ---------------------------------------- |
| `start()`                  | Inicia o tour                            |
| `goToStep(step)`           | Vai para um passo específico             |
| `addStep(options)`         | Adiciona um novo passo programaticamente |
| `nextStep()`               | Avança para o próximo passo              |
| `previousStep()`           | Retorna ao passo anterior                |
| `exit()`                   | Encerra o tour                           |
| `setOption(option, value)` | Define uma opção específica              |
| `setOptions(options)`      | Define múltiplas opções                  |
| `refresh()`                | Atualiza a posição das dicas             |

## Contribuindo

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou enviar pull requests.

## Licença

Este projeto é licenciado sob os mesmos termos do projeto original Intro.js.

## Agradecimentos

- [Intro.js](https://introjs.com/) - Projeto original
- [Afshin Mehrabani](https://github.com/afshinm) - Criador do Intro.js

---

Para documentação completa e mais exemplos, visite [a documentação oficial do Intro.js](https://introjs.com/docs/) (em inglês).
