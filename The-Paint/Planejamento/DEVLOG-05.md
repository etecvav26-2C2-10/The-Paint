# DEVLOG #05
## Mobile First e Recursos Interativos — The Paint v1.0

---

### 1. O que foi desenvolvido nesta etapa

Com o conteúdo mapeado, a equipe estabeleceu a **estratégia técnica de implementação**: como o site será construído para funcionar bem em qualquer dispositivo e quais recursos interativos serão entregues na versão 1.0. Esta etapa é conduzida por **Pedro Menezes**.

---

### 2. O Conceito Mobile First

O The Paint adota a abordagem **Mobile First**: toda a estrutura visual e a disposição dos elementos foram pensadas primeiramente para telas de celular e adaptadas para desktop via media queries.

**Por quê Mobile First?**
O público-alvo — jovens de 14 a 30 anos — acessa conteúdo esportivo e realiza compras prioritariamente pelo smartphone. Projetar o mobile como ponto de partida garante que a experiência principal seja otimizada para o dispositivo mais usado pelo nosso usuário.

---

### 3. Implementação Técnica

| Técnica | Descrição |
|---|---|
| Layout em coluna única | Estrutura padrão no mobile, sem quebras de conteúdo |
| Menu hambúrguer | Acionado por JavaScript, compacto no topo da tela |
| Grid responsivo | `auto-fit` + `minmax` para colunas automáticas |
| Imagens fluidas | `max-width: 100%` em todos os elementos de mídia |
| Tabelas com scroll | `overflow-x: auto` evita quebras em tabelas comparativas |
| Font-size mínimo | 16px em todo o corpo de texto |
| Área de toque | Botões com mínimo de 44px de altura (acessibilidade) |
| Media query principal | `@media (max-width: 768px)` |

---

### 4. Expansão para Desktop

No desktop, o layout se expande naturalmente sem reescrever CSS:

- Menu horizontal visível (hambúrguer oculto)
- Grid multi-colunas para cards e seções
- Layout em duas colunas na página de Contato

---

### 5. Recursos Interativos — v1.0

| Recurso | Tecnologia | Descrição |
|---|---|---|
| Menu hambúrguer | JavaScript | Toggle de classe CSS, animação suave |
| FAQ expansível | JavaScript + CSS | Accordion com transição de altura |
| Formulário de contato | HTML5 | Validação nativa + feedback de sucesso |
| Embed de mapa | HTML (iframe) | Google Maps responsivo |

---

### 6. Recursos Planejados para v2.0 e Além

- Sistema de login e cadastro via modal
- Filtros de categoria na loja (JavaScript)
- Toast notification ao adicionar ao carrinho
- Sistema de troca de idioma em tempo real
- Busca interna no portal
- Carrinho de compras completo
- Integração com API de notícias esportivas

---

### 7. Diretrizes de Desempenho Mobile

- Imagens comprimidas antes do upload
- Fontes carregadas via sistema (Segoe UI / Arial), sem dependência de CDN
- CSS com variáveis nativas (sem pré-processadores)
- JavaScript mínimo e sem frameworks externos

---

### 8. Commits desta Etapa

| Integrante | Commit | Mensagem |
|---|---|---|
| Pedro | #03 | `docs: redigir a justificativa tecnica da escolha do Mobile First` |
| Pedro | #04 | `docs: documentar a estrategia de adaptacao do menu responsivo` |
| Pedro | #05 | `docs: definir cuidados com imagens e textos no ambiente mobile` |
| Misael | #07 | `docs: documentar ideias para os recursos interativos do site` |

---

### 9. Próximos Passos

Com a estratégia Mobile First estabelecida, o projeto avança para o planejamento dos **formulários e mapas** da página de contato. Tema do DEVLOG #06.

---

*The Paint — Basquete Total © 2026 | DEVLOG #05 — Mobile First e Recursos Interativos*
