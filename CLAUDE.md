# CLAUDE.md — giacomoponte.com.br

Este arquivo define as diretrizes de design e desenvolvimento para o site pessoal de Giácomo Ponte, personal trainer independente baseado em Fortaleza, CE.

---

## Identidade Visual

### Paleta de Cores
```css
--color-bg:        #07101a;   /* fundo principal */
--color-surface:   #0b1828;   /* cards, seções */
--color-surface-2: #0f2035;   /* elementos elevados */
--color-accent:    #4A7FA5;   /* destaque, CTAs, links */
--color-text:      #e8edf2;   /* texto principal */
--color-text-muted:#8aa3b8;   /* texto secundário */
```

### Tipografia
- **Display / Títulos**: Raleway (Google Fonts) — weights 700, 800
- **Corpo / UI**: Barlow (Google Fonts) — weights 400, 500, 600
- Evitar: Inter, Roboto, Arial, system-ui

### Tom Geral
- Refinado, confiante, atlético — não genérico
- Dark theme com detalhes em azul aço
- Espaçamento generoso, hierarquia clara

---

## Diretrizes de Design

### Layout
- Mobile-first sempre
- `max-width: 360px` para seções de formulário e conteúdo centralizado
- Containers de conteúdo: `max-width: 900px` centrado
- Padding padrão de seção: `padding: 48px 24px`

### Componentes
- Botões primários: background `--color-accent`, `height: 48px`, `border-radius: 8px`, largura 100% em mobile
- Cards: background `--color-surface`, `border-radius: 12px`, `padding: 24px`
- Bordas sutis: `border: 1px solid rgba(74, 127, 165, 0.15)`

### Animações
- Preferir CSS puro (transitions, keyframes)
- Entradas: fade + translateY sutil (não exagerado)
- Hover em botões: leve brighten no accent + scale 1.02
- Evitar animações pesadas que prejudiquem performance mobile

### Imagens e Mídia
- Logo: giacomoponte.com.br/logo (verificar path real no projeto)
- Fotos sempre com `object-fit: cover` e aspect-ratio fixo

---

## Stack & Convenções de Código

- HTML5 semântico, CSS puro ou com variáveis CSS
- JavaScript vanilla (sem frameworks pesados salvo necessidade)
- Sem dependências desnecessárias
- Comentários em português
- Nomes de classes em kebab-case descritivo (ex: `.hero-section`, `.cta-button`)

---

## Conteúdo & Voz

- Idioma: Português brasileiro
- Tom: direto, confiante, acolhedor — sem jargão excessivo
- Público: pessoas buscando personal trainer presencial ou online em Fortaleza
- Evitar: excesso de exclamações, clichês fitness ("transforme sua vida!"), linguagem corporativa fria

---

## Páginas e Seções Previstas

- Hero (apresentação + CTA de contato)
- Sobre (história, valores, certificações)
- Planos (Start, Evolução, Performance, Transformação, Elite + Duo)
- Depoimentos
- Contato (WhatsApp + Instagram)

---

## Instruções para o Claude Code

Ao trabalhar neste projeto:
1. Sempre manter consistência com a paleta e tipografia acima
2. Priorizar performance e compatibilidade mobile (especialmente Safari iOS)
3. Antes de criar um novo componente, verificar se já existe um padrão no projeto
4. Preservar o estilo visual existente ao editar — não "modernizar" sem instrução explícita
5. Sugerir melhorias de acessibilidade quando relevante (alt texts, contraste, foco)
