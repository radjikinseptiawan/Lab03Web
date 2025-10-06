# Praktikum: Membuat Form dengan Listbox (Multiple Selection)

## 📘 Tujuan
Membuat sebuah form HTML yang menampilkan **listbox** dengan fitur **multiple selection**, sehingga pengguna dapat memilih **lebih dari satu hobi** sekaligus.

---

## 🧩 Langkah-langkah Praktikum

### 1️⃣ Membuat Struktur Dasar HTML
Pertama, buat file baru bernama **`index.html`** dan tuliskan struktur dasar HTML seperti berikut:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <!-- Form akan ditulis di sini -->
</body>
</html>
````

📖 **Penjelasan:**

* `<!DOCTYPE html>` : Menentukan bahwa dokumen ini adalah file HTML5.
* `<html lang="en">` : Menandakan bahwa bahasa halaman ini adalah bahasa Inggris.
* `<meta charset="UTF-8">` : Mengatur encoding karakter agar mendukung huruf dan simbol internasional.
* `<meta name="viewport" ...>` : Membuat tampilan halaman menyesuaikan dengan layar perangkat (responsif).
* `<title>` : Judul halaman yang akan muncul di tab browser.

---

### 2️⃣ Menambahkan Elemen Form

Di dalam `<body>`, buat elemen `<form>` untuk menampung input pengguna.

```html
<form action="">
    <!-- Isi form -->
</form>
```

📖 **Penjelasan:**

* Tag `<form>` digunakan untuk membuat formulir yang bisa berisi input teks, tombol, dan pilihan.
* Atribut `action` bisa diisi dengan URL tujuan pengiriman data. Di sini dikosongkan (`""`) karena tidak mengirim ke server.

---

### 3️⃣ Menambahkan Label dan Listbox

Tambahkan label dan elemen `<select>` yang berfungsi sebagai **listbox** dengan kemampuan **multiple selection**.

```html
<label for="hobi">Hobi</label>
<select name="skills[]" id="hobi" multiple>
    <option value="">Mancing</option>
    <option value="">Game</option>
    <option value="">Ngoding</option>
    <option value="">Gambar</option>
</select>
```

📖 **Penjelasan:**

* `<label for="hobi">` : Label teks untuk menunjukkan input yang dimaksud, dihubungkan dengan elemen `id="hobi"`.
* `<select>` : Elemen yang membuat daftar pilihan (listbox atau dropdown).
* `multiple` : Atribut penting yang membuat pengguna bisa memilih **lebih dari satu opsi** (multiple selection).
* `name="skills[]"` : Nama variabel yang akan dikirim ke server. Tanda `[]` menandakan bahwa data ini bisa berisi **lebih dari satu nilai**.
* `<option>` : Menentukan item-item yang bisa dipilih (contohnya: Mancing, Game, Ngoding, Gambar).

📸 **Tampilan di browser:**
*(Masukkan screenshot kamu di sini)*
![Screenshot Listbox](screenshot_form.png)

---

### 4️⃣ Menambahkan Tombol

Tambahkan tombol di bawah listbox agar pengguna dapat mengirim pilihan.

```html
<button>Pilih</button>
```

📖 **Penjelasan:**

* Tag `<button>` digunakan untuk membuat tombol.
* Saat diklik, tombol ini akan mengirimkan data form (meskipun di contoh ini belum terhubung ke server).

---

### 5️⃣ Hasil Akhir Kode Lengkap

Berikut isi lengkap file **`index.html`** setelah semua langkah dilakukan:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <form action="">
        <label for="hobi">Hobi</label>
        <select name="skills[]" id="hobi" multiple>
            <option value="">Mancing</option>
            <option value="">Game</option>
            <option value="">Ngoding</option>
            <option value="">Gambar</option>
       </select>
       <button>Pilih</button>
    </form>
</body>
</html>
```

📸 **Screenshot hasil tampilan (contoh):**
*(Tambahkan gambar hasil tampilannya di browser)*

![Hasil Akhir Form Listbox](screenshot_result.png)

---

## 📑 Kesimpulan

* Elemen `<select>` digunakan untuk membuat daftar pilihan (listbox atau dropdown).
* Atribut `multiple` memungkinkan pengguna memilih **lebih dari satu pilihan**.
* Elemen `<option>` digunakan untuk menuliskan isi daftar.
* Form ini bisa digunakan untuk mengirim data berupa **beberapa nilai sekaligus**, misalnya daftar hobi yang dipilih.

---

✍️ **Nama:** Radjikin Septiawan
🧠 **Mata Kuliah:** Pemrograman Web1

```