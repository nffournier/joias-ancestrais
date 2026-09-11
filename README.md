# Joias Ancestrais

Landing page da **Joias Ancestrais** — marca de joias e acessórios artesanais inspirados na ancestralidade afro-brasileira, na natureza, na memória e na identidade.

O projeto foi desenvolvido como parte de um desafio acadêmico: criar uma landing page real, acessível, responsiva e publicada com **GitHub Pages**, usando apenas HTML5, CSS3, Git e GitHub.

## Descrição

A página apresenta o conceito da marca e suas três coleções (Águas de Oxum, Caminhos de Ogum e Matas de Oxóssi), o processo criativo, o impacto cultural do projeto, uma galeria de peças e canais de contato.

O objetivo visual é transmitir **ancestralidade, artesanato, identidade, sofisticação e contemporaneidade** — com tipografia editorial, fotos grandes, bastante respiro e tons naturais. O resultado não é um template genérico de e-commerce, e sim uma marca cultural contemporânea.

## Tecnologias

- HTML5 (estrutura semântica)
- CSS3 (design system com variáveis, layout em Flexbox/Grid)
- Git (controle de versão)
- GitHub Pages (publicação)

**Sem JavaScript.** A página funciona 100% sem scripts.

## Estrutura de arquivos

```text
joias-ancestrais/
│
├── index.html
│
├── assets/
│   ├── css/
│   │   └── style.css
│   │
│   ├── images/
│   │   ├── hero/       ← foto do hero
│   │   ├── colecoes/   ← fotos das coleções
│   │   └── galeria/    ← fotos da galeria
│   │
│   └── icons/
│
├── README.md
│
└── .gitignore
```

## Funcionalidades

- **Navegação por âncoras** — menu fixo que leva a cada seção da página
- **Hero** — mensagem central "Cada joia conta uma história." com chamada para a coleção
- **Sobre** — narrativa do conceito da marca
- **Coleções** — três cards semânticos com imagem, título e descrição
- **Processo criativo** — timeline em HTML/CSS puro (Pesquisa, Criação, Produção, Finalização)
- **Impacto** — cinco pilares do projeto (artesanato, identidade, saberes, renda, protagonismo), sem dados numéricos inventados
- **Galeria** — grid responsivo com formatos variados (imagem grande/pequena)
- **Contato** — Instagram, WhatsApp e e-mail
- **Rodapé** — marca, descrição, navegação e copyright

## Imagens

As imagens são **fotografias reais** de bancos gratuitos ([Unsplash](https://unsplash.com)), baixadas localmente para `assets/images/` e recortadas nos formatos usados pelo layout (hero 4:5, cards 4:3 e galeria em proporções variadas).

- **Hero** — retrato de mulher negra com trajes e joias tradicionais africanas, reforçando ancestralidade e identidade;
- **Coleções** — uma foto por coleção: pingente de pedra azul (Oxum), pulseira artesanal com pedra sobre madeira (Ogum) e pingente de pedra natural em madeira (Oxóssi);
- **Galeria** — pulseiras e colares de contas e pedras naturais, feitos à mão, em diferentes enquadramentos.

**Créditos e licença:** as fotos são de autores do Unsplash e seguem a [Unsplash License](https://unsplash.com/license) (uso gratuito, inclusive comercial, sem necessidade de atribuição). Os textos `alt` descrevem o conteúdo de cada foto.

Para substituir por fotos próprias da marca: coloque os arquivos em `assets/images/hero/`, `assets/images/colecoes/` e `assets/images/galeria/`, atualize os `src` no `index.html` e revise os `alt`.

## Acessibilidade

Decisões tomadas:

- **HTML semântico** — `header`, `nav`, `main`, `section`, `article`, `figure`, `ol`, `footer`; `div` só quando não há elemento semântico melhor;
- **Um único `h1`** — hierarquia de títulos lógica (h1 → h2 → h3), tamanho controlado pelo CSS;
- **Navegação por teclado** — todos os links e botões são focáveis, com **foco visível** (`:focus-visible`) em toda a página;
- **Skip link** — link "Pular para o conteúdo" no início da página;
- **`alt` descritivos** em todas as imagens — nunca "imagem" ou "foto";
- **Contraste adequado** entre texto e fundo em todas as seções (inclusive na seção Impacto, em fundo escuro);
- **Landmarks claras** — `header`, `main`, `footer` e `nav` com `aria-label` apenas onde necessário;
- **`prefers-reduced-motion`** — animações e rolagem suave são desativadas para quem prefere menos movimento;
- **Áreas clicáveis adequadas** — botões e links com área de toque confortável.

## Responsividade

Abordagem **mobile-first**: o CSS base é escrito para telas pequenas e `media queries` (`min-width`) vão ampliando o layout conforme o espaço disponível.

- **Celular:** colunas únicas, menu empilhado, galeria em 2 colunas;
- **Tablet (640px e 768px):** cards e grade do impacto em 2 colunas;
- **Desktop (1024px):** hero em 2 colunas, 3 cards de coleção, timeline horizontal, galeria em 4 colunas, impacto em 5 colunas.

O layout usa `clamp()`, `min()`, `max()`, `grid` e `flex` para evitar valores fixos que quebram em telas pequenas — **nunca há rolagem horizontal**.

## Tipografia

- **Fraunces** (Google Fonts) — títulos: serifada com personalidade, transmite editorial e artesanal;
- **Work Sans** (Google Fonts) — textos: limpa, moderna e legível.

Fontes carregadas via Google Fonts com `preconnect` e `display=swap`, e com *fallback* para fontes do sistema (Georgia / system-ui). Documentação: decisão de usar duas famílias apenas, para equilíbrio entre identidade visual e performance.

## Publicação (GitHub Pages)

Para publicar:

1. Crie um repositório no GitHub com o nome desejado;
2. Envie este projeto para o repositório:
   ```bash
   git remote add origin https://github.com/SEU-USUARIO/joias-ancestrais.git
   git push -u origin main
   ```
3. No GitHub: **Settings → Pages → Source: Deploy from a branch → Branch: main / root**.

```text
Site:
[LINK]

Repositório:
[LINK]
```

## Uso da IA

Este projeto foi desenvolvido com o apoio de uma IA (opencode). A IA foi usada como **ferramenta de apoio**, e não como substituta da compreensão do código.

### O que a IA fez

- Gerou a primeira versão da estrutura HTML e do CSS a partir das especificações do desafio;
- Ajudou a definir o design system (variáveis de cor, tipografia, espaçamento) e a estratégia de responsividade mobile-first;
- Auxiliou na redação dos textos e na auditoria final (semântica, acessibilidade, links).

### O que é do estudante

- As decisões de conceito e identidade visual da marca (tema, coleções, direção de arte);
- A revisão e a compreensão de **todo** o código antes da apresentação;
- A validação manual do resultado (navegação, contraste, responsividade, troca de placeholders por fotos reais);
- A publicação e o gerenciamento no GitHub.

### Exemplos de prompts utilizados

- "Crie uma landing page acessível e responsiva em HTML/CSS puro para uma marca de joias artesanais inspirada na ancestralidade afro-brasileira."
- "Como montar uma timeline horizontal e vertical usando apenas HTML e CSS?"
- "Revise a acessibilidade desta página: hierarquia de títulos, alt das imagens e foco visível."

### Nota honesta

Partes do código (estrutura HTML, organização do CSS) foram geradas pela IA e **revisadas manualmente** pelo estudante, que deve ser capaz de explicar cada decisão durante a apresentação. Nenhuma funcionalidade foi "escondida" na forma de truques ou bibliotecas.