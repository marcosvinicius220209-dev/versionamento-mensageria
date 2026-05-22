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

# 🧬 Tipos de Controle de Versão

## 🔹 Local

O histórico fica salvo apenas no computador do desenvolvedor.

### ✅ Vantagens

* Simples
* Rápido

### ❌ Desvantagens

* Sem backup online
* Alto risco de perda

---

## 🔹 Centralizado

Existe um servidor central responsável pelo versionamento.

### Exemplos

* SVN
* CVS

### ✅ Vantagens

* Controle centralizado
* Fácil administração

### ❌ Desvantagens

* Dependência do servidor
* Menor flexibilidade

---

## 🔹 Distribuído (Git)

Cada desenvolvedor possui uma cópia completa do repositório.

### ✅ Vantagens

* Maior segurança
* Trabalho offline
* Melhor desempenho
* Histórico completo local

---

# 🐙 Git vs GitHub

| Git | GitHub |
|------|--------|
| Sistema de versionamento | Plataforma de hospedagem |
| Funciona localmente | Funciona online |
| Controla histórico | Facilita colaboração |
| Criado por Linus Torvalds | Plataforma da Microsoft |

---

# ⚙️ Configuração Inicial do Git

```bash
# Configurar nome
git config --global user.name "Seu Nome"

# Configurar email
git config --global user.email "seuemail@email.com"

# Verificar configurações
git config --list