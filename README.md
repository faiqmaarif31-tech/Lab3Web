# PRAKTIKUM 3 CSS DASAR

## Identitas

**Nama:** [Faiq Rayyan Ma'arif]
**NIM:** [312510062]
**Kelas:** TI25 A1
**Mata Kuliah:** Pemrograman Web
**Universitas:** Universitas Pelita Bangsa

---

## Tujuan Praktikum

Praktikum ini bertujuan untuk:

1. Memahami konsep dasar CSS.
2. Memahami aturan penulisan pada CSS.
3. Memahami selector sebagai pengontrol CSS.
4. Membuat pengaturan CSS pada HTML.

---

## Langkah-Langkah Praktikum

### 1. Membuat Dokumen HTML

Pertama, membuat file HTML dengan nama:

`lab2_css_dasar.html`

Kemudian membuat struktur dasar dokumen HTML yang terdiri dari `header`, `nav`, heading, paragraf, dan link.

![Screenshot HTML Dasar](screenshots/01-html-dasar.png)

---

### 2. Mendeklarasikan CSS Internal

Selanjutnya menambahkan CSS Internal pada bagian `<head>` menggunakan tag `<style>`.

CSS Internal digunakan untuk mengatur font, header, border, ukuran heading, warna heading, posisi teks, dan warna teks pada bagian tertentu.

![Screenshot CSS Internal](screenshots/02-css-internal.png)

---

### 3. Menambahkan Inline CSS

Selanjutnya menambahkan Inline CSS secara langsung pada elemen HTML menggunakan atribut `style`.

Inline CSS digunakan untuk memberikan pengaturan CSS secara langsung pada elemen tertentu.

![Screenshot Inline CSS](screenshots/03-inline-css.png)

---

### 4. Membuat CSS Eksternal

Selanjutnya membuat file CSS baru dengan nama:

`style_eksternal.css`

File CSS tersebut kemudian dihubungkan dengan dokumen HTML menggunakan tag `<link>` pada bagian `<head>`.

![Screenshot CSS Eksternal](screenshots/04-css-eksternal.png)

---

### 5. Menambahkan CSS Selector

Pada tahap ini menambahkan CSS Selector menggunakan **ID Selector** dan **Class Selector**.

ID Selector digunakan pada elemen dengan atribut `id`, sedangkan Class Selector digunakan pada elemen dengan atribut `class`.

Contoh ID Selector:

```css
#intro {
    background: #418fb1;
    border: 1px solid #099249;
    min-height: 100px;
    padding: 10px;
}
```

Contoh Class Selector:

```css
.button {
    padding: 15px 20px;
    background: #bebcbd;
    color: #fff;
    display: inline-block;
    margin: 10px;
    text-decoration: none;
}
```

![Screenshot CSS Selector](screenshots/05-css-selector.png)

---

## Pertanyaan dan Tugas

### 1. Eksperimen CSS

Melakukan eksperimen dengan mengubah dan menambahkan properti serta nilai pada kode CSS dengan mengacu pada CSS Cheat Sheet.

Beberapa properti yang dapat digunakan antara lain:

* `color`
* `background`
* `font-size`
* `font-family`
* `text-align`
* `padding`
* `margin`
* `border`

---

### 2. Perbedaan `h1 {...}` dengan `#intro h1 {...}`

`h1 {...}` merupakan selector yang digunakan untuk memberikan aturan CSS pada elemen `<h1>`.

Sedangkan `#intro h1 {...}` merupakan selector yang lebih spesifik karena aturan CSS diterapkan pada elemen `<h1>` yang berada di dalam elemen dengan ID `intro`.

Contoh:

```css
h1 {
    color: red;
}

#intro h1 {
    color: white;
}
```

Pada contoh tersebut, `<h1>` yang berada di dalam `#intro` akan mengikuti aturan `#intro h1`.

---

### 3. CSS Internal, Eksternal, dan Inline

Jika terdapat CSS Internal, CSS Eksternal, dan Inline CSS yang diterapkan pada elemen yang sama, deklarasi yang memiliki prioritas atau specificity lebih tinggi akan digunakan oleh browser.

Contoh:

```html
<p style="color: red;">
    Contoh paragraf
</p>
```

CSS Inline pada contoh tersebut memberikan warna merah secara langsung pada elemen `<p>`.

---

### 4. ID Selector dan Class Selector

Jika sebuah elemen memiliki ID dan Class, kemudian ked
