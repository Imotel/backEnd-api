
# 📖 Glossário de Branches no Git  

### 🔍 Verificar branches existentes
```bash
git branch
```
- Mostra todas as branches locais.  
- O `*` indica em qual branch você está.  

```bash
git branch -a
```
- Mostra também as branches remotas.  

---

### 🔄 Trocar de branch
```bash
git checkout nome-da-branch
```
ou (forma mais nova):
```bash
git switch nome-da-branch
```

---

### ➕ Criar nova branch
```bash
git checkout -b nome-da-branch
```
ou
```bash
git switch -c nome-da-branch
```

---

### ⬆️ Atualizar branch com a remota
1. Vá para a branch desejada:
   ```bash
   git checkout develop
   ```
2. Atualize:
   ```bash
   git pull origin develop
   ```

---

### 🚀 Subir nova branch para o repositório remoto
```bash
git push -u origin nome-da-branch
```

---

### 🗑️ Deletar uma branch
- Local:
  ```bash
  git branch -d nome-da-branch
  ```
- Remota:
  ```bash
  git push origin --delete nome-da-branch
  ```

---

👉 **Resumo do fluxo mais comum:**
1. **Listar branches** → `git branch -a`  
2. **Trocar** para a que você quer → `git checkout develop`  
3. **Atualizar** com o remoto → `git pull origin develop`  
4. **Criar** uma nova se precisar → `git checkout -b minha-feature`  
