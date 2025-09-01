# 📘 Glossário Git/Gitflow

### 🔹 Configuração inicial
```bash
git init
```
👉 Inicia um repositório Git no diretório atual.  

```bash
git remote add origin <url-do-repo>
```
👉 Conecta seu repositório local ao remoto (GitHub/GitLab etc.).  

---

### 🔹 Branch principal
```bash
git checkout main
```
👉 Troca para a branch `main`.  

```bash
git pull origin main
```
👉 Atualiza sua `main` com o remoto.  

---

### 🔹 Criar branch develop
```bash
git checkout -b develop
git push -u origin develop
```
👉 Cria a branch `develop` a partir da `main` e envia para o remoto.  

---

### 🔹 Inicializar Gitflow
```bash
git flow init
```
👉 Configura o Gitflow no repositório (pede a branch principal e a de desenvolvimento).  

---

### 🔹 Features (novas funcionalidades)
```bash
git flow feature start nome-da-feature
```
👉 Cria uma branch `feature/nome-da-feature` a partir da `develop`.  

```bash
git flow feature finish nome-da-feature
```
👉 Finaliza a feature, faz merge na `develop` e apaga a branch da feature.  

---

### 🔹 Release (preparar versão)
```bash
git flow release start v1.0.0
```
👉 Cria a branch `release/v1.0.0` a partir da `develop`.  

```bash
git flow release finish v1.0.0
```
👉 Faz merge na `main` e na `develop`, cria **tag** da versão e apaga a release.  

---

### 🔹 Hotfix (corrigir bug urgente em produção)
```bash
git flow hotfix start hotfix-1.0.1
```
👉 Cria a branch `hotfix/hotfix-1.0.1` a partir da `main`.  

```bash
git flow hotfix finish hotfix-1.0.1
```
👉 Faz merge na `main` e na `develop`, cria **tag** da correção e apaga a branch.  

---

### 🔹 Operações básicas
```bash
git status
```
👉 Mostra status dos arquivos.  

```bash
git add .
```
👉 Adiciona todos os arquivos para commit.  

```bash
git commit -m "mensagem"
```
👉 Registra as mudanças no histórico.  

```bash
git push
```
👉 Envia commits para o repositório remoto.  

```bash
git pull
```
👉 Puxa mudanças do remoto para o local.  
