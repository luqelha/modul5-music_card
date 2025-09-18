# 🎶 Music Card - Flutter Example

Proyek ini menampilkan contoh implementasi **Music Card** di Flutter dengan menggabungkan widget **Card**, **SizedBox**, dan **Spacer**.  
Tujuan utamanya adalah memahami bagaimana tata letak (layout) bekerja secara fleksibel dan rapi di Flutter.

---

## 📌 Tentang Proyek
- **Nama Proyek:** music_card_example  
- **Deskripsi:** Contoh sederhana pembuatan kartu musik dengan cover album, judul lagu, nama artis, progress bar, dan tombol play.  
- **Tujuan:**
  - Mengenal penggunaan **Card** untuk tampilan container dengan elevation dan border radius.
  - Menggunakan **SizedBox** sebagai jarak antar widget.
  - Memanfaatkan **Spacer** untuk mengatur tata letak agar elemen tertentu terdorong ke bawah.
  - Mengombinasikan dengan **Expanded** agar informasi lagu fleksibel mengikuti sisa ruang.

---

## 🔲 Konsep Utama

### 📐 Card
Membungkus seluruh konten dalam sebuah kartu dengan efek **elevation** dan **rounded corner**.

```dart
Card(
  elevation: 6,
  shape: RoundedRectangleBorder(
    borderRadius: BorderRadius.circular(16),
  ),
  child: ...
)
```

```dart
const SizedBox(width: 16),
Column(
  children: [
    Text("Song Title"),
    Text("Artist Name"),
    Spacer(), // progress bar terdorong ke bawah
    LinearProgressIndicator(...),
  ],
)
```
