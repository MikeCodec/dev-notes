# 🖤 Git Cheatsheet – Nivel Pro

---

# 1️⃣ Configuración Inicial
```bash
git config --global user.name "Mikecodec"
git config --global user.email "correo@example.com"
# **🚀 2️⃣ Crear repositorio y conectar con GitHub**  
---
git init
git remote add origin https://github.com/USUARIO/dev-notes.git
git branch -M main
git push -u origin main
3️⃣ ⚡ Flujo Básico de Trabajo
# Agregar cambios
git add .               # Todos los archivos
git add archivo.js       # Archivo específico

# Confirmar cambios
git commit -m "Mensaje claro y conciso"

# Subir cambios al remoto
git push
4️⃣ 🌿 Trabajar con Ramas (Branching)
# Crear y cambiar a una nueva rama
git checkout -b feature-login

# Cambiar de rama
git checkout main

# Fusionar rama en main
git checkout main
git pull
git merge feature-login
git push

# Renombrar rama
git branch -m nuevo-nombre

# Eliminar rama
git branch -d nombre-rama
git push origin --delete nombre-rama
5️⃣ 🔄 Colaboración / Actualizar desde GitHub
# Traer cambios del remoto
git pull origin main

# Clonar repositorio
git clone https://github.com/USUARIO/dev-notes.git
git checkout -b nombreRama origin/nombreRama
6️⃣ 🔥 Comandos Avanzados
# Ver historial de commits en grafo
git log --oneline --graph --all

# Guardar trabajo temporalmente
git stash
git stash pop

# Reaplicar cambios encima de otra rama
git rebase main

# Recuperar commits perdidos
git reflog

# Ver quién cambió una línea
git blame archivo.js
7️⃣ 🐞 Debugging Git / Problemas Comunes
# Ver cambios no confirmados
git diff

# Quitar archivo del staging
git reset HEAD archivo.js

# Restaurar archivo
git restore archivo.js

# Estado actual del repo
git status
8️⃣ 💀 Eliminación / Reinicio
# Eliminar repositorio local
Remove-Item -Recurse -Force .git   # Windows PowerShell
rm -rf .git                        # Linux / Mac

# Rehacer commit local (sin perder cambios)
git reset --soft HEAD~1

# Rehacer commit y descartar cambios
git reset --hard HEAD~1
9️⃣ 💡 Tips Pro Reales

Commits pequeños y claros, un commit = un cambio lógico

Branches para features, fixes, experiments; nunca trabajar directo en main

Antes de mergear, siempre git pull para evitar conflictos

git log --oneline --graph --decorate = tu mejor amigo para entender historial

Aprende a usar stash y rebase antes de depender solo de merges

10️⃣ ⚡ Cheatsheet Rápido
# Setup
git config --global user.name "Mikecodec"
git config --global user.email "correo@example.com"

# Workflow básico
git add .
git commit -m "mensaje"
git push
git pull

# Branch workflow
git checkout -b rama
git merge rama
git branch -d rama

# Debugging
git log --oneline --graph
git diff
git reflog
git reset HEAD archivo.js
git restore archivo.js

✅ Todo en un solo archivo continuo, con títulos grandes (H1), emojis y separadores visuales.
Perfecto para guardar como git-cheatsheet.md.


---

Si querés, puedo hacer **una versión todavía más “visual PRO”**, usando **tablas para comandos**, **colores de bloques**, y resaltando secciones críticas, que se vea casi como un Word profesional, **pero todo en Markdown y un solo archivo**.  

¿Quieres que haga eso también?

---- Ctrl + Shift + V ----