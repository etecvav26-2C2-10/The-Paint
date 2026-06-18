# DEVLOG #03
## Arquitetura de Navegação — The Paint v1.0

---

### 1. O que foi desenvolvido nesta etapa

Com a identidade visual definida, Pedro Menezes conduziu o mapeamento da **arquitetura de informação e navegação** do portal. Esta etapa define quais páginas existem, o que cada uma contém, como o usuário transita entre elas e como o repositório está organizado no GitHub.

---

### 2. Mapa de Páginas

```
The Paint v2.0
├── index.html       — Home (vitrine e conteúdo principal)
├── sobre.html       — Sobre o projeto e equipe
├── nba.html         — Conteúdo dedicado à NBA
├── fiba.html        — Conteúdo dedicado à FIBA
├── shop.html        — Loja de cosméticos temáticos
├── contato.html     — Formulário e informações
├── style.css        — Estilos globais (Mobile First)
├── translations.js  — Sistema de 10 idiomas
└── README.md        — Documentação do projeto
```

---

### 3. Função de Cada Página

| Página | Objetivo Principal |
|---|---|
| `index.html` | Apresentar o portal, destaques, notícias e comparativos |
| `sobre.html` | Comunicar história, missão e equipe do projeto |
| `nba.html` | Conteúdo aprofundado sobre a liga norte-americana |
| `fiba.html` | Conteúdo sobre o basquete internacional e FIBA |
| `shop.html` | Loja com 10 produtos cosméticos temáticos |
| `contato.html` | Formulário de contato e mapa de localização |

---

### 4. Estrutura de Pastas no Repositório

```
the-paint/
├── index.html
├── sobre.html
├── nba.html
├── fiba.html
├── shop.html
├── contato.html
├── style.css
├── translations.js
├── README.md
├── planejamento/    — 14 arquivos markdown de documentação
├── imagens/         — Assets visuais do portal
├── logo/            — Rascunhos e versão final da marca
└── referencias/     — Referências visuais e de conteúdo
```

---

### 5. Fluxo de Navegação do Usuário

1. Usuário acessa a **Home** (`index.html`) — vitrine principal.
2. Pode navegar via menu para **NBA**, **FIBA**, **Sobre** ou **Contato**.
3. Ao clicar em **Loja** (Shop), visualiza produtos sem precisar de login.
4. Ao tentar comprar, é redirecionado ao **modal de login**.
5. Após autenticação, pode finalizar a compra.

---

### 6. Padrões do Repositório

- **Mensagens de commit semânticas:** prefixos `docs:`, `feat:`, `fix:`, `chore:`, `style:`.
- **Pastas organizadas** desde o início: planejamento, imagens, logo, referencias.
- **README** atualizado a cada grande entrega como documento vivo do projeto.

---

### 7. Commits desta Etapa

| Integrante | Commit | Mensagem |
|---|---|---|
| Pedro | #01 | `chore: inicializar estrutura de pastas do projeto no git` |
| Pedro | #06 | `docs: mapear a arquitetura da informacao e navegacao do site` |
| Pedro | #08 | `docs: criar os arquivos markdown base para cada pagina futura` |
| Pedro | #09 | `docs: revisar consistencia tecnica e finalizar README para entrega` |

---

### 8. Próximos Passos

Com a arquitetura mapeada, a equipe avança para o **planejamento detalhado do conteúdo** de cada página — o que o usuário vai ler, ver e interagir em cada seção. Tema do DEVLOG #04.

---

*The Paint — Basquete Total © 2026 | DEVLOG #03 — Arquitetura de Navegação*
