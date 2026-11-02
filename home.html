<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <title>Toko Snack Basah & Kering</title>
    <style>
        /* CSS Sederhana buat ngatur Header & Background Headline */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: gold;
        }
        
        .header-nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            background-color: #333;
            color: white;
            padding: 10px 20px;
        }
        .header-nav nav a {

            color: white;
            text-decoration: none;
            margin-left: 15px;
        }
        /* Bagian Headline dengan Background Gambar */
        .headline-section {
            background-image: url('img/drawing.png'); /* Ganti nama file gambarmu */
            background-size: cover;
            background-position: center;
            height: 300px;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            color: white;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.7);
        }
    </style>

</head>
<body>
    
    <!-- 1. BAGIAN ATAS: Logo & Menu (Sesuai Sketsa) -->
    <div class="header-nav">
        <div class="logo">
            <strong>Jerry's Snack</strong>
        </div>
        <nav>
            <a href="index.php">Home</a>
            <a href="product.php">Product</a>
        </nav>
    </div>

    <!-- 2. BAGIAN HEADLINE DENGAN BACKGROUND (Sesuai Sketsa) -->
    <div class="headline-section">

        <h1>Selamat Datang!</h1>
        <p>Rasa Pasti Joss, Harga Pasti Pas!</p>
    </div>

    <div class="content-section" style="background-color: white; padding: 40px; display: flex; justify-content: center; align-items: flex-start;">
        <div style="width: 45%;">
            <h3 style="color: #333; border-bottom: 2px solid #ff7b00; padding-bottom: 5px;">Tentang Kami</h3>
            <p>Jerry's Snack adalah toko yang menjual berbagai macam jajanan basah, kering, ataupun frozen dengan harga yang terjangkau tapi dengan rasa yang joss.</p>
        </div>
    </div>
    <div style="background-color: white; padding: 40px; display: flex; justify-content: space-between; align-items: flex-start; border-top: 2px solid #ddd;">
        <div style="width: 48%; background: #fff; padding: 20px; box-shadow: 0px 0px 10px rgba(0,0,0,0.05); display: flex; flex-direction: column; justify-content: space-between;">
            <h3 style="color: #333; border-bottom: 2px solid #ff7b00; padding-bottom: 5px;">Contact</h3>
            <p><strong>Whatsapp:</strong> <a href="https://wa.me/62882008499248" target="_blank">+62882008499248</a></p>
            <p><strong>Instagram:</strong> <a href="https://www.instagram.com/jerico_sanjaya608?exln=MXJtOWJhNDN0ODh6cQ== " target="_blank">Jerry's Snack</a></p>
            <p><strong>Facebook:</strong> <a href="https://www.facebook.com/share/1FUuTN6S9s/" target="_blank">Jerry's Snack</a></p>
            <p><strong>Twitter:</strong> <a href="https://x.com/Jerico_Sanjaya">Jerry's Snack</a></p>
        </div>
        <div style="width: 48%; background: #fff; padding: 20px; box-shadow: 0px 0px 10px rgba(0,0,0,0.05); display: flex; flex-direction: column; justify-content: space-between;" >
            <h3 style="color: #333; border-bottom: 2px solid #ff7b00; padding-bottom: 5px;">Lokasi</h3>
            <iframe src="https://maps.app.goo.gl/Sjik9KK2uyjGAREG9" 
            frameborder="0"
            width="100%"
            height="200"
            style="border: 0;"
            loading="lazy">
            ></iframe>
        </div>
    </div>

    <!-- BAGIAN PHP: Menampilkan Data Produk dari Database -->
    <div style="background-color: #fff; padding: 40px; text-align: center;">
        <h3 style="color: #333; border-bottom: 2px solid #ff7b00; padding-bottom: 5px; display: inline-block;">Daftar Produk</h3>
        
        <div style="display: flex; justify-content: center; gap: 20px; margin-top: 20px; flex-wrap: wrap;">
            <?php
                // 1. Panggil file koneksi
                include 'Connection.php';

                // 2. Ambil data dari tabel snack di database
                $query = mysqli_query($koneksi, "SELECT * FROM snack LIMIT 2");

                // 3. Perulangan (looping) untuk mencetak data produk ke layar
                while($row = mysqli_fetch_assoc($query)){
            ?>
                <!-- Kotak Kartu Produk -->
                <div style="border: 1px solid #ddd; padding: 15px; width: 200px; border-radius: 8px; background: #fff; box-shadow: 0px 2px 5px rgba(0,0,0,0.1);">
                    <h4 style="margin: 10px 0; color: #333;"><?php echo $row['nama_snack']; ?></h4>
                    <img src="img/<?php echo $row['gambar']; ?>" alt="<?php echo $row['nama_snack']; ?>" style="width: 100%; height: 120px; object-fit: cover; border-radius: 6px;">
                    <p style="color: #666; font-size: 14px;">Harga: Rp <?php echo number_format($row['harga'], 0, ',', '.'); ?></p>
                    <span style="background: #ff7b00; color: white; padding: 5px 10px; font-size: 12px; border-radius: 4px; display: inline-block;">Stok: <?php echo $row['stok']; ?></span>

                    <a href="cart.php?id=<?php echo $row['id_snack']; ?>" 
                        style="background: #007bff; color: white; padding: 6px 10px; text-decoration: none; border-radius: 4px; font-size: 12px; font-weight: bold;">
                        + Keranjang
                    </a>
                </div>
            <?php 
                } // Penutup perulangan while
            ?>
        </div>
    </div>
</body>
</html>
