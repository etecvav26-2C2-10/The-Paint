# DEVLOG #08
## Loja de Cosméticos — The Paint Shop v2.0

---

### 1. O que foi desenvolvido nesta etapa

O segundo grande pilar da v2.0 é a **The Paint Shop**: uma loja de cosméticos temáticos NBA integrada diretamente ao portal. A proposta une dois universos aparentemente distantes — beleza e basquete — em uma experiência de marca coesa e inovadora.

---

### 2. Conceito da Loja

Cada produto carrega nomes e referências diretas ao esporte, criando uma identidade de marca única e memorável para o público-alvo: jovens fãs de basquete que também consomem moda e beleza.

**Identidade visual da loja:**
- Cor predominante: **Roxo** (`#7b2d8b`) no hero
- Atmosfera: esportiva, moderna e premium
- Avaliação geral: ⭐ 4,9

---

### 3. Catálogo Completo — v1.0

| Produto | Categoria | Preço |
|---|---|---|
| Batom NBA Red — Lakers | Maquiagem | R$ 49,90 |
| Paleta Court Vision | Maquiagem | R$ 89,90 |
| Esmalte Three-Pointer | Maquiagem | R$ 39,90 |
| Sérum Game Face SPF 50 | Skincare | R$ 129,90 |
| Hidratante Skin in the Paint | Skincare | R$ 74,90 |
| Máscara Facial Slam Dunk | Skincare | R$ 44,90 |
| Loção Corporal Fast Break | Corpo | R$ 59,90 |
| Kit Banho All-Star | Corpo | R$ 139,90 |
| Nécessaire The Paint | Acessórios | R$ 89,90 |
| Kit Escovas Bench Warmer | Acessórios | R$ 119,90 |

---

### 4. Categorias da Loja

| Categoria | Produtos | Descrição |
|---|---|---|
| Maquiagem | 3 | Batons, paletas de sombra, esmaltes |
| Skincare | 3 | Séruns, hidratantes, máscaras faciais |
| Corpo | 2 | Loções corporais, kits de banho |
| Acessórios | 2 | Nécessaires, pincéis profissionais |

---

### 5. Funcionalidades da Loja

| Funcionalidade | Descrição |
|---|---|
| Filtros por categoria | Botões que filtram produtos em tempo real (JavaScript puro) |
| Toast notification | Confirmação visual ao adicionar produto ao carrinho |
| Frete grátis | Ativado automaticamente para compras acima de R$ 150 |
| Avaliação geral | 4,9 estrelas exibida na vitrine para gerar confiança |
| Integração com login | Finalização de compra exige autenticação (DEVLOG #07) |

---

### 6. Estrutura da Página (`shop.html`)

1. **Hero da loja** — Título, chamada para ação e paleta roxa temática
2. **Barra de filtros** — Todos | Maquiagem | Skincare | Corpo | Acessórios
3. **Grid de produtos** — Cards com nome, categoria, avaliação e preço
4. **Botão de compra** — "Adicionar ao carrinho" em cada card
5. **Banner de frete grátis** — Comunicação do benefício acima de R$ 150

---

### 7. Lógica dos Filtros (JavaScript)

```javascript
// Ao clicar em um filtro:
// 1. Remove classe 'active' de todos os botões
// 2. Adiciona 'active' ao botão clicado
// 3. Oculta todos os cards de produto
// 4. Exibe apenas cards da categoria selecionada
// (sem recarregar a página)
```

---

### 8. Commits desta Etapa

| Integrante | Commit | Mensagem |
|---|---|---|
| João Paulo | #feat | `feat: criar pagina shop com hero e grid de produtos` |
| João Paulo | #feat | `feat: estilizar cards de produto com paleta roxa da loja` |
| Pedro | #feat | `feat: implementar filtros de categoria na loja` |
| Pedro | #feat | `feat: adicionar toast notification ao carrinho` |
| Misael | #docs | `docs: planejar catalogo de 10 produtos cosmeticos tematicos` |

---

### 9. Próximos Passos

Com a loja integrada ao sistema de login, o terceiro pilar da v2.0 é o **sistema de 10 idiomas** que tornará o portal verdadeiramente global. Tema do DEVLOG #09.

---

*The Paint — Basquete Total © 2026 | DEVLOG #08 — Loja de Cosméticos*
