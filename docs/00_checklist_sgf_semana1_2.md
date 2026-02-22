# SGF — Checklist Operacional (Semanas 1 e 2)

Objetivo: manter trilha única do SGF com baixa carga cognitiva e evidência incremental em Git.

Escopo coberto:

- Front (PFE/CFE)
- Processos
- SAD
- RL/IA (base lógica)

Status esperado ao final da Semana 2: ambiente estável, semanticamente estruturado e pronto para evolução analítica.

---

# 🔷 SEMANA 1 — BASELINE SGF
Período: 09/02–15/02  
Foco: colocar o ecossistema de pé

---

## 🧱 FRONT — Baseline do Dashboard

### Preparação da planilha SGF

- [ ] Garantir colunas mínimas:
  - [ ] Item
  - [ ] Quantidade
  - [ ] Valor_Unitario
  - [ ] Valor_Total = Quantidade * Valor_Unitario
- [ ] Remover células vazias nas colunas críticas
- [ ] Ordenar por Valor_Total (decrescente)
- [ ] Validar consistência numérica

**Resultado esperado:** planilha pronta para análise e publicação.

---

### Publicação no Google Sheets

- [ ] Upload da planilha
- [ ] Arquivo → Compartilhar → Publicar na web
- [ ] Copiar link `pubhtml`
- [ ] Testar abertura direta no navegador

**Critério de aceite:** link público funcionando sem autenticação.

---

### Dashboard mínimo (index.html)

Garantir que o arquivo contenha:

- [ ] `<!DOCTYPE html>`
- [ ] `<html lang="pt-BR">`
- [ ] `<head>` com `<meta charset>`
- [ ] `<title>` definido
- [ ] `<iframe>` apontando para o pubhtml
- [ ] largura 100%
- [ ] altura ~600px
- [ ] borda desabilitada

**Teste obrigatório:**

- [ ] abre localmente
- [ ] abre via GitHub Pages

---

### Organização do repositório

Estrutura mínima:
/sgf-dashboard
├─ index.html
├─ README.md
└─ docs/

Commit sugerido:


baseline SGF


---

## ⚙️ PROCESSOS — Fundamentos aplicados ao SGF

Criar:
docs/01_processos_aula1.md

Conteúdo mínimo:

- [ ] definição do problema SGF
- [ ] conceito de processo
- [ ] noção de atividade e artefato
- [ ] evidência via Git/Markdown
- [ ] fluxo de entregas incrementais

**Critério de maturidade:** documento curto, direto e versionado.

---

## 📊 SAD — Contexto BI/DM do SGF

Validar na planilha:

- [ ] Valor_Total calculado corretamente
- [ ] ordenação por impacto financeiro
- [ ] ausência de texto em colunas numéricas

Preparar leitura analítica:

- [ ] identificar item de maior impacto
- [ ] identificar concentração de custos
- [ ] reconhecer potencial para Curva ABC

**Objetivo:** preparar terreno analítico sem ainda formalizar a ABC.

---

## 🧠 RL / IA — Base proposicional

Definir proposições a partir da planilha.

Modelo recomendado:

- P: item possui alto valor
- Q: item pertence à categoria elétrica
- R: item é classificado como crítico

Checklist:

- [ ] proposições bem definidas
- [ ] cada proposição tem valor lógico claro
- [ ] sem uso de conectivos ainda
- [ ] exemplos coerentes com a planilha real

**Resultado esperado:** base lógica pronta para expansão.

---

---

# 🔷 SEMANA 2 — CONSOLIDAÇÃO
Período: 16/02–22/02  
Foco: estruturar sem aumentar carga cognitiva

---

## 🧱 FRONT — HTML semântico e qualidade estrutural

Atualizar `index.html`.

### Semântica

- [ ] inserir `<header>`
- [ ] inserir `<main>`
- [ ] inserir `<footer>`
- [ ] manter hierarquia correta de headings

---

### SEO mínimo

No `<head>`:

- [ ] `<meta name="description">` preenchida
- [ ] título coerente com SGF

---

### Acessibilidade (a11y)

No iframe:

- [ ] atributo `title`
- [ ] estrutura semântica válida
- [ ] leitura clara do documento

---

### Regressão funcional

- [ ] iframe continua carregando
- [ ] GitHub Pages funcional
- [ ] layout não quebrou

Commit sugerido:
html semantico + a11y


---

## ⚙️ PROCESSOS — Modelos prescritivos no SGF

Registrar análise comparativa:

- [ ] modelo Cascata aplicado ao SGF
- [ ] modelo Espiral aplicado ao SGF
- [ ] modelo em V aplicado ao SGF
- [ ] justificativa de adequação

Criar:
docs/02_modelos_processo_sgf.md


**Critério de qualidade:** análise objetiva, sem excesso teórico.

---

## 📊 SAD — Estatística descritiva inicial

Na planilha SGF calcular:

- [ ] soma do Valor_Total
- [ ] média do Valor_Total
- [ ] valor máximo
- [ ] valor mínimo

Reflexões esperadas:

- [ ] concentração de custos
- [ ] dispersão dos valores
- [ ] indício de itens críticos

**Objetivo:** preparar base quantitativa para Curva ABC.

---

## 🧠 RL / IA — Conectivos e equivalências

Expandir proposições da Semana 1.

Introduzir:

- [ ] conjunção (E)
- [ ] disjunção (OU)
- [ ] negação (NÃO)
- [ ] implicação (→)

Exemplos esperados no contexto SGF:

- [ ] regra de inspeção
- [ ] regra de criticidade
- [ ] combinação de condições

Validar:

- [ ] construção de pelo menos 1 tabela-verdade
- [ ] verificação de equivalência simples
- [ ] coerência com dados reais

---

# 🛡️ Regras de Blindagem Operacional

Durante estas duas semanas evitar:

- ❌ introduzir Prolog ainda
- ❌ adicionar JavaScript pesado
- ❌ estilização CSS avançada
- ❌ modelagem UML formal
- ❌ algoritmos de ML

Prioridade absoluta:
funcionar > sofisticar
evidenciar > enfeitar
incrementar > reinventar


---

# ✅ Estado de Prontidão ao Final da Semana 2

O ambiente SGF deve estar:

- [ ] planilha confiável
- [ ] dashboard semântico funcional
- [ ] evidência versionada
- [ ] base lógica definida
- [ ] estatística descritiva calculada
- [ ] modelos de processo analisados

Se todos os itens estiverem marcados, a trilha está estável para avançar para:

- Curva ABC
- Regras em Prolog
- Evolução analítica do SGF
