# 🏆 Folder Titles - Tim Lagger

Folder ini untuk menyimpan **gambar title/badge** setiap member.

## ✅ Current Members (12/30)

| No | Member | Title File | Stats (STR/INT/LUCK) | Total | Type |
|----|--------|------------|----------------------|-------|------|
| 1  | **Evarick** | `title 1.png` | 70 / 70 / 70 | 210 | 🎯 Balanced |
| 2  | **LunaAan** | `title 2.png` | 79 / 81 / 58 | 218 | 🧠 Smart & Strong |
| 3  | **Rulers** | `title 3.png` | 87 / 81 / 53 | 221 | 💪 Powerhouse |
| 4  | **Rudeus** | `title 4.png` | 65 / 88 / 72 | 225 | 🎓 Genius |
| 5  | **Orion** | `title 5.png` | 92 / 68 / 75 | 235 | ⚔️ Warrior |
| 6  | **redflash** | `title 6.png` | 84 / 76 / 91 | 251 | 🍀 Lucky Beast |
| 7  | **Asan** | `title 7.png` | 58 / 82 / 64 | 204 | 📚 Strategist |
| 8  | **Newb** | `title 8.png` | 45 / 62 / 89 | 196 | 🎲 Lucky Rookie |
| 9  | **LovaNoona** | `title 9.png` | 73 / 85 / 78 | 236 | 👑 All-rounder |
| 10 | **Oggy** | `title 10.png` | 81 / 59 / 93 | 233 | 🎰 Super Lucky |
| 11 | **Gxvts** | `title 11.png` | 77 / 91 / 68 | 236 | 🧙 Mastermind |
| 12 | **Indo'Tuo** | `title 12.png` | 69 / 74 / 88 | 231 | 🎴 Fortunate |
| 13-30 | _TBA_ | `title 13.png` - `title 30.png` | - | - | 🔜 Future |

## 📐 Spesifikasi Gambar Title:

- **Ukuran Badge:** 320px × 96px (2x lebih besar!)
- **Format:** PNG (recommended untuk transparansi), JPG, WEBP
- **Naming:** `title 1.png`, `title 2.png`, `title 3.png`, dst.
- **Style:** Pixel art / retro gaming style (sesuai tema website)
- **Background:** Transparan atau sesuai desain

## 📝 Cara Tambah Title Gambar:

1. **Save gambar title dengan format:** `title [nomor].png`
2. **Taruh di folder `titles/`**
3. Gambar akan otomatis muncul di badge member yang sesuai
4. Jika gambar tidak ada, akan muncul placeholder text "TITLE"

## 🎮 Cara Kerja System:

```html
<img src="titles/title 1.png" 
     alt="Evarick Title" 
     onload="this.style.display='block'; 
             this.nextElementSibling.style.display='none'">
<span>TITLE</span>
```

- Jika gambar berhasil load → gambar tampil, text "TITLE" hilang
- Jika gambar gagal load → gambar hidden, text "TITLE" tetap tampil

## ➕ Template untuk Tambah Member Baru:

Copy-paste block ini di `index.html` (section roster):

```html
<!-- Member #[nomor]: [nama] -->
<div class="player" data-str="50" data-int="50" data-luck="50">
  <button class="player-row" onclick="togglePlayer(this)">
    <span class="player-name">[Nama Member]</span>
    <div class="title-badge">
      <img src="titles/title [nomor].png" alt="[Nama] Title" onload="this.style.display='block'; this.nextElementSibling.style.display='none'">
      <span>TITLE</span>
    </div>
    <svg class="chev" viewBox="0 0 24 24" width="16" height="16" fill="none" stroke="currentColor" stroke-width="2"><path d="M6 9l6 6 6-6"/></svg>
  </button>
  <div class="player-stats">
    <div class="stat-row">
      <span class="stat-label">Kekuatan</span>
      <div class="stat-track"><div class="stat-fill str"></div></div>
      <span class="stat-value">0</span>
    </div>
    <div class="stat-row">
      <span class="stat-label">Kecerdasan</span>
      <div class="stat-track"><div class="stat-fill int"></div></div>
      <span class="stat-value">0</span>
    </div>
    <div class="stat-row">
      <span class="stat-label">Keberuntungan</span>
      <div class="stat-track"><div class="stat-fill luck"></div></div>
      <span class="stat-value">0</span>
    </div>
  </div>
</div>
```

## 📊 Stats Member Saat Ini:

| Member | Kekuatan | Kecerdasan | Keberuntungan | Total |
|--------|----------|------------|---------------|-------|
| **Evarick** | 70 | 70 | 70 | 210 (Balanced) |
| **LunaAan** | 79 | 81 | 58 | 218 (Smart & Strong) |
| **Rulers** | 87 | 81 | 53 | 221 (Powerhouse) |

- `data-str` = **Kekuatan** (Strength) → 0-100
- `data-int` = **Kecerdasan** (Intelligence) → 0-100  
- `data-luck` = **Keberuntungan** (Luck) → 0-100

Angka-angka ini bisa disesuaikan sesuai "karakter" tiap member!

---

**Status:**
- ✅ Folder titles sudah dibuat
- ✅ 3 member pertama sudah setup (Evarick, LunaAan, Rulers)
- ⏳ Siap untuk 27 member tambahan (total target: 30)
- ⏳ Waiting for title images: `title 1.png` - `title 30.png`
