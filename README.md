<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pendaftaran Belajar Bahasa Jepang Online</title>
    <style>
        * {margin:0; padding:0; box-sizing:border-box; font-family:'Segoe UI', sans-serif;}
        body {background:linear-gradient(135deg, #fef5f5, #fce4ec); min-height:100vh; padding:20px;}
        .container {max-width:700px; margin:0 auto; background:#fff; border-radius:16px; box-shadow:0 4px 20px rgba(0,0,0,0.1); padding:30px;}
        h1 {text-align:center; color:#b71c1c; margin-bottom:10px; font-size:1.8rem;}
        .subhead {text-align:center; color:#666; margin-bottom:30px;}
        .form-group {margin-bottom:18px;}
        label {display:block; margin-bottom:6px; font-weight:600; color:#333;}
        input, select, textarea {width:100%; padding:12px; border:1px solid #ddd; border-radius:8px; font-size:1rem;}
        input:focus, select:focus, textarea:focus {outline:none; border-color:#b71c1c; box-shadow:0 0 0 3px rgba(183,28,28,0.1);}
        .radio-group, .checkbox-group {display:flex; flex-wrap:wrap; gap:15px; margin-top:8px;}
        .radio-item, .checkbox-item {display:flex; align-items:center; gap:6px; cursor:pointer;}
        button {width:100%; padding:14px; background:#b71c1c; color:#fff; border:none; border-radius:8px; font-size:1.1rem; font-weight:600; cursor:pointer; margin-top:10px; transition:background 0.3s;}
        button:hover {background:#9e1515;}
        .btn-secondary {background:#f5f5f5; color:#333; margin-top:8px;}
        .btn-secondary:hover {background:#e0e0e0;}
        .agreement {margin-top:25px; padding:15px; background:#fef0f0; border-radius:8px;}
        .agreement p {margin-bottom:10px; display:flex; align-items:flex-start; gap:8px;}
        .success {display:none; text-align:center; padding:30px;}
        .success h2 {color:#2e7d32; margin-bottom:15px;}
        .print-area {display:none;}
        @media print {
            body {background:#fff;}
            .no-print {display:none !important;}
            .print-area {display:block !important;}
        }
    </style>
</head>
<body>
    <div class="container no-print" id="formContainer">
        <h1>🌸 Pendaftaran Belajar Bahasa Jepang Online</h1>
        <p class="subhead">Silakan lengkapi formulir di bawah ini dengan data yang benar</p>

        <form id="registrationForm">
            <!-- 1 -->
            <div class="form-group">
                <label>1. Nama Lengkap sesuai KTP *</label>
                <input type="text" id="nama" required placeholder="Contoh: Siti Aminah">
            </div>

            <!-- 2 -->
            <div class="form-group">
                <label>2. Jenis Kelamin *</label>
                <div class="radio-group">
                    <label class="radio-item"><input type="radio" name="gender" value="Laki-laki" required> Laki-laki</label>
                    <label class="radio-item"><input type="radio" name="gender" value="Perempuan"> Perempuan</label>
                </div>
            </div>

            <!-- 3 -->
            <div class="form-group">
                <label>3. Tempat & Tanggal Lahir *</label>
                <input type="text" id="tempatLahir" required placeholder="Tempat lahir">
                <input type="date" id="tglLahir" required style="margin-top:8px;">
            </div>

            <!-- 4 -->
            <div class="form-group">
                <label>4. Nomor WhatsApp Aktif *</label>
                <input type="tel" id="whatsapp" required placeholder="Contoh: 081234567890">
            </div>

            <!-- 5 -->
            <div class="form-group">
                <label>5. Alamat Email *</label>
                <input type="email" id="email" required placeholder="email@contoh.com">
            </div>

            <!-- 6 -->
            <div class="form-group">
                <label>6. Pekerjaan Saat Ini *</label>
                <select id="pekerjaan" required>
                    <option value="">-- Pilih --</option>
                    <option value="Pelajar">Pelajar</option>
                    <option value="Mahasiswa">Mahasiswa</option>
                    <option value="Karyawan">Karyawan</option>
                    <option value="Lainnya">Lainnya</option>
                </select>
                <input type="text" id="pekerjaanLain" placeholder="Sebutkan pekerjaan Anda" style="margin-top:8px; display:none;">
            </div>

            <!-- 7 -->
            <div class="form-group">
                <label>7. Alamat Lengkap *</label>
                <textarea id="alamat" rows="3" required placeholder="Alamat lengkap beserta kode pos"></textarea>
            </div>

            <!-- 8 -->
            <div class="form-group">
                <label>8. Level Bahasa Jepang *</label>
                <div class="radio-group">
                    <label class="radio-item"><input type="radio" name="level" value="N5" required> N5</label>
                    <label class="radio-item"><input type="radio" name="level" value="N4"> N4</label>
                </div>
            </div>

            <!-- 9 -->
            <div class="form-group">
                <label>9. Sesi Belajar Pilihan *</label>
                <div class="radio-group">
                    <label class="radio-item"><input type="radio" name="sesi" value="Sesi Pagi (09.00 - 10.30 WIB)" required> Sesi Pagi (09.00 - 10.30 WIB)</label>
                    <label class="radio-item"><input type="radio" name="sesi" value="Sesi Malam (19.00 - 20.30 WIB)"> Sesi Malam (19.00 - 20.30 WIB)</label>
                </div>
            </div>

            <!-- 10 -->
            <div class="form-group">
                <label>10. Tujuan Belajar *</label>
                <select id="tujuan" required>
                    <option value="">-- Pilih --</option>
                    <option value="Hobi">Hobi</option>
                    <option value="Persiapan Studi">Persiapan Studi</option>
                    <option value="Persiapan Kerja Magang / Tokutei Ginou">Persiapan Kerja Magang / Tokutei Ginou</option>
                    <option value="Lainnya">Lainnya</option>
                </select>
                <input type="text" id="tujuanLain" placeholder="Sebutkan tujuan Anda" style="margin-top:8px; display:none;">
            </div>

            <!-- Persetujuan -->
            <div class="agreement">
                <label><strong>Persetujuan *</strong></label>
                <p>
                    <input type="checkbox" id="setujuData" required>
                    <label for="setujuData">Saya menyatakan bahwa data yang saya isi di atas adalah benar dan valid.</label>
                </p>
                <p>
                    <input type="checkbox" id="setujuAturan" required>
                    <label for="setujuAturan">Saya bersedia mengikuti tata tertib kelas online yang berlaku.</label>
                </p>
            </div>

            <button type="submit">Kirim Pendaftaran</button>
            <button type="button" class="btn-secondary" onclick="window.print()">Cetak Formulir</button>
        </form>
    </div>

    <!-- Halaman Sukses -->
    <div class="container success" id="successPage">
        <h2>✅ Pendaftaran Berhasil!</h2>
        <p>Terima kasih telah mendaftar. Konfirmasi akan dikirim ke email Anda dan ke <strong>japaneseonlineclass.co@gmail.com</strong></p>
        <div id="ringkasanData" style="margin:20px 0; text-align:left; background:#f9f9f9; padding:20px; border-radius:8px;"></div>
        <button class="btn-secondary" onclick="window.print()">Cetak Bukti Pendaftaran</button>
        <button class="btn-secondary" onclick="location.reload()">Daftar Ulang</button>
    </div>

    <!-- Area Cetak -->
    <div class="print-area" id="printArea">
        <h2 style="text-align:center; color:#b71c1c;">BUKTI PENDAFTARAN BELAJAR BAHASA JEPANG ONLINE</h2>
        <p style="text-align:center; margin-bottom:20px;">Tanggal: <span id="printTanggal"></span></p>
        <table border="1" cellpadding="10" cellspacing="0" style="width:100%; border-collapse:collapse; margin-top:15px;">
            <tbody id="printContent"></tbody>
        </table>
        <p style="margin-top:30px; text-align:right;">Tanda Tangan,<br><br><br><br>( ........................... )</p>
    </div>

    <script>
        // Tampilkan input tambahan jika pilih Lainnya
        document.getElementById('pekerjaan').addEventListener('change', function(){
            document.getElementById('pekerjaanLain').style.display = this.value==='Lainnya' ? 'block' : 'none';
        });
        document.getElementById('tujuan').addEventListener('change', function(){
            document.getElementById('tujuanLain').style.display = this.value==='Lainnya' ? 'block' : 'none';
        });

        document.getElementById('registrationForm').addEventListener('submit', function(e){
            e.preventDefault();

            // Ambil semua nilai
            const getData = () => ({
                nama: document.getElementById('nama').value,
                gender: document.querySelector('input[name="gender"]:checked').value,
                tempatLahir: document.getElementById('tempatLahir').value,
                tglLahir: document.getElementById('tglLahir').value,
                whatsapp: document.getElementById('whatsapp').value,
                email: document.getElementById('email').value,
                pekerjaan: document.getElementById('pekerjaan').value === 'Lainnya' 
                    ? document.getElementById('pekerjaanLain').value 
                    : document.getElementById('pekerjaan').value,
                alamat: document.getElementById('alamat').value,
                level: document.querySelector('input[name="level"]:checked').value,
                sesi: document.querySelector('input[name="sesi"]:checked').value,
                tujuan: document.getElementById('tujuan').value === 'Lainnya' 
                    ? document.getElementById('tujuanLain').value 
                    : document.getElementById('tujuan').value,
                tglDaftar: new Date().toLocaleString('id-ID', {dateStyle:'full', timeStyle:'short'})
            });

            const data = getData();

            // 1. Simpan ke localStorage (bisa dibuka Excel lewat export)
            let pendaftaran = JSON.parse(localStorage.getItem('pendaftaran') || '[]');
            pendaftaran.push(data);
            localStorage.setItem('pendaftaran', JSON.stringify(pendaftaran));

            // 2. Tampilkan ringkasan
            const html = Object.entries(data).map(([k,v]) => `<p><strong>${k}:</strong> ${v}</p>`).join('');
            document.getElementById('ringkasanData').innerHTML = html;

            // 3. Isi area cetak
            document.getElementById('printTanggal').textContent = data.tglDaftar;
            const labelMap = {
                nama: 'Nama Lengkap', gender: 'Jenis Kelamin', tempatLahir: 'Tempat Lahir',
                tglLahir: 'Tanggal Lahir', whatsapp: 'No. WhatsApp', email: 'Alamat Email',
                pekerjaan: 'Pekerjaan', alamat: 'Alamat Lengkap', level: 'Level Bahasa',
                sesi: 'Sesi Belajar', tujuan: 'Tujuan Belajar', tglDaftar: 'Tanggal Pendaftaran'
            };
            document.getElementById('printContent').innerHTML = Object.entries(data)
                .map(([k,v]) => `<tr><td style="width:40%; background:#f5f5f5;">${labelMap[k]}</td><td>${v}</td></tr>`).join('');

            // 4. Kirim email (menggunakan mailto - akan buka aplikasi email pengguna)
            const subject = encodeURIComponent(`Pendaftaran Baru: ${data.nama} - ${data.level}`);
            const body = encodeURIComponent(
`Pendaftaran Belajar Bahasa Jepang Online

Nama: ${data.nama}
Jenis Kelamin: ${data.gender}
Tempat, Tanggal Lahir: ${data.tempatLahir}, ${data.tglLahir}
No. WhatsApp: ${data.whatsapp}
Email: ${data.email}
Pekerjaan: ${data.pekerjaan}
Alamat: ${data.alamat}
Level: ${data.level}
Sesi: ${data.sesi}
Tujuan Belajar: ${data.tujuan}
Tanggal Daftar: ${data.tglDaftar}

--- Silakan hubungi calon peserta segera ---`
            );
            window.location.href = `mailto:japaneseonlineclass.co@gmail.com?cc=${data.email}&subject=${subject}&body=${body}`;

            // Tampilkan halaman sukses
            document.getElementById('formContainer').style.display = 'none';
            document.getElementById('successPage').style.display = 'block';
        });

        // Fungsi export ke Excel
        function exportToExcel(){
            const data = JSON.parse(localStorage.getItem('pendaftaran') || '[]');
            if(!data.length) return alert('Belum ada data pendaftaran');
            
            const csv = [
                ['Nama','Jenis Kelamin','Tempat Lahir','Tanggal Lahir','WhatsApp','Email','Pekerjaan','Alamat','Level','Sesi','Tujuan','Tanggal Daftar'].join(','),
                ...data.map(d => [
                    `"${d.nama}","${d.gender}","${d.tempatLahir}","${d.tglLahir}","${d.whatsapp}","${d.email}","${d.pekerjaan}","${d.alamat}","${d.level}","${d.sesi}","${d.tujuan}","${d.tglDaftar}"`
                ].join(','))
            ].join('\n');
            
            const blob = new Blob([csv], {type:'text/csv;charset=utf-8;'});
            const url = URL.createObjectURL(blob);
            const a = document.createElement('a');
            a.href = url; a.download = 'Pendaftaran_Bahasa_Jepang.csv'; a.click();
        }

        // Tambahkan tombol export
        window.onload = function(){
            const btn = document.createElement('button');
            btn.textContent = '📊 Ekspor Data ke Excel';
            btn.className = 'btn-secondary no-print';
            btn.onclick = exportToExcel;
            document.querySelector('.container').appendChild(btn);
        };
    </script>
</body>
</html>
