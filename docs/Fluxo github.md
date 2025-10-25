# 📘 Fluxo Github - Padrões de Projeto & Desenvolvimento

> Guia prático e amigável para gerenciar branches, releases, correções e versões de forma simples.

---

## 🌿 Branches principais

* `master` → Produção ✅
* `develop` → Código pronto para próxima release 🔄
* `feature/*` → Novas funcionalidades ✨
* `bugfix/*` → Correções não urgentes 🐞
* `hotfix/*` → Correções urgentes em produção 🩹

> Nunca commit direto em `master` ou `develop`. Use branches e PRs.

---

## 🧾 Passo a passo diário

1️⃣ **Atualizar develop:**

```bash
git checkout develop
git pull origin develop
```

2️⃣ **Criar branch de trabalho:**

```bash
git checkout -b feature/nome-curto
```

3️⃣ **Commits claros:**

* `feat: adicionar botão de compartilhar`
* `fix: corrigir validação`
* `chore: atualizar dependências`

4️⃣ **Subir branch e abrir PR:**

```bash
git push -u origin feature/nome-curto
```

* PR para `develop`, revisão de pelo menos 1 pessoa.

5️⃣ **Merge em develop:**

* Use `Squash and merge` ou `Rebase` para histórico limpo.

---

## 🚀 Release / Deploy

1️⃣ Preparar release (opcional):

```bash
git checkout -b release/vX.Y.Z
```

2️⃣ Merge para `master` → deploy
3️⃣ Merge `master` → `develop`
4️⃣ Criar tag de versão:

```bash
git tag -a v1.2.3 -m "Release v1.2.3"
git push origin v1.2.3
```

> Use Semantic Versioning: `MAJOR.MINOR.PATCH`

---

## 🩹 Hotfix

1️⃣ Criar branch a partir de master:

```bash
git checkout master
git pull origin master
git checkout -b hotfix/descricao
```

2️⃣ Corrigir, commit e PR para master
3️⃣ Tag + merge em develop

---

## 🧰 Dicas rápidas

* Commits claros (`type(scope): breve descrição`)
* PR sempre com descrição e passos para testar
* CI para lint, build e testes
* Tests mínimos para fluxos principais
* Atualize docs/ sempre que mudar padrões

---

## ✅ Check-list antes da release

* [ ] develop testado e estável
* [ ] CHANGELOG atualizado
* [ ] Versionamento atualizado
* [ ] Tests passando
* [ ] Tag criada e push

---

## 🎯 Resumo do fluxo

`feature/*` → develop → release → master + tag → deploy
Hotfix → master → tag → merge develop
