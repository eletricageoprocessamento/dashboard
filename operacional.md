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
