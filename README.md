Perfeito — o que falta agora é **transformar o “processo” em um Fluxo (página própria no GitHub Pages)**, igual você já fez com AE/NPS/Case. A planilha (Excel/Sheets) fica como **sub-link** dentro do Fluxo, e o Hub aponta para o **site do fluxo** (não direto pra planilha). Assim fica 100% correto e padronizado.

Abaixo vai o **passo a passo completo** pra criar o novo Git + GitHub Pages + adicionar o processo + adicionar o link da planilha + atualizar o Hub.

---

# 1) Criar um novo repositório no GitHub (padrão dos seus fluxos)

1. Entre no GitHub → **New repository**
2. Nomeie com o padrão que você já usa, por exemplo:

   * `fluxo-mrr-x-churn-cscx-sankhya-abc-paulista`
3. Marque:

   * ✅ Public
   * ✅ Add a README
4. Create repository

---

# 2) Ativar o GitHub Pages

1. No repositório novo, vá em **Settings → Pages**
2. Em **Build and deployment**:

   * Source: **Deploy from a branch**
   * Branch: **main**
   * Folder: **/(root)**
3. Salve.
4. O GitHub vai te entregar a URL (vai ficar nesse padrão):

   * `https://germaninho.github.io/fluxo-mrr-x-churn-cscx-sankhya-abc-paulista/`

---

# 3) Criar o arquivo do Fluxo (index.html)

Você pode fazer de 2 formas:

## Opção A (mais rápida): pelo próprio GitHub

1. No repo → **Add file → Create new file**
2. Nome: `index.html`
3. Cole o HTML do fluxo (o conteúdo do processo)
4. Commit.

## Opção B (padrão dev): via Git no PC

1. Abra um terminal na pasta que você usa pros fluxos
2. Rode:

```bash
git clone https://github.com/germaninho/fluxo-mrr-x-churn-cscx-sankhya-abc-paulista.git
cd fluxo-mrr-x-churn-cscx-sankhya-abc-paulista
```

3. Crie `index.html`, cole o conteúdo, e rode:

```bash
git add .
git commit -m "Cria Fluxo MRR x Churn"
git push
```

---

# 4) Conteúdo do Fluxo (o “processo” + link do Excel)

Dentro do `index.html` do novo fluxo, você precisa ter:

* **Título:** Fluxo MRR x Churn
* **Objetivo do fluxo**
* **Pré-requisitos** (Unidade, período, etc.)
* **Passo a passo que você colou** (do item 1 ao 6)
* **Link do Google Sheets** (o seu link)
* (Opcional) seção “Validações” e “Erros comuns” (ex.: divergência por competência/classificação)

✅ O link da planilha entra como botão tipo:

* “Abrir planilha — MRR x Churn”

---

# 5) Atualizar o Hub (apontar para o Fluxo, e não direto pra planilha)

Hoje você colocou no Hub o link direto do Sheets. O correto no padrão “Fluxo” é:

### No Hub, trocar para:

```html
<!-- ✅ NOVA ABA: Fluxo MRR x Churn -->
<li>
  <a class="nav-link"
     href="https://germaninho.github.io/fluxo-mrr-x-churn-cscx-sankhya-abc-paulista/">
    <i class="ion-arrow-graph-up-right"></i>
    <span class="nav-text">Fluxo MRR x Churn</span>
  </a>
</li>
```

E **dentro** do novo fluxo (index.html do repo novo), você mantém o link da planilha.

---

# 6) Checklist final (pra ficar “100% correto”)

* [ ] Repo criado com nome padrão
* [ ] Pages habilitado (main / root)
* [ ] `index.html` publicado
* [ ] Fluxo contém:

  * [ ] Passo 1 a 6 (seu texto)
  * [ ] Link do Sheets
  * [ ] Regras de conferência (Dez–Nov etc.)
* [ ] Hub aponta para o **GitHub Pages do fluxo**
* [ ] Testar no navegador (Hub → Fluxo → Sheets)

---

Se você quiser, eu já te devolvo **o `index.html` completo do Fluxo MRR x Churn** (bonitinho no mesmo padrão visual dos seus fluxos) com:

* o texto do processo formatado,
* botão “Abrir planilha — MRR x Churn”,
* e uma seção “Checklist de amarração” (Ganhos – Perdas = variação da carteira).

Só me diga: você quer esse fluxo com **layout simples (texto + botão)** ou com o **mesmo estilo “Hub” (sidebar/hero)**?
