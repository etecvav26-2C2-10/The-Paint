# DEVLOG #07
## Sistema de Login e Cadastro — The Paint v2.0

---

### 1. O que foi desenvolvido nesta etapa

A versão 2.0 do The Paint introduz três grandes pilares que elevam o portal de um site informativo para uma **plataforma completa**. O primeiro é o **sistema de login e cadastro de usuários**, implementado como modal interativo acessível a partir de qualquer página.

---

### 2. Objetivo do Sistema

Permitir que usuários criem conta e façam login para acessar funcionalidades exclusivas — em especial a **finalização de compras na loja de cosméticos**. O sistema também estrutura a base para funcionalidades futuras como histórico de pedidos e wishlist.

---

### 3. Funcionamento do Modal

| Característica | Detalhes |
|---|---|
| Acionamento | Botão "Entrar" fixo no header de todas as páginas |
| Fechamento | Clique no botão × ou clique fora do modal |
| Estrutura interna | Duas abas: Login e Cadastro |
| Login social | Botões para autenticação via Google e Apple |
| Validação | Atributos HTML5 nativos (`required`, `type="email"`) |

---

### 4. Campos por Aba

#### Aba Login
- E-mail
- Senha
- Botão: "Entrar com Google"
- Botão: "Entrar com Apple"

#### Aba Cadastro
- Nome completo
- E-mail
- Senha
- Botão: "Cadastrar com Google"
- Botão: "Cadastrar com Apple"

---

### 5. Integração com a Loja

| Situação do Usuário | Comportamento do Sistema |
|---|---|
| Não logado | Pode navegar e visualizar todos os produtos |
| Tentativa de compra | Exibe botão "Entrar / Cadastrar" com CTA na loja |
| Logado | Pode adicionar ao carrinho e finalizar compra |

Esta abordagem reduz o atrito inicial (sem forçar login para navegar) e converte o usuário no momento mais relevante: quando ele demonstra intenção de compra.

---

### 6. Implementação Técnica

Toda a lógica foi implementada com **JavaScript puro**, sem frameworks externos:

- Estado das abas controlado por classes CSS toggled via JS
- Modal aparece com animação de opacidade e `transform`
- Evento de clique fora do modal capturado no overlay
- Nenhuma dependência externa — zero impacto no carregamento

---

### 7. Expansão Futura

| Funcionalidade | Status |
|---|---|
| Autenticação real com backend | Planejado para v3.0 |
| Área do usuário com histórico de pedidos | Planejado para v3.0 |
| Wishlist de produtos favoritos | Planejado para v3.0 |
| Sessão persistente entre visitas | Planejado para v3.0 |

---

### 8. Commits desta Etapa

| Integrante | Commit | Mensagem |
|---|---|---|
| Pedro | #feat | `feat: implementar modal de login e cadastro com abas` |
| Pedro | #feat | `feat: adicionar login social Google e Apple no modal` |
| João Paulo | #style | `style: estilizar modal com paleta e tipografia do projeto` |

---

### 9. Próximos Passos

Com o sistema de autenticação em funcionamento, o próximo passo é apresentar o destino principal do usuário logado: a **loja de cosméticos temáticos NBA**. Tema do DEVLOG #08.

---

*The Paint — Basquete Total © 2026 | DEVLOG #07 — Sistema de Login e Cadastro*
