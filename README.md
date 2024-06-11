<!DOCTYPE html>

<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>centrallibrary</title>
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.2/dist/css/bootstrap.min.css" integrity="sha384-ZenhVNpHmPQ0oW9R7ls9dQoEOzEt0tUlKFqwTGTYBjH1lVA++cvTTA/SxbCwmzOe" crossorigin="anonymous">
  <link rel="stylesheet" href="style.css">
  <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.6.3/jquery.min.js"></script>
  <script src="script.js"></script>

</head>
<script>
  console. log ( "Hello, Terima kasih Telah Mengunjungi Website") ;
</script> 
   
<script>
  document.write("<h3> Hello, Terima Kasih Telah Mengunjungi Website Ini</h3>");
</script>
<th><h2 style="color:rgb(105, 104, 104)"> Berikut ini contoh website perpustakaan yang dibuat untuk memenuhi tugas pada mata kuliah Pemrograman Web Praktik Program Studi S-1 Ilmu Perpustakaan, Universitas Sumatera Utara.</h2></th>

  <header>
    <h1>Central Library</h1>
  </header>



<style>
  .menu {
    list-style-type: none;
    padding: 10px; /* Tambahkan padding untuk memperindah tampilan */
    margin: 0;
    background-color: #e6e4e4; /* Warna latar belakang putih */
    border-radius: 7px; /* Tambahkan border radius untuk sudut kotak yang lebih halus */
    box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1); /* Tambahkan bayangan untuk efek kedalaman */
  }

  .menu li {
    display: inline;
  }

  .menu li a {
    text-decoration: none;
    color: rgb(10, 10, 10); /* Sesuaikan warna teks */
  }

  .menu li span {
    margin-left: 5px; /* Sesuaikan jarak antara tautan dan teks */
    margin-right: 5px; /* Sesuaikan jarak antara teks dan tautan berikutnya */
  }
</style>


<ul class="menu">
  <li><a href="modul 1.html">Beranda Library</a><span>   </span></li>
  <li><a href="Modul 2.1.html">Form Anggota</a><span>    </span></li>
  <li><a href="Modul 2.2.html">Form Pemesanan & Peminjaman</a><span>   </span></li>
  <li><a href="Modul 3.2.html">HTML & CSS</a><span>    </span></li>
  <li><a href="Modul 4.html">Tabel & Form</a><span>    </span></li>
  <li><a href="Modul 5.2.2.html">JavaScript</a><span>    </span></li>
  <li><a href="Modul 5.3.html">Koleksi</a><span>    </span></li> 
  <li><a href="Modul 6.html">jquery</a><span>    </span></li> 
  <li><a href="Modul 7.1.html">PHP</a><span>    </span></li> 
  <li><a href="Modul 8.html">Database</a><span>    </span></li> 
  <li><a href="Modul kontak.6 .html">About Us</a></li>
</ul>



  <div class="content"></div>
  <img src="https://www.nusabali.com/article_images/35867/badung-tambah-koleksi-buku-perpustakaan-sd-senila-800-2018-08-13-105154_0.jpg" style="width:1340px;height:300px;" align="middle">
</div>

  


    <section id="categories">
      <h2>Kategori</h2>
      <ul>
        <li><a href="Modul 5.3.html">Fiksi </a></li>
        <li><a href="Modul 5.3.html">Non Fiksi</a></li>
        

      </ul>
    </section>

    <main>
        <section id="featured">
          <h2> Koleksi Terbaru</h2>
          <title></title>
<style>
  body {
    font-family: Arial, sans-serif;
    margin: 20px;
  }
  h1 {
    text-align: center;
  }
  #searchInput {
    width: 30%;
    padding: 8px;
    margin-bottom: 20px;
    box-sizing: border-box;
  }
  table {
    width: 100%;
    border-collapse: collapse;
  }
  th, td {
    border: 1px solid #dddddd;
    padding: 8px;
    text-align: left;
  }
  th {
    background-color: #f2f2f2;
  }
</style>
</head>
<body>

<input type="text" id="searchInput"placeholder="Search by title...">
<div id="bookTable"></div>
<script>
  // Contoh data buku
  var books = [
    { title: "The Hunger Games ", author: "Suzanne Collins", genre: "Fiksi", year: 2008},
    { title: "The Great Gatsby", author: "F. Scott Fitzgerald", genre: "Fiksi", year: 1925 },
    { title: "Harry Potter ", author: "J.K Rowling ", genre: " Fiksi", year: 1997 },
    { title: "Sejarah Dunia Yang Disembunyikan ", author: "Jonathan Black ", genre: " Non Fiksi", year: 2007 },
    { title: "The Lean Startup", author: "Eric Ries", genre: "Non Fiksi", year: 2011 },
    ];

  // Fungsi untuk menampilkan tabel buku
  function displayBooks(searchTerm) {
    var table = "<table><tr><th>Title</th><th>Author</th><th>Genre</th><th>Year</th></tr>";
    for (var i = 0; i < books.length; i++) {
      // Jika buku cocok dengan pencarian atau pencarian kosong, tampilkan
      if (books[i].title.toLowerCase().includes(searchTerm.toLowerCase()) || searchTerm === "") {
        table += "<tr>";
        table += "<td>" + books[i].title + "</td>";
        table += "<td>" + books[i].author + "</td>";
        table += "<td>" + books[i].genre + "</td>";
        table += "<td>" + books[i].year + "</td>";
        table += "</tr>";
      }
    }
    table += "</table>";
    document.getElementById("bookTable").innerHTML = table;
  }

  // Menangani event saat input pencarian berubah
  document.getElementById("searchInput").addEventListener("input", function() {
    displayBooks(this.value);
  });

  // Menampilkan tabel saat halaman dimuat
  displayBooks("");
</script>
</body>
</html>
          <div id="featured-carousel" class="carousel slide" data-bs-ride="carousel">
            <div class="carousel-inner">
              </div>
            <button class="carousel-control-prev" type="button" data-bs-target="#featured-carousel" data-bs-slide="prev">
              <span class="carousel-control-prev-icon" aria-hidden="true"></span>
              <span class="visually-hidden">Previous Slide</span>
            </button>
            <button class="carousel-control-next" type="button" data-bs-target="#featured-carousel" data-bs-slide="next">
              <span class="carousel-control-next-icon" aria-hidden="true"></span>
              <span class="visually-hidden">Next Slide</span>
            </button>
          </div>
        </section>
  </main>
  
</body>
</html>

