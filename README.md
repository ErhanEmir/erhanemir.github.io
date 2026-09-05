# Erhan Emir — Kişisel Site (ErhanEmir.github.io)

Modern koyu temalı, TR/EN dilli, tek dosyalık (`index.html`) kişisel portfolyo.
Hakkımda • Yetenekler • Projeler (GitHub API'den canlı) • Yazılar • İletişim.

## Yayınlama (GitHub Pages)

Bu klasördeki siteyi `https://ErhanEmir.github.io` adresinde yayınlamak için:

1. GitHub'da **yeni repo** aç, adı tam olarak: `ErhanEmir.github.io` (Public)
2. Bu klasörü o repoya push'la:
```powershell
cd C:\Users\eminb\Desktop\projeler\githubio
git init
git add .
git commit -m "Kisisel site ilk surum"
git branch -M main
git remote add origin https://github.com/ErhanEmir/ErhanEmir.github.io.git
git push -u origin main
```
3. Repo → **Settings → Pages** → Deploy from branch → `main` / `/ (root)` seç. 1-2 dk sonra yayında.
4. LinkedIn linkini `index.html` içinde `https://www.linkedin.com/` geçen yeri kendi profilinle değiştir.

## Yerelde önizleme
```powershell
cd C:\Users\eminb\Desktop\projeler\githubio
python -m http.server 8000
# http://localhost:8000
```

## Özelleştirme
- İsim/unvan: `index.html` → hero + profile kartı
- Yetenek yüzdeleri: `<script>` içinde `skills` dizisi
- Projeler: featured 3 kart + otomatik GitHub listesi (`ghRepos`)
- Dil: `TR` butonu, `localStorage` ile hatırlanır. Varsayılan tarayıcı diline göre.
- Tema: `◐` butonu (dark/light).
