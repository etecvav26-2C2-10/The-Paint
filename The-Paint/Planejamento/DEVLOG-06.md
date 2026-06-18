# DEVLOG #06
## Formulários e Mapas — The Paint v1.0

---

### 1. O que foi desenvolvido nesta etapa

Esta etapa detalha a implementação técnica dos **formulários de contato** e do **mapa embed** presentes na página `contato.html`, além do **modal de login e cadastro** que será acessível a partir de qualquer página do portal.

---

### 2. Formulário de Contato

O formulário da página `contato.html` foi projetado com foco em simplicidade e validação nativa:

| Configuração | Detalhe |
|---|---|
| Campos | Nome, E-mail, Assunto, Mensagem |
| Validação | HTML5 nativo: `required` e `type="email"` |
| Feedback | Mensagem de sucesso exibida após envio |
| Layout | `flex-column` — empilhamento responsivo no mobile |
| Estilização | Inputs com borda laranja em foco (`#f97316`) |

**Decisão técnica:** A validação via atributos HTML5 elimina a necessidade de JavaScript extra para o caso de uso básico, mantendo o código limpo e o carregamento rápido.

---

### 3. Embed de Mapa

| Configuração | Valor |
|---|---|
| Tecnologia | Google Maps via `<iframe>` |
| Largura | `width: 100%` para responsividade total |
| Visual | `border-radius: 12px` para estética moderna |
| Localização | São Paulo, SP (Rua do Basquete, 1891 — fictício) |
| Altura mobile | `height: 300px` |
| Altura desktop | `height: 450px` via media query |

---

### 4. Modal de Login e Cadastro

O modal de autenticação é um componente reutilizável acessível do header de qualquer página:

| Característica | Detalhe |
|---|---|
| Acionamento | Botão "Entrar" no header (todas as páginas) |
| Fechamento | Clique no × ou fora do modal |
| Estrutura interna | Duas abas: Login e Cadastro |
| Login social | Botões Google e Apple |
| Validação | HTML5 nativo (`required`, `type="email"`) |

**Aba de Login:** E-mail + Senha + opções sociais.

**Aba de Cadastro:** Nome completo + E-mail + Senha + opções sociais.

---

### 5. Fluxo Técnico do Modal

```
1. Usuário clica em "Entrar" no header
2. JavaScript adiciona classe 'active' ao modal
3. Modal aparece com animação CSS (opacity + transform)
4. Usuário seleciona aba Login ou Cadastro
5. Preenche campos e submete
6. Clique no × ou fora remove a classe 'active'
```

---

### 6. Layout de Duas Colunas no Desktop

Na página de Contato, o desktop exibe formulário e mapa lado a lado:

```
[ Formulário (50%) ] [ Mapa (50%) ]
```

No mobile, empilha verticalmente:

```
[ Formulário (100%) ]
[ Mapa (100%) ]
```

---

### 7. Commits desta Etapa

| Integrante | Commit | Mensagem |
|---|---|---|
| Pedro | #07 | `docs: detalhar o funcionamento tecnico dos formularios e mapas` |

---

### 8. Próximos Passos

Com toda a base técnica da v1.0 documentada, o projeto avança para o grande salto da **v2.0**: o sistema de login integrado à loja. Tema do DEVLOG #07.

---

*The Paint — Basquete Total © 2026 | DEVLOG #06 — Formulários e Mapas*
