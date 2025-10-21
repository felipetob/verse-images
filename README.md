
# 2️⃣ Cambia al branch principal
git checkout main

# 3️⃣ Elimina todo menos el README.md (opcional)
find . -maxdepth 1 ! -name '.git' ! -name 'README.md' -exec rm -rf {} +

# 4️⃣ Dile a Git que borre todo
git rm -rf .

# 5️⃣ (Opcional) Si quieres conservar README.md
git restore README.md

# 6️⃣ Commit y push
git commit -m "clean repository"
git push origin main
