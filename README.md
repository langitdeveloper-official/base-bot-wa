# 🤖 Mahiru Base — Bot Whatsapp

![Version](https://img.shields.io/badge/version-1.0.0-blue)
![Node](https://img.shields.io/badge/Node.js-20.x-green)
![License](https://img.shields.io/badge/license-MIT-yellow)
![By](https://img.shields.io/badge/by-LangitDev-purple)
![WhatsApp](https://img.shields.io/badge/WhatsApp-Bot-25D366)

**Base Bot WhatsApp** yang dirancang modern dengan sistem **plugin** dan **case**. Mudah dikembangkan, ringan, dan siap pakai untuk berbagai keperluan

---

## 📁 Struktur Folder

```
mahiru/
├── 📂 Settings/
│   └── config.js          
├── 📂 database/
│   ├── owner.json
│   └── premium.json
├── 📂 lib/
│   ├── exif.js            
│   └── storage.js         
├── 📂 plugins/            
│   └── ping.js
├── index.js               
├── mahiru.js              
└── package.json
```

---

## ⚙️ Konfigurasi

Edit `Settings/config.js`:

```js
global.botName  = 'Mahiru'
global.prefix   = '.'
global.owner    = ['628xxxxxxxxxx']
global.publicX  = true   // false = self mode
```

---

## 🧩 Buat Plugin

Buat file baru di `plugins/namafitur.js`:

```js
exports.command = ['cmd']
exports.tags    = ['kategori']
exports.desc    = 'Deskripsi'

exports.handler = async ({ m, Reply, text, args, isOwner }) => {
  Reply('Halo!')
}
```

---

## 📦 Dependensi Utama

| Package | Kegunaan |
|---------|----------|
| `@whiskeysockets/baileys` | WhatsApp Web API |
| `axios` | HTTP request |
| `fluent-ffmpeg` | Konversi media |
| `jimp` | Manipulasi gambar |
| `moment-timezone` | Format waktu |

---

## 📄 Lisensi

MIT License — bebas digunakan dengan tetap mencantumkan kredit.

---

<p align="center">Made With By <strong>LangitDev</strong></p>
