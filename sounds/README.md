# 🎵 Folder Sounds - Tim Lagger

Folder ini untuk menyimpan file musik background (BGM) website.

## ✅ Status: Sequential Playlist Active

Website sekarang menggunakan **sequential playlist system**:
- Lagu 1 → Lagu 2 → Lagu 3 → Lagu 4 → (repeat dari awal)

## 📂 File Musik Saat Ini:

1. ✅ `lagu 1.mpeg` - Track pertama
2. ✅ `lagu 2.mpeg` - Track kedua  
3. ✅ `lagu 3.mpeg` - Track ketiga
4. ✅ `lagu 4.mpeg` - Track keempat

## 🎮 Cara Kerja:

1. User klik/tap intro gate (splash screen)
2. Lagu 1 mulai play
3. Setelah lagu 1 selesai → otomatis lanjut ke lagu 2
4. Setelah lagu 4 selesai → kembali ke lagu 1 (looping)
5. SFX glitch akan muncul random selama musik play

## 🔧 Cara Tambah/Ganti Lagu:

Jika mau tambah lagu atau ganti urutan, edit di `index (4).html` sekitar line 800-806:

```javascript
var playlist = [
  'sounds/lagu 1.mpeg',
  'sounds/lagu 2.mpeg',
  'sounds/lagu 3.mpeg',
  'sounds/lagu 4.mpeg'
  // tambah lagu baru di sini
];
```

## 📝 Format yang Didukung:

- ✅ MP3 (.mp3)
- ✅ MPEG (.mpeg)
- ✅ WAV (.wav)
- ✅ OGG (.ogg)

---

**Dibuat:** Sequential playlist system implemented
**SFX Built-in:** ✅ 4 glitch sounds + 1 boot sound (synthesized)

