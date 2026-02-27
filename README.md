# k2ab.copyprinting
percetakan dan potocopy
<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Percetakan & Fotocopy Cepat</title>

<style>
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background: #f4f4f4;
}

header {
    background: #0077cc;
    color: white;
    padding: 20px;
    text-align: center;
}

nav {
    background: #005fa3;
    text-align: center;
    padding: 10px;
}

nav a {
    color: white;
    text-decoration: none;
    margin: 15px;
    font-weight: bold;
}

section {
    padding: 40px;
    background: white;
    margin: 20px;
    border-radius: 8px;
}

h2 {
    color: #0077cc;
}

.services {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 20px;
}

.service-box {
    background: #f0f8ff;
    padding: 20px;
    border-radius: 8px;
    text-align: center;
}

button {
    background: #0077cc;
    color: white;
    padding: 10px 20px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
}

button:hover {
    background: #005fa3;
}

footer {
    background: #0077cc;
    color: white;
    text-align: center;
    padding: 15px;
}

input, select {
    width: 100%;
    padding: 10px;
    margin: 10px 0;
}
</style>
</head>

<body>

<header>
    <h1>Percetakan & Fotocopy Cepat</h1>
    <p>Cetak cepat, harga hemat, kualitas mantap!</p>
</header>

<nav>
    <a href="#layanan">Layanan</a>
    <a href="#order">Order Online</a>
    <a href="#kontak">Kontak</a>
</nav>

<section id="layanan">
    <h2>Layanan Kami</h2>
    <div class="services">
        <div class="service-box">
            <h3>Print Hitam Putih</h3>
            <p>Mulai 500 / lembar</p>
        </div>
        <div class="service-box">
            <h3>Print Warna</h3>
            <p>Mulai 2.000 / lembar</p>
        </div>
        <div class="service-box">
            <h3>Fotocopy</h3>
            <p>Mulai 300 / lembar</p>
        </div>
        <div class="service-box">
            <h3>Jilid & Laminating</h3>
            <p>Rapi & Profesional</p>
        </div>
    </div>
</section>

<section id="order">
    <h2>Order Online</h2>
    <form onsubmit="kirimWhatsApp(); return false;">
        <input type="text" id="nama" placeholder="Nama Anda" required>
        
        <select id="layananSelect">
            <option value="Print Hitam Putih">Print Hitam Putih</option>
            <option value="Print Warna">Print Warna</option>
            <option value="Fotocopy">Fotocopy</option>
            <option value="Jilid / Laminating">Jilid / Laminating</option>
        </select>

        <input type="number" id="jumlah" placeholder="Jumlah Lembar" required>

        <button type="submit">Kirim ke WhatsApp</button>
    </form>
</section>

<section id="kontak">
    <h2>Kontak Kami</h2>
    <p>📍 Alamat: Jl. Contoh No.123</p>
    <p>📞 WhatsApp: 081234567890</p>
    <p>🕒 Jam Buka: 08.00 - 21.00</p>
</section>

<footer>
    <p>© 2026 Percetakan & Fotocopy Cepat</p>
</footer>

<script>
function kirimWhatsApp() {
    var nama = document.getElementById("nama").value;
    var layanan = document.getElementById("layananSelect").value;
    var jumlah = document.getElementById("jumlah").value;

    var nomor = "6281234567890"; // Ganti dengan nomor WhatsApp Anda
    var pesan = `Halo, saya ${nama} ingin order ${layanan} sebanyak ${jumlah} lembar.`;

    var url = "https://wa.me/" + nomor + "?text=" + encodeURIComponent(pesan);
    window.open(url, "_blank");
}
</script>

</body>
</html>
