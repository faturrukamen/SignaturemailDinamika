# Dinamika Polimerindo Email Signature Generator

Generator email signature untuk PT Dinamika Polimerindo dengan fitur **banner event seasonal**.

🔗 **Live:** https://faturrukamen.github.io/SignaturemailDinamika/

---

## Cara Update Banner Event

### 1. Tambah gambar banner
Upload gambar banner ke folder `banners/` (format: JPG/PNG, lebar ideal 600px).

### 2. Edit `events.json`

```json
{
  "events": [
    {
      "id": "nama-event-tahun",
      "name": "Nama Event",
      "date": "19–23 Mei 2026",
      "banner_url": "https://raw.githubusercontent.com/faturrukamen/SignaturemailDinamika/main/banners/nama-file.jpg",
      "link": "https://website-event.com",
      "active": true,
      "is_new": true
    }
  ]
}
```

### 3. Push ke GitHub → otomatis live

```bash
git add banners/nama-file.jpg events.json
git commit -m "Add event banner: Nama Event"
git push
```

---

## Struktur Repo

```
SignaturemailDinamika/
├── index.html        ← Generator (deploy via GitHub Pages)
├── events.json       ← Config banner aktif
└── banners/          ← Folder gambar banner event
    └── .gitkeep
```

