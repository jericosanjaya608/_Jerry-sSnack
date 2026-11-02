<?php
session_start();
include 'Connection.php';

    // Tangkap aksi kosongkan keranjang di sini (paling atas sebelum ada HTML)
        if (isset($_GET['aksi']) && $_GET['aksi'] == 'kosongkan') {
             unset($_SESSION['cart']);
             header("Location: cart.php");
             exit;
        }
    // Tangkap aksi tambah atau kurang jumlah item di keranjang
    if (isset($_GET['aksi']) && isset($_GET['id'])) {
        $id_snack = $_GET['id'];
        
        if ($_GET['aksi'] == 'tambah') {
            // Tambah jumlah stok di session cart
            if (isset($_SESSION['cart'][$id_snack])) {
                $_SESSION['cart'][$id_snack] += 1;
            }
        } elseif ($_GET['aksi'] == 'kurang') {
            // Kurangi jumlah, jika sisa 1 lalu dikurangi maka hapus item dari keranjang
            if (isset($_SESSION['cart'][$id_snack])) {
                $_SESSION['cart'][$id_snack] -= 1;
                if ($_SESSION['cart'][$id_snack] <= 0) {
                    unset($_SESSION['cart'][$id_snack]);
                }
            }
        }
    
    // Refresh halaman cart agar total harga langsung ter-update otomatis
    header("Location: cart.php");
    exit;
}   

