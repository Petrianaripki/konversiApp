<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Aplikasi Konversi Satuan</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #f5f5f5;
        }

        header {
            background-color: #007BFF;
            color: white;
            padding: 10px;
        }

        main {
            margin: 20px auto;
            padding: 20px;
            background-color: white;
            max-width: 400px;  /* Lebih kecil agar lebih ringkas */
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }

        label, select, input {
            display: block;
            text-align: left;
            margin: 10px auto;
            width: 100%;  /* Menyempitkan input dan dropdown */
            max-width: 300px;  /* Membatasi lebar maksimal */
        }

        input, select {
            padding: 8px;
        }

        button {
            background-color: #007BFF;
            color: white;
            padding: 12px 20px;
            font-size: 16px;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            transition: background-color 0.3s ease;
            margin-top: 15px;
        }

        button:hover {
            background-color: #0056b3;
        }

        #hasil p {
            font-size: 18px;
            margin-top: 15px;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <header>
        <h1>Aplikasi Konversi Satuan</h1>
    </header>

    <main>
        <section>
            <label for="kategori">Pilih Jenis Konversi:</label>
            <select id="kategori" onchange="tampilkanInput()">
                <option value="panjang">Panjang</option>
                <option value="berat">Berat/Massa</option>
                <option value="suhu">Suhu</option>
                <option value="waktu">Waktu</option>
            </select>

            <div id="input-konversi"></div>  <!-- Tempat inputan dinamis -->
        </section>

        <section id="hasil">
            <label>Hasil Konversi:</label>
            <p id="output"></p>  <!-- Output konversi -->
        </section>
    </main>

    <script>
        document.addEventListener("DOMContentLoaded", function() {
            document.getElementById("kategori").value = "panjang";
            tampilkanInput();
        });

        function tampilkanInput() {
            const kategori = document.getElementById("kategori").value;
            const inputKonversi = document.getElementById("input-konversi");

            let html = `
                <label for="nilai">Masukkan Nilai:</label>
                <input type="number" id="nilai" placeholder="Nilai yang akan dikonversi">
                
                <label for="satuanAsal">Satuan Asal:</label>
                <select id="satuanAsal">
            `;

            let options = "";
            if (kategori === "panjang") {
                options = `
                    <option value="mm">Milimeter (mm)</option>
                    <option value="cm">Sentimeter (cm)</option>
                    <option value="m">Meter (m)</option>
                    <option value="km">Kilometer (km)</option>
                    <option value="in">Inci (inch)</option>
                    <option value="ft">Kaki (feet)</option>
                    <option value="yd">Yard (yard)</option>
                    <option value="mile">Mil (mile)</option>
                `;
            } else if (kategori === "berat") {
                options = `
                    <option value="mg">Miligram (mg)</option>
                    <option value="gram">Gram (g)</option>
                    <option value="kg">Kilogram (kg)</option>
                    <option value="ton">Ton (t)</option>
                    <option value="pon">Pon (lb)</option>
                    <option value="oz">Ons (oz)</option>
                `;
            } else if (kategori === "suhu") {
                options = `
                    <option value="c">Celcius (°C)</option>
                    <option value="f">Fahrenheit (°F)</option>
                    <option value="k">Kelvin (K)</option>
                    <option value="r">Reamur (°R)</option>
                `;
            } else if (kategori === "waktu") {
                options = `
                    <option value="ms">Milidetik (ms)</option>
                    <option value="detik">Detik (s)</option>
                    <option value="menit">Menit (min)</option>
                    <option value="jam">Jam (h)</option>
                    <option value="hari">Hari (d)</option>
                    <option value="minggu">Minggu (week)</option>
                    <option value="bulan">Bulan (month)</option>
                    <option value="tahun">Tahun (year)</option>
                `;
            }

            html += options + `</select>
                <label for="satuanTujuan">Satuan Tujuan:</label>
                <select id="satuanTujuan">
                    ${options}
                </select>
                <button onclick="konversi()">Konversi</button>
            `;

            inputKonversi.innerHTML = html;
        }

        function konversi() {
            const nilai = parseFloat(document.getElementById("nilai").value);
            const satuanAsal = document.getElementById("satuanAsal").value;
            const satuanTujuan = document.getElementById("satuanTujuan").value;
            let hasil;

            if (isNaN(nilai)) {
                alert("Masukkan nilai yang valid!");
                return;
            }

            const panjang = { mm: 1, cm: 10, m: 1000, km: 1000000, in: 25.4, ft: 304.8, yd: 914.4, mile: 1609344 };
            const berat = { mg: 1, gram: 1000, kg: 1000000, ton: 1000000000, lb: 453592.37, oz: 28349.5 };
            const waktu = { ms: 1, detik: 1000, menit: 60000, jam: 3600000, hari: 86400000, minggu: 604800000, bulan: 2592000000, tahun: 31536000000 };
            const suhu = {
                "c": val => val, "f": val => (val * 9 / 5) + 32, "k": val => val + 273.15, "r": val => val * 4 / 5,
                "c_reverse": val => val, "f_reverse": val => (val - 32) * 5 / 9, "k_reverse": val => val - 273.15, "r_reverse": val => val * 5 / 4
            };

            if (satuanAsal in panjang && satuanTujuan in panjang) {
                hasil = (nilai * panjang[satuanAsal]) / panjang[satuanTujuan];
            } else if (satuanAsal in berat && satuanTujuan in berat) {
                hasil = (nilai * berat[satuanAsal]) / berat[satuanTujuan];
            } else if (satuanAsal in waktu && satuanTujuan in waktu) {
                hasil = (nilai * waktu[satuanAsal]) / waktu[satuanTujuan];
            } else if (satuanAsal in suhu && satuanTujuan in suhu) {
                hasil = satuanAsal === satuanTujuan ? nilai : suhu[satuanTujuan](suhu[satuanAsal + "_reverse"](nilai));
            } else {
                hasil = "Satuan tidak valid atau tidak dapat dikonversi.";
            }

            document.getElementById("output").innerText = `Hasil: ${hasil}`;
        }
    </script>
</body>
</html>
