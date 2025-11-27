# 📘 Java Cheat Sheet

## 🔑 Modificadores de Acesso
- **public** → acesso global
- **protected** → classe, pacote e subclasses
- **default (package-private)** → apenas no mesmo pacote
- **private** → apenas dentro da classe

---

## 📂 Estrutura de Diretórios (MVC)
- **model** → entidades e objetos de domínio
- **repository** → acesso a dados (DAO/JPA)
- **service** → regras de negócio
- **controller** → expõe endpoints REST
- **view** → interface gráfica
- **util** → classes utilitárias

---

## 🌱 Git Essencial
- `git init` → inicia repositório
- `git add .` → adiciona arquivos
- `git commit -m "msg"` → cria commit
- `git push origin main` → envia alterações
- `git pull` → baixa alterações
- `git checkout -b branch` → cria branch
- `git merge branch` → mescla branch
- `git stash` → guarda alterações temporárias
- `git reset --hard <hash>` → desfaz commit

---

## 🗂 Collections
- **List** → ordenada, aceita duplicados
- **Set** → não aceita duplicados
- **Map** → chave-valor

---

## ⚡ Streams
**Intermediárias** → `filter`, `map`, `sorted`, `distinct`, `limit`, `skip`  
**Terminais** → `forEach`, `collect`, `reduce`, `count`, `anyMatch`, `allMatch`, `noneMatch`

```java
nomes.stream()
     .filter(n -> n.startsWith("A"))
     .map(String::toUpperCase)
     .forEach(System.out::println);
