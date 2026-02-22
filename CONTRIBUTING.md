# Como Editar o Site do LAFISE

Este guia explica como os membros do laboratório podem adicionar e editar conteúdo no site.

## Pré-requisitos

- Uma conta no [GitHub](https://github.com)
- Ser colaborador do repositório (peça acesso ao administrador)

## Como funciona

O site é gerado automaticamente a partir de arquivos de texto simples (Markdown). Quando você cria ou edita um arquivo no GitHub e abre um **Pull Request**, outro membro revisa e aprova a mudança. Após a aprovação e o merge, o site é atualizado automaticamente em cerca de 2 minutos.

---

## Editando uma página existente

1. Acesse o repositório: https://github.com/rafael0torres/lafise-ufmg-website
2. Navegue até a pasta `content/` e encontre o arquivo que deseja editar
3. Clique no arquivo e depois no ícone de lápis (✏️) no canto superior direito
4. O GitHub vai criar automaticamente uma "branch" (cópia) para suas mudanças
5. Faça suas alterações no editor
6. Na parte inferior da página, escreva uma breve descrição da mudança (ex: "Atualizar email de contato")
7. Clique em **"Propose changes"**
8. Na próxima tela, clique em **"Create pull request"**
9. Aguarde outro membro do lab revisar e aprovar sua mudança

---

## Adicionando uma nova reunião científica

1. No repositório, navegue até `content/reunioes-cientificas/`
2. Clique em **"Add file"** > **"Create new file"**
3. Nomeie o arquivo no formato: `AAAA-MM-DD-titulo-resumido.md`
   - Exemplo: `2025-03-15-efeitos-exercicio-cognicao.md`
4. Cole o seguinte modelo e preencha com os dados da reunião:

```yaml
---
title: "Título da apresentação"
date: 2025-03-15
presenter: "Nome do(a) apresentador(a)"
presenter_role: "Ex: Mestrando(a) em Ciências do Esporte"
advisor: "Prof. Dr(a). Nome do(a) orientador(a)"
tags: ["palavra-chave-1", "palavra-chave-2"]
---

Descrição ou resumo da apresentação aqui.
```

5. Clique em **"Propose new file"** e depois **"Create pull request"**

---

## Adicionando uma publicação (artigo)

1. Navegue até `content/publicacoes/artigos/`
2. Clique em **"Add file"** > **"Create new file"**
3. Nomeie o arquivo no formato: `AAAA-sobrenome-tema.md`
   - Exemplo: `2024-zanetti-heat-acclimation.md`
4. Cole o modelo:

```yaml
---
title: "Título completo do artigo"
date: 2024-01-15
authors: ["Sobrenome AB", "Sobrenome CD", "Sobrenome EF"]
journal: "Nome do Periódico"
year: 2024
doi: "10.1016/j.exemplo.2024.123456"
---
```

5. Clique em **"Propose new file"** e depois **"Create pull request"**

> **Dica:** Para dissertações, use a pasta `content/publicacoes/dissertacoes/`. Para teses, use `content/publicacoes/teses/`.

---

## Adicionando um membro da equipe

1. Navegue até `content/equipe/`
2. Clique em **"Add file"** > **"Create new file"**
3. Nomeie como `nome-sobrenome.md` (ex: `maria-silva.md`)
4. Cole o modelo:

```yaml
---
title: "Nome Completo"
role: "Ex: Mestrando(a), Doutorando(a), Professor(a)"
status: "active"
weight: 10
email: "email@exemplo.com"
lattes: "http://lattes.cnpq.br/..."
photo: ""
---

Breve biografia do membro.
```

5. Clique em **"Propose new file"** e depois **"Create pull request"**

> **Sobre o campo `weight`:** números menores aparecem primeiro na lista. Professores geralmente usam 1-5, pós-graduandos 10-20, graduandos 20+.

> **Sobre o campo `status`:** use `"active"` para membros atuais e `"alumni"` para ex-membros.

---

## Editando páginas gerais

As páginas de conteúdo geral ficam em:

| Página | Arquivo |
|--------|---------|
| Sobre o LAFISE | `content/o-lafise/_index.md` |
| Disciplinas | `content/disciplinas/_index.md` |
| Grupo de Pesquisa | `content/grupo-de-pesquisa/_index.md` |
| Contato | `content/contato.md` |
| Links | `content/links/_index.md` |

Basta navegar até o arquivo, clicar no lápis, editar e seguir o fluxo de Pull Request.

---

## Fluxo de revisão (Pull Request)

Todas as mudanças passam por revisão antes de irem ao ar:

1. Você propõe uma mudança (cria um Pull Request)
2. Outro membro do lab recebe uma notificação
3. O revisor analisa as mudanças e aprova (ou pede ajustes)
4. Após a aprovação, clique em **"Merge pull request"**
5. O site é atualizado automaticamente em ~2 minutos

---

## Formatação básica em Markdown

| O que você quer | O que escrever |
|----------------|----------------|
| **Negrito** | `**texto em negrito**` |
| *Itálico* | `*texto em itálico*` |
| Link | `[texto do link](https://url.com)` |
| Lista com marcadores | `- item` (uma linha por item) |
| Lista numerada | `1. item` (uma linha por item) |
| Título grande | `## Título` |
| Título menor | `### Subtítulo` |

---

## Dúvidas?

Se tiver dúvidas sobre como editar o site, entre em contato com o administrador do repositório.
