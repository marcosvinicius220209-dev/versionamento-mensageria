---

# 🏗️ Guia Completo de Versionamento com Git & GitHub

> 📌 Esta seção complementa o estudo de versionamento abordando fluxos profissionais, organização de equipes, automação e boas práticas utilizadas em projetos reais.

---

# 📖 O que é Versionamento?

Versionamento é o processo de registrar e controlar alterações realizadas em arquivos ao longo do tempo.

Com o Git, é possível:

* 🔄 Recuperar versões antigas
* 👥 Trabalhar em equipe sem sobrescrever código
* 🧠 Organizar o histórico do projeto
* 🚀 Automatizar processos de desenvolvimento
* 🛡️ Garantir maior segurança nas alterações

---

# 🐙 Git vs GitHub

| Git | GitHub |
|------|--------|
| Sistema de versionamento | Plataforma de hospedagem |
| Funciona localmente | Funciona online |
| Controla histórico | Facilita colaboração |

---

# ⚙️ Configuração Inicial do Git

```bash
git config --global user.name "Seu Nome"

git config --global user.email "seuemail@email.com"

git config --list
```

---

# 📁 Inicializando um Repositório

```bash
# Criar repositório Git
git init

# Clonar projeto existente
git clone https://github.com/usuario/repositorio.git
```

---

# 📌 Estados dos Arquivos no Git

| Estado | Descrição |
|--------|------------|
| Modified | Arquivo alterado |
| Staged | Arquivo preparado |
| Committed | Alteração salva |

---

# 🔄 Fluxo Completo de Trabalho

```bash
git status

git add .

git commit -m "feat: adiciona tela de login"

git push origin main
```

---

# 🧾 Conventional Commits

## 📌 Estrutura

```bash
tipo: descrição
```

## 📌 Exemplos

```bash
feat: adiciona sistema de autenticação
fix: corrige erro de validação
docs: atualiza documentação
style: ajusta formatação
refactor: melhora estrutura do código
test: adiciona testes unitários
chore: atualiza dependências
```

---

# 🌿 Trabalhando com Branches

## 📌 Criar Branch

```bash
git checkout -b feature/login
```

## 📌 Trocar de Branch

```bash
git checkout main
```

## 📌 Listar Branches

```bash
git branch
```

## 📌 Excluir Branch

```bash
git branch -d feature/login
```

---

# 🔀 Merge vs Rebase

| Merge | Rebase |
|--------|---------|
| Mantém histórico completo | Histórico mais limpo |
| Cria merge commit | Reescreve histórico |

---

## 🔄 Exemplo Merge

```bash
git checkout main
git merge feature/login
```

---

## 🔄 Exemplo Rebase

```bash
git checkout feature/login
git rebase main
```

---

# 🧩 Resolução de Conflitos

Conflitos acontecem quando duas alterações modificam a mesma linha.

## 📌 Passos para Resolver

1. Abrir arquivo conflitante
2. Escolher qual alteração manter
3. Salvar arquivo
4. Finalizar merge

```bash
git add .
git commit
```

---

# 🏷️ Tags e Versionamento Semântico

## 📌 Criar Tag

```bash
git tag v1.0.0
```

## 📌 Enviar Tags

```bash
git push origin --tags
```

---

# 🔢 Semantic Versioning (SemVer)

Formato:

```bash
MAJOR.MINOR.PATCH
```

## 📌 Exemplo

```bash
1.4.2
```

| Tipo | Significado |
|------|--------------|
| MAJOR | Mudanças incompatíveis |
| MINOR | Novas funcionalidades |
| PATCH | Correções |

---

# 🚀 Git Flow

| Branch | Objetivo |
|--------|-----------|
| main | Produção |
| develop | Desenvolvimento |
| feature/* | Novas funcionalidades |
| release/* | Preparação de versão |
| hotfix/* | Correções urgentes |

---

## 📌 Exemplo

```bash
git checkout develop
git checkout -b feature/dashboard
```

---

# 🔐 Boas Práticas de Segurança

* ❌ Nunca subir senhas
* ❌ Nunca enviar arquivos `.env`
* ✅ Utilizar `.gitignore`
* ✅ Revisar commits antes do push

---

# 📄 Exemplo de .gitignore

```bash
node_modules/
.env
dist/
coverage/
```

---

# 🤝 Pull Requests

## 📌 Fluxo

1. Criar branch
2. Fazer alterações
3. Realizar push
4. Abrir Pull Request
5. Revisar código
6. Aprovar merge

---

# 👨‍💻 Code Review

O Code Review ajuda a:

* Encontrar bugs
* Melhorar qualidade
* Compartilhar conhecimento
* Padronizar código

---

# ⚡ GitHub Actions (CI/CD)

## 📌 Exemplos de Automação

* ✅ Testes automáticos
* 🚀 Deploy automático
* 🔍 Análise de código
* 📦 Build de aplicações

---

# 📂 Estrutura de Workflow

```bash
.github/
└── workflows/
    └── ci.yml
```

---

# 🧪 Exemplo de Workflow

```yaml
name: CI

on:
  push:
    branches:
      - main

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
      - name: Checkout
        uses: actions/checkout@v3

      - name: Instalar dependências
        run: npm install

      - name: Executar testes
        run: npm test
```

---

# 🛠️ Comandos Avançados

## 📌 Ver Histórico Completo

```bash
git log
```

## 📌 Histórico Resumido

```bash
git log --oneline
```

## 📌 Desfazer Alterações

```bash
git restore arquivo.txt
```

## 📌 Remover Arquivo do Stage

```bash
git reset arquivo.txt
```

## 📌 Voltar Commit

```bash
git revert HASH
```

---

# 📚 Principais Plataformas Git

* GitHub
* GitLab
* Bitbucket
* Azure DevOps

---

# 🎯 Benefícios do Versionamento

* 🧠 Organização
* 🔒 Segurança
* 🚀 Agilidade
* 👥 Colaboração
* 📈 Escalabilidade
* 🔄 Controle de mudanças

---

# 🏆 Dicas para se Destacar no Mercado

* ✅ Utilize Conventional Commits
* ✅ Faça Pull Requests organizados
* ✅ Escreva READMEs profissionais
* ✅ Domine Git Flow
* ✅ Automatize processos com CI/CD
* ✅ Documente alterações importantes

---

# 🧠 Conclusão

Dominar Git e GitHub vai muito além de salvar arquivos.

Versionamento é:

* 📖 Contar a evolução do projeto
* 👥 Facilitar colaboração
* 🚀 Automatizar entregas
* 🔒 Garantir segurança no desenvolvimento

---

> 💬 "Grandes projetos não são construídos apenas com código, mas com organização, colaboração e histórico bem versionado." 🚀

---