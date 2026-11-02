<?php
session_start();
include 'Connection.php';

if (isset($_POST['proses_pesanan']) && !empty($_SESSION['cart'])) {
    
    // 1. Ambil data dari form yang dikirim lewat cart.php
    $nama_penerima = mysqli_real_escape_string($koneksi, $_POST['nama_penerima']);
    $no_telepon    = mysqli_real_escape_string($koneksi, $_POST['no_telepon']);
    $alamat        = mysqli_real_escape_string($koneksi, $_POST['alamat']);
    
    // 2. Simpan data customer baru ke tabel 'customer'
    $query_customer = mysqli_query($koneksi, "INSERT INTO customer (nama_pelanggan, no_telepone, alamat_rumah) VALUES ('$nama_penerima', '$no_telepon', '$alamat')");
    
    if ($query_customer) {
        // Ambil ID customer yang baru saja masuk secara otomatis
        $id_pelanggan = mysqli_insert_id($koneksi);
        
        $tanggal_pesan = date('Y-m-d');
        $status_order  = 'Pending';
        
        // 3. Masukkan data ke tabel 'order' menggunakan ID customer yang baru
        $query_order = mysqli_query($koneksi, "INSERT INTO `order` (id_pelanggan, tanggal_pesan, status_order) VALUES ('$id_pelanggan', '$tanggal_pesan', '$status_order')");
        
        if ($query_order) {
            $id_pesanan_baru = mysqli_insert_id($koneksi);
            
            // 4. Masukkan setiap item keranjang ke tabel 'detail_order'
            foreach ($_SESSION['cart'] as $id_snack => $jumlah) {
                mysqli_query($koneksi, "INSERT INTO `detail_order` (id_pesanan, id_snack, jumlah_pembelian) VALUES ('$id_pesanan_baru', '$id_snack', '$jumlah')");
            }
            
            // 5. Kosongkan keranjang belanja
            unset($_SESSION['cart']);
            
            echo "<script>alert('Checkout Berhasil! Data pesanan dan pelanggan masuk ke Database.'); window.location='home.php';</script>";
        } else {
            echo "<script>alert('Gagal memproses pesanan!'); window.location='cart.php';</script>";
        }
    } else {
        echo "<script>alert('Gagal menyimpan data customer!'); window.location='cart.php';</script>";
    }
} else {
    header("Location: cart.php");
}
?>