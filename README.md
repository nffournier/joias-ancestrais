# Joias Ancestrais

Landing page da **Joias Ancestrais**, marca de joias e acessórios artesanais inspirados na ancestralidade afro-brasileira, na natureza, na memória e na identidade.

Fiz este projeto para um desafio acadêmico: criar uma landing page de verdade, acessível, responsiva e publicada no GitHub Pages, usando só HTML5, CSS3, Git e GitHub. Sem JavaScript, sem atalhos.

## Sobre o projeto

A página apresenta o conceito da marca, as três coleções (Águas de Oxum, Caminhos de Ogum e Matas de Oxóssi), o processo criativo, o impacto cultural, uma galeria de peças e os canais de contato.

Queria que o visual transmitisse ancestralidade, artesanato e sofisticação sem parecer um template genérico de e-commerce. Por isso apostei em tipografia editorial, fotos grandes, bastante respiro e tons naturais.

## Tecnologias

- HTML5 semântico
- CSS3 (variáveis, Flexbox e Grid)
- Git e GitHub
- GitHub Pages

**Sem JavaScript.** A página funciona 100% sem scripts.

## Estrutura

```text
joias-ancestrais/
├── index.html
├── assets/
│   ├── css/style.css
│   ├── images/   (hero, colecoes, galeria)
│   └── icons/
├── README.md
└── .gitignore
```

## O que a página tem

- Menu fixo com navegação por âncoras
- Hero com a chamada "Cada joia conta uma história."
- Sobre: a história da marca
- Coleções: três cards com imagem, título e descrição
- Processo criativo: timeline em HTML/CSS puro (Pesquisa, Criação, Produção, Finalização)
- Impacto: cinco pilares do projeto, sem números inventados
- Galeria: grid responsivo com formatos variados
- Contato e rodapé

## Imagens

Usei fotografias gratuitas do [Unsplash](https://unsplash.com), baixadas para `assets/images/` e recortadas nos formatos do layout (hero 4:5, cards 4:3 e galeria em proporções variadas). São de autores do Unsplash, sob a [Unsplash License](https://unsplash.com/license): uso gratuito, inclusive comercial, sem exigir atribuição.

Os textos `alt` descrevem cada foto. Para trocar por imagens da marca, basta substituir os arquivos nas pastas `hero/`, `colecoes/` e `galeria/`, atualizar os `src` no `index.html` e revisar os `alt`.

## Acessibilidade

Cuidei para que a página fosse usável por todo mundo:

- HTML semântico (`header`, `nav`, `main`, `section`, `article`, `figure`, `ol`, `footer`), com `div` só quando não havia opção melhor
- Um único `h1` e hierarquia de títulos coerente
- Foco visível em links e botões (`:focus-visible`) e navegação por teclado
- Link "Pular para o conteúdo" no início da página
- `alt` descritivo em todas as imagens
- Contraste adequado em todas as seções, inclusive na seção Impacto (fundo escuro)
- `prefers-reduced-motion` para quem prefere menos movimento

## Responsividade

Fiz mobile-first: o CSS base serve telas pequenas e as media queries (`min-width`) ampliam o layout conforme o espaço.

- **Celular:** uma coluna, menu em linha com rolagem horizontal, galeria em 2 colunas
- **Tablet (640px e 768px):** cards e impacto em 2 colunas
- **Desktop (1024px):** hero em 2 colunas, 3 cards, timeline horizontal, galeria em 4 colunas e impacto em 5

Uso `clamp()`, `min()`, `max()`, `grid` e `flex` para evitar medidas fixas. Não há rolagem horizontal.

## Tipografia

- **Fraunces** nos títulos, serifada e com personalidade
- **Work Sans** nos textos, limpa e legível

Carrego as duas pelo Google Fonts com `preconnect` e `display=swap`, com fallback para Georgia e system-ui.

## Publicação

Site: https://nffournier.github.io/joias-ancestrais/
Repositório: https://github.com/nffournier/joias-ancestrais

Publiquei pelo GitHub Pages (branch `main`, pasta raiz). Para publicar um projeto novo, o caminho é o mesmo que segui: criar o repositório, enviar os arquivos com `git push` e ativar o Pages em **Settings → Pages**.

## Uso da IA

Usei o opencode como apoio, não como substituto do entendimento. Ele me ajudou a escrever a primeira versão do HTML e do CSS, a montar o design system e a estratégia de responsividade, e a revisar textos, semântica e acessibilidade.

O conceito da marca, as coleções e a direção de arte são meus, assim como a revisão de todo o código. Também fiz a validação manual (navegação, contraste, responsividade, troca das imagens) e a publicação no GitHub.

Alguns prompts que usei:

- "Crie uma landing page acessível e responsiva em HTML/CSS puro para uma marca de joias artesanais inspirada na ancestralidade afro-brasileira."
- "Como montar uma timeline horizontal e vertical usando apenas HTML e CSS?"
- "Revise a acessibilidade desta página: hierarquia de títulos, alt das imagens e foco visível."

Parte do código foi gerada pela IA e revisada por mim. Consigo explicar cada decisão na apresentação, e nada aqui depende de truques ou bibliotecas escondidas.
