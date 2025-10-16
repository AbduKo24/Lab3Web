# Lab3Web
```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title> HTML Lanjutan</title>
    </head>
    <body>
        <header>
            <h1>
                Membuat List
            </h1>
            <section id="order-list">
                <h2>
                    order-list
                </h2>
                <ol>
                    <li>Pemrograman web</li>
                    <li>Sistem Informasi</li>
                    <li>Basis Data</li>
                </ol>
            </section>
            <section id="unorder-list"> 
                <h2>unorder-list</h2>
                <ul type="square">
                    <li>Jaringan Komputer</li>
                    <li>Struktur Data</li>
                    <li>Algoritma &amp; Pemrograman</li>
                </ul>
            </section>
            <section id="unorder-list">
                <h2>Description List</h2>
                <dl>
                    <dt>Fakultas Teknik</dt>
                    <dd>Teknik Industri</dd>
                    <dd>Teknik Informatika</dd>
                    <dd>Teknik Lingkungan</dd>\
                    <dt>fakultas Ekonomi dan Bisnis</dt>
                    <dd>Akuntasi</dd>
                    <dd>Manajemen</dd>
                    <dd>Bisnis Digital</dd>
                </dl>
            </section>
        </header>
    </body>
</html>


```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title> HTML Lanjutan </title>
    </head>
    <body>
        <header>
            <h1>Membuat Table</h1>
        </header>
        <table border="1" cellpadding="4" cellspacing="0">
            <thead>
                <tr>
                    <th>NO.</th>
                    <th>Fakultas</th>
                    <th>Pemrogram Studi</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>1.</td>
                    <td rowspan="3">Teknik</td>
                    <td>Teknik Informatika</td>
                </tr>
                <tr>
                    <td>2.</td>
                    <td>Teknik Industri</td>
                </tr>
                <tr>
                    <td>3.</td>
                    <td>Teknik Lingkungan</td>
                </tr>
            </tbody>
        </table>
    </body>
</html>


```html
<!DOCTYPE html> 
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Lanjutan</title>
</head>
<body>
    <header>
        <h1>Membuat From</h1>
    </header>
    <form action="proses.php" method="post">
        <fieldset>
            <legend>Data Pelanggan</legend>
            <p>
                <label for="nama">Nama</label>
                <input type="text" id="nama" name="nama">
            </p>
            <p>
                <label for="alamat">Alamat</label>
                <textarea  id="alamat" name="alamat" cols="20" rows="3"></textarea>
            </p>
            <p>
                <label>Jenis Kelamin</label>
                <input id="jk_l" type="radio" name="kelamin" value="L">
                <label for="jk_l">Laki-laki</label>
                <input id="jk_p" type="radio" name="kelamin" value="P">
                <label for="jk_p">Perempuan</label>
            </p>
            <p>
                <input type="submit" value="login">
            </p>
        </fieldset>
    </form>
    <style>
       form p > label {
            display: inline-block;
            width: 100px;
        }
        form input[type="text"], form textarea {
            border: 1px solid #197a43;
        }
        form input[type="submit"] {
            border: 1px solid #197a43;
            background-color: #197a43;
            color: #ffffff;
            font-weight: bold;
            padding: 5px 15px;
        }
    </style>
</body>
</html>


```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Form Pendaftaran</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 20px;
        }
        form p > label {
            display: inline-block;
            width: 120px;
        }
        form input[type="text"], form textarea, select {
            border: 1px solid #197a43;
            padding: 5px;
        }
        form input[type="submit"] {
            border: 1px solid #197a43;
            background-color: #197a43;
            color: #ffffff;
            font-weight: bold;
            padding: 5px 15px;
            cursor: pointer;
        }
        form input[type="submit"]:hover {
            background-color: #145a32;
        }
    </style>
</head>
<body>
    <header>
        <h1>Form Pendaftaran</h1>
    </header>

    <form action="proses.php" method="post">
        <fieldset>
            <legend>Data Mahasiswa</legend>
            
            <!-- Input Nama -->
            <p>
                <label for="nama">Nama</label>
                <input type="text" id="nama" name="nama" required>
            </p>

            <!-- Dropdown (Select) -->
            <p>
                <label for="jurusan">Jurusan</label>
                <select id="jurusan" name="jurusan">
                    <option value="">-- Pilih Jurusan --</option>
                    <option value="ar">Arsitektur</option>
                    <option value="ts">Teknik Sipil</option>
                    <option value="ie">Teknik Industri</option>
                    <option value="ti">Teknik Informatika</option>
                    <option value="tl">Teknik Lingkungan</option>
                    <option value="tp">Teknologi Hasil Pertanian</option>
                    <option value="mm">Manajemen</option>
                    <option value="bd">Bisnis Digital</option>
                    <option value="kn">Kewirausahaan</option>
                    <option value="es">Ekonomi Syariah</option>
                    <option value="ai">Akutansi</option>
                    <option value="pgsd">Pendidikan Guru Sekolah Dasar</option>
                    <option value="pgpaud">Pendidikan Guru Pendidikan Anak Usia Dini</option>
                    <option value="bkpi">Bimbingan Dan Konseling Pendidikan Islam</option>
                    <option value="hm">Hukum</option>
                </select>
            </p>

            <!-- Listbox Multiple Selection -->
            <p>
                <label for="hobi">Hobi</label>
                <select id="hobi" name="hobi[]" multiple size="4">
                    <option value="Mancing">Mancing</option>
                    <option value="olahraga">Olahraga</option>
                    <option value="Game">Game</option>
                    <option value="Gaming">Gaming</option>
                </select>
            </p>

            <!-- Tombol Submit -->
            <p>
                <input type="submit" value="Kirim Data">
            </p>
        </fieldset>
    </form>
</body>
</html>