// Jika tombol keranjang diklik dan membawa parameter ID produk
if (isset($_GET['id'])) {
    $id_snack = $_GET['id'];
    
    // Jika produk sudah ada di keranjang, tambahkan jumlahnya (+1)
    if (isset($_SESSION['cart'][$id_snack])) {
        $_SESSION['cart'][$id_snack] += 1;
    } else {
        // Jika belum ada, masukkan sebagai item baru dengan jumlah 1
        $_SESSION['cart'][$id_snack] = 1;
    }
    
    // Redirect agar URL bersih kembali
    header("Location: cart.php");
    exit();
}
?>
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <title>Keranjang Belanja - Jerry's Snack</title>
</head>
<body style="font-family: Arial, sans-serif; background-color: #f4f4f4; padding: 30px; text-align: center;">

    <div style="background: #fff; padding: 25px; border-radius: 8px; max-width: 650px; margin: 0 auto; box-shadow: 0px 2px 5px rgba(0,0,0,0.1);">
        <h2 style="color: #333; margin-bottom: 10px;">Keranjang Belanja Jerry's Snack</h2>
        <hr style="border: 0; border-top: 2px solid #ff7b00; margin-bottom: 20px;">

        <?php if (!empty($_SESSION['cart'])): ?>
            <table style="width: 100%; border-collapse: collapse; margin-bottom: 20px;">
                <thead>
                    <tr style="background: #ff7b00; color: white;">
                        <th style="padding: 10px; border: 1px solid #ddd;">Nama Produk</th>
                        <th style="padding: 10px; border: 1px solid #ddd;">Harga</th>
                        <th style="padding: 10px; border: 1px solid #ddd;">Jumlah</th>
                        <th style="padding: 10px; border: 1px solid #ddd;">Subtotal</th>
                    </tr>
                </thead>
                <tbody>
                    <?php 
                    $total_semua = 0;
                    foreach ($_SESSION['cart'] as $id_snack => $jumlah):
                        // Ambil data produk dari database berdasarkan ID snack
                        $result = mysqli_query($koneksi, "SELECT * FROM snack WHERE id_snack = '$id_snack'");
                        if ($row = mysqli_fetch_assoc($result)):
                            $subtotal = $row['harga'] * $jumlah;
                            $total_semua += $subtotal;
                    ?>
                    <tr>
                        <td style="padding: 10px; border: 1px solid #ddd; text-align: left;"><?php echo $row['nama_snack']; ?></td>
                        <td style="padding: 10px; border: 1px solid #ddd;">Rp <?php echo number_format($row['harga'], 0, ',', '.'); ?></td>
                        <td style="padding: 10px; border: 1px solid #ddd;"><?php echo $jumlah; ?></td>
                        <td style="padding: 10px; border: 1px solid #ddd;">Rp <?php echo number_format($subtotal, 0, ',', '.'); ?></td>

                        <td style="text-align: center; vertical-align: middle; padding: 10px; border: 1px solid #ddd;">
                            <a href="cart.php?aksi=kurang&id=<?php echo $id_snack; ?>" style="text-decoration: none; padding: 3px 10px; background: #dc3545; color: white; border-radius: 3px; font-weight: bold; margin-right: 5px;">-</a>
                            
                            <a href="cart.php?aksi=tambah&id=<?php echo $id_snack; ?>" style="text-decoration: none; padding: 3px 10px; background: #28a745; color: white; border-radius: 3px; font-weight: bold; margin-left: 5px;">+</a>
                        </td>
                    </tr>
                    <?php 
                        endif;
                    endforeach; 
                    ?>
                    <!-- Di dalam loop tabel keranjang cart.php -->
                   
                </tbody>
            </table>

            <!-- Bagian Tabel Keranjang yang sudah ada -->
        <!-- ... -->
        
        <!-- Total Tagihan -->
        <div style="text-align: right; margin-top: 15px; font-weight: bold; font-size: 16px;">
            Total Tagihan: Rp <?php echo number_format($total_semua, 0, ',', '.'); ?>
        </div>

        <!-- FORM INPUT DATA PENGIRIMAN & CHECKOUT DISINI -->
        <form action="checkout.php" method="POST" style="margin-top: 25px; border-top: 2px dashed #ddd; padding-top: 20px;">
            <h3 style="margin-bottom: 15px; color: #333;">Informasi Pengiriman & Pembayaran</h3>
            
            <div style="margin-bottom: 12px;">
                <label style="display: block; font-weight: bold; margin-bottom: 5px; font-size: 14px;">Nama Penerima:</label>
                <input type="text" name="nama_penerima" required placeholder="Masukkan nama lengkap..." style="width: 100%; padding: 8px; box-sizing: border-box; border: 1px solid #ccc; border-radius: 4px;">
            </div>

            <div style="margin-bottom: 12px;">
                <label style="display: block; font-weight: bold; margin-bottom: 5px; font-size: 14px;">No. Telepon / WhatsApp:</label>
                <input type="text" name="no_telepon" required placeholder="Contoh: 08123456789" style="width: 100%; padding: 8px; box-sizing: border-box; border: 1px solid #ccc; border-radius: 4px;">
            </div>

            <div style="margin-bottom: 12px;">
                <label style="display: block; font-weight: bold; margin-bottom: 5px; font-size: 14px;">Alamat Lengkap:</label>
                <textarea name="alamat" rows="2" required placeholder="Masukkan alamat tujuan pengiriman..." style="width: 100%; padding: 8px; box-sizing: border-box; border: 1px solid #ccc; border-radius: 4px;"></textarea>
            </div>

            <div style="margin-bottom: 20px;">
                <label style="display: block; font-weight: bold; margin-bottom: 5px; font-size: 14px;">Metode Pembayaran:</label>
                <select name="metode_pembayaran" required style="width: 100%; padding: 8px; box-sizing: border-box; border: 1px solid #ccc; border-radius: 4px;">
                    <option value="">-- Pilih Metode Pembayaran --</option>
                    <option value="Transfer Bank">Transfer Bank</option>
                    <option value="COD">COD (Bayar di Tempat)</option>
                    <option value="QRIS">QRIS / E-Wallet</option>
                </select>
            </div>

            <!-- Tombol Aksi di Bawah Form -->
            <div style="display: flex; justify-content: space-between; align-items: center;">
                <a href="home.php" style="background: #6c757d; color: white; padding: 8px 15px; text-decoration: none; border-radius: 4px; font-size: 14px; font-weight: bold;">&larr; Lanjut Belanja</a>
                
                <div>
                    <a href="cart.php?aksi=kosongkan" onclick="return confirm('Yakin ingin mengosongkan keranjang?')" style="background: #dc3545; color: white; padding: 8px 15px; text-decoration: none; border-radius: 4px; font-size: 14px; font-weight: bold; margin-right: 10px;">Kosongkan Keranjang</a>

                    <button type="submit" name="proses_pesanan" style="background: #28a745; color: white; padding: 9px 18px; border: none; border-radius: 4px; font-weight: bold; font-size: 14px; cursor: pointer;">
                        Proses Checkout Sekarang
                    </button>
                </div>
            </div>
        </form>

        <?php else: ?>
            <p style="color: #666; font-style: italic; margin: 30px 0;">Keranjang belanja kamu masih kosong nih.</p>
            <a href="home.php" style="background: #ff7b00; color: white; padding: 10px 20px; text-decoration: none; border-radius: 4px; font-weight: bold;">Kembali ke Beranda</a>
        <?php endif; ?>

        
    </div>

</body>
</html>