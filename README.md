# ⚡ OPERAÇÃO AGV — Versão Acessível

Aplicação web educacional de página única (SPA) para ensinar conceitos de **eletrônica analógica** — especificamente **Amplificadores Operacionais (AmpOp)** e **condicionamento de sinais** — a estudantes com **Transtorno do Espectro Autista (TEA) Nível 3**.

O projeto usa a metáfora de um **AGV** (Automated Guided Vehicle / Veículo Guiado Automaticamente) que "não segue a linha" para introduzir, de forma concreta e sequencial, os conceitos de sensor, buffer, filtro, comparador e controlador.

---

## 🎯 Objetivo Pedagógico

Ensinar os fundamentos de sistemas eletrônicos de forma **acessível, previsível e literal**, respeitando as características do público-alvo:

- **Rotina previsível**: cada módulo segue a mesma estrutura de 5 etapas (Leia → Veja → Exemplos → Pratique → Responda).
- **Linguagem literal**: frases curtas, sem metáforas ambíguas, com apoio visual constante.
- **Integração de hiperfocos**: exemplos contextualizados em **futebol**, **aviação** e **rotinas/ordem**, temas comumente associados a interesses restritos.
- **Reforço positivo**: sistema de XP, medalhas e progresso visual.
- **Baixa carga cognitiva**: um conceito por vez, com repetição e feedback imediato.

---

## 🧩 Estrutura do Curso

O curso é dividido em **9 módulos sequenciais** (0 a 8), com desbloqueio progressivo:

| Módulo | Título | Tema | XP |
|--------|--------|------|----|
| 0 | O Problema | Introdução ao AGV e ao sinal ruidoso | 10 |
| 1 | O Cérebro do Condicionador | Amplificador Operacional (AmpOp) | 15 |
| 2 | O Manual do Chip | Leitura de *datasheet* | 15 |
| 3 | O Juiz do Circuito | Comparador (Vin vs Vref) | 20 |
| 4 | Antes de Ligar | Segurança e checklist | 15 |
| 5 | Medindo com Cuidado | Multímetro e osciloscópio | 20 |
| 6 | Achando o Problema | Diagnóstico em 5 passos | 20 |
| 7 | Anotando Tudo | Documentação técnica | 15 |
| 8 | Tudo Juntos | Arquitetura completa do sistema | 25 |

Cada módulo contém:
- **Conteúdo textual** adaptado;
- **Ilustrações SVG** acessíveis (com `role="img"` e `aria-label`);
- **Exemplos nos 3 hiperfocos**;
- **Atividade prática interativa** (sliders, canvas, checklists, formulários);
- **Quiz** com feedback corretivo e possibilidade de nova tentativa;
- **Requisitos de conclusão** claros.

---

## 🏅 Sistema de Gamificação

### Níveis (por XP acumulado)
- **Aprendiz** — 0 XP
- **Observador** — 40 XP
- **Praticante** — 100 XP
- **Técnico Júnior** — 180 XP
- **Técnico** — 280 XP

### Medalhas
| Medalha | Como conquistar |
|---------|-----------------|
| 🎉 Primeiro Passo | Concluir o Módulo 0 |
| 📖 Leitor Atento | Acerte o quiz do Módulo 1 |
| 👁️ Olho Técnico | Acerte o quiz do Módulo 2 |
| ⚽ Juiz Eletrônico | Acerte o quiz do Módulo 3 |
| 🛡️ Montador Cuidadoso | Faça o checklist do Módulo 4 |
| 📏 Medidor Preciso | Registre 1 medição no Módulo 5 |
| 🔍 Detetive | Revele a análise do Módulo 6 |
| 📋 Documentador | Salve o dossiê no Módulo 7 |
| 🏆 Integrador | Conclua o Módulo 8 |

---

## ♿ Recursos de Acessibilidade

- **Tipografia ampliada** (`font-size: 18px` na raiz, com ajustes em mobile).
- **Alvos de toque generosos** (mínimo 44–52px de altura em botões).
- **Alto contraste** entre texto e fundo.
- **Foco visível** com contorno laranja de 4px (`:focus-visible`).
- **Estrutura semântica**: `fieldset`, `legend`, `role="radiogroup"`, `aria-label`, `aria-disabled`.
- **Respeito a `prefers-reduced-motion`** (desativa animações).
- **Layout responsivo** (mobile-first a partir de 640px).
- **Feedback multimodal**: visual (cores, ícones), textual (mensagens claras) e sonoro/estrutural (toasts).
- **Imagens SVG com descrição textual** embutida.

---

## 🛠️ Tecnologias Utilizadas

- **HTML5** semântico
- **CSS3** puro (variáveis CSS, grid, flexbox, `container-type`, `aspect-ratio`)
- **JavaScript vanilla** (ES6+, sem frameworks)
- **SVG** inline para ilustrações
- **Canvas API** para simulação de osciloscópio
- **LocalStorage** para persistência de progresso

**Não há dependências externas** — o arquivo é 100% autocontido e funciona offline.

---

## 🚀 Como Usar

### Opção 1 — Abrir diretamente
1. Baixe o arquivo `index.html`.
2. Dê duplo clique ou abra em qualquer navegador moderno (Chrome, Firefox, Edge, Safari).

### Opção 2 — Servir localmente
```bash
# Python 3
python -m http.server 8000

# Node.js (com npx)
npx serve