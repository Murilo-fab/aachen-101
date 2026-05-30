# aachen-101

Bem-vindo ao repositório de conteúdo do nosso blog! Este espaço foi criado para centralizar dicas, guias e informações práticas para estudantes brasileiros que estão de mudança ou já vivem em Aachen.

Toda a parte técnica e de publicação é automatizada. **Para contribuir com um novo artigo ou atualizar uma informação, você não precisa mexer em nenhum código**, basta adicionar ou editar um arquivo de texto (Markdown) na pasta `content/`.

---

## 🚀 Como Contribuir (Passo a Passo)

Como os workflows de deploy já estão configurados, o site se atualiza sozinho assim que um novo texto é adicionado à branch principal. Para enviar um artigo:

1. Navegue até a pasta `content/`.
2. Escolha a subpasta da categoria que melhor se encaixa no seu tema (veja a lista abaixo).
3. Crie um novo arquivo com a extensão `.md` (ex: `aluguel-estudantil.md`).
4. Insira o **Front-Matter** obrigatório no topo do arquivo (regrinhas abaixo).
5. Escreva o seu texto usando Markdown padrão e faça o Commit/Pull Request.

---

## 📂 Organização das Pastas (Categorias)

Para manter o site organizado, coloque o seu arquivo `.md` dentro de uma pastas em `content/` e indique a categória correspondente no Front-Matter:

*   `moradia/` – Como achar WG, Studierendenwerk, contratos de aluguel.
*   `estudos/` – Dicas de disciplinas da RWTH/FH Aachen, exames, bibliotecas.
*   `burocracias/` – Vistos, seguro saúde, Anmeldung, Sparkasse/Deutsche Bank, etc.
*   `viagens/` – Como usar o Semesterticket, viagens de trem, destinos perto da fronteira.
*   `aachen/` – O que fazer na cidade, restaurantes, pubs (Ponttor), integração.

---

## ⚠️ Regras Estritas de Formatação (Fail-Fast)

O nosso gerador de site (`another-ssg`) possui uma arquitetura de validação estrita. **Se o seu arquivo esquecer de alguma dessas informações abaixo, o build vai falhar** e o site não será atualizado.

### 1. O Front-Matter Obrigatório
Todo arquivo de texto precisa começar exatamente com as três variáveis abaixo preenchidas, delimitadas por três traços (`---`):

```yaml
title: Como conseguir uma vaga no Studierendenwerk
category: Moradia
date: 2026-05-29
toc: true
---