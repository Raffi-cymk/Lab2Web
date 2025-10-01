# Lab2Web - Praktikum 2: CSS Dasar

## 📖 Deskripsi
Praktikum ini dibuat untuk memenuhi tugas mata kuliah **Pemrograman Web**.  
Tujuannya adalah mempelajari dan memahami penggunaan **CSS Dasar** (Cascading Style Sheets) dengan penerapan pada:
- Inline CSS
- Internal CSS
- External CSS
- Selector (Element, Class, ID)
- Urutan prioritas (Cascade) pada CSS


---

## 📸 Screenshot
1. Tampilan `lab2_css_dasar.html` (Internal + Inline CSS)
<img width="1366" height="768" alt="Screenshot 2025-10-01 122350" src="https://github.com/user-attachments/assets/95a3e555-9a3e-43ef-b9ff-4ef29d307c4d" />

2. Tampilan `lab2_css_eksternal.html` (External CSS)  
<img width="1366" height="768" alt="Screenshot 2025-10-01 123936" src="https://github.com/user-attachments/assets/d694a5c0-078e-4a60-a1c1-5bdbd11d43b5" />

3. Validasi CSS eksternal di W3C (No Error Found)  
<img width="1366" height="768" alt="Screenshot 2025-10-01 124257" src="https://github.com/user-attachments/assets/db55342f-73d0-465b-b976-0e09b669fe3e" />

4. Screenshot kode CSS eksternal (`style_eksternal.css`) di VSCode
<img width="1366" height="768" alt="Screenshot 2025-10-01 122939" src="https://github.com/user-attachments/assets/e3b5ae8b-32f8-4ac0-a02b-d5b0c0fe76da" />

*(masukkan gambar hasil screenshot yang sudah lo ambil ke repo, contoh: `screenshot1.png`, `screenshot2.png`, dst)*


---

## ❓ Pertanyaan & Jawaban

**1. Lakukan eksperimen dengan mengubahan menambah properti CSS!**
Jawaban: 
Eksperimen dapat dilakukan dengan menambahkan properti baru, misalnya `background-color`, `padding`, `margin`, dan `border-radius`.  
Contoh:

```css
h1 {
  color: navy;
  font-size: 30px;
  background-color: lightyellow;
  padding: 10px;
  border-radius: 5px;
}

---

**2. Apa perbedaan h1 {...} dengan #intro h1 {...}?**
Jawaban:

h1 {...} → berlaku untuk semua elemen <h1> di halaman.

#intro h1 {...} → hanya berlaku untuk <h1> di dalam elemen dengan id="intro".
Perbedaannya ada pada cakupan dan spesifisitas selector.

---

**3. Jika ada internal, eksternal, dan inline CSS pada elemen yang sama, mana yang ditampilkan?**

Jawaban:
Urutan prioritas CSS:

Inline CSS → paling tinggi
Internal CSS
External CSS → paling rendah

Contoh:
<p style="color:red;">Teks ini merah (inline menang)</p>

---

**4. Pada elemen terdapat ID dan Class, jika keduanya ada CSS, mana yang dipakai?

Jawaban:
Selector ID lebih kuat daripada Class. Jadi jika ada konflik, aturan ID akan menang.

Contoh:
CSS
.text-paragraf { color: green; }
#paragraf-1 { color: orange; }

HTML
<p id="paragraf-1" class="text-paragraf">Teks ini tampil oranye</p>

---

5. Apa fungsi validasi CSS dengan W3C Validator?

Jawaban:
Validasi CSS digunakan untuk memastikan kode CSS sesuai standar internasional (W3C).
Manfaatnya:

- Menghindari error sintaks.
- Membuat tampilan konsisten di berbagai browser.
- Membuktikan kode sudah sesuai best practice.
- Hasil validasi pada file style_eksternal.css adalah No Error Found ✅.


---

##Kesimpulan

- Berhasil membuat CSS dengan 3 metode: Inline, Internal, dan Eksternal.
- Paham perbedaan penggunaan selector (Element, Class, ID).
- Mengetahui urutan prioritas CSS (Cascade).
- Kode CSS tervalidasi di W3C tanpa error.
