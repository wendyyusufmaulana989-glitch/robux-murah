<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Top Up Robux • QRIS DANA</title>
  <meta name="description" content="Top up Robux diskon 30% • Pembayaran QRIS DANA • Order via WhatsApp" />
  <link rel="icon" href="favicon.ico" />
  <!-- Tailwind CDN (works on GitHub Pages) -->
  <script src="https://cdn.tailwindcss.com"></script>
  <style>
    /* Simple skeleton shimmer */
    .shimmer{background:linear-gradient(90deg,#f3f4f6 25%,#e5e7eb 37%,#f3f4f6 63%);background-size:400% 100%;animation:shimmer 1.4s ease infinite}
    @keyframes shimmer{0%{background-position:100% 0}100%{background-position:0 0}}
  </style>
</head>
<body class="bg-neutral-50 text-neutral-900">
  <header class="sticky top-0 z-40 bg-white/80 backdrop-blur border-b border-neutral-200">
    <div class="max-w-6xl mx-auto px-4 py-3 flex items-center justify-between">
      <div class="flex items-center gap-3">
        <img src="/logo.png" alt="Logo" class="w-9 h-9 rounded-xl ring-1 ring-neutral-200" onerror="this.style.display='none'"/>
        <div>
          <h1 class="font-bold text-lg leading-tight">Top Up Robux</h1>
          <p class="text-xs text-neutral-500">Diskon 30% • Pembayaran QRIS DANA</p>
        </div>
      </div>
      <nav class="hidden sm:flex items-center gap-4 text-sm">
        <a href="#harga" class="hover:underline">Harga</a>
        <a href="#order" class="hover:underline">Order</a>
        <a href="#pembayaran" class="hover:underline">Pembayaran</a>
        <a href="#faq" class="hover:underline">FAQ</a>
      </nav>
    </div>
  </header>

  <main class="max-w-6xl mx-auto px-4 py-8">
    <!-- Hero -->
    <section class="grid md:grid-cols-2 gap-6 items-center">
      <div>
        <h2 class="text-3xl md:text-4xl font-extrabold">Top Up <span class="text-indigo-600">Robux</span> Murah & Aman</h2>
        <p class="mt-3 text-neutral-600">Bayar sekali klik pakai <strong>QRIS DANA</strong>. Order diverifikasi via WhatsApp. <span class="inline-block rounded-full bg-emerald-100 text-emerald-700 text-xs px-2 py-1 align-middle">Tanpa login password akun game</span>.</p>
        <ul class="mt-4 text-sm text-neutral-700 list-disc pl-5 space-y-1">
          <li>Diskon <strong>30%</strong> dari harga normal.</li>
          <li>Input <strong>Username Roblox</strong> & <strong>User ID</strong> saja.</li>
          <li>Order otomatis buat pesan WhatsApp ke admin.</li>
        </ul>
        <div class="mt-6 flex gap-3">
          <a href="#order" class="px-4 py-2.5 bg-indigo-600 hover:bg-indigo-700 text-white rounded-xl shadow">Mulai Order</a>
          <a href="#harga" class="px-4 py-2.5 bg-white border border-neutral-200 hover:bg-neutral-50 rounded-xl">Lihat Harga</a>
        </div>
      </div>
      <div class="aspect-video rounded-2xl bg-gradient-to-br from-indigo-50 to-purple-50 border border-neutral-200 p-6">
        <div class="grid grid-cols-2 gap-4 h-full">
          <div class="rounded-xl bg-white border border-neutral-200 p-4 flex flex-col justify-between">
            <div>
              <p class="text-sm font-semibold">Pembayaran</p>
              <p class="text-xs text-neutral-500">QRIS DANA</p>
            </div>
            <img src="/qris-dana.png" alt="QRIS DANA" class="w-full rounded-lg border border-neutral-200" onerror="this.classList.add('shimmer')"/>
          </div>
          <div class="rounded-xl bg-white border border-neutral-200 p-4 flex flex-col justify-between">
            <div>
              <p class="text-sm font-semibold">Order via</p>
              <p class="text-xs text-neutral-500">WhatsApp</p>
            </div>
            <a href="#order" class="block text-center px-3 py-2 rounded-lg border border-neutral-200 hover:bg-neutral-50">Buat Pesanan</a>
          </div>
        </div>
      </div>
    </section>

    <!-- Harga -->
    <section id="harga" class="mt-12">
      <h3 class="text-2xl font-bold">Harga Paket Robux (Diskon 30%)</h3>
      <p class="text-sm text-neutral-600 mt-1">Harga acuan dari paket resmi (USD) dikonversi ke IDR dan didiskon 30%. Kurs dapat berubah sewaktu-waktu. Harga dibulatkan ribuan terdekat.</p>
      <div id="priceGrid" class="mt-6 grid sm:grid-cols-2 lg:grid-cols-3 gap-4"></div>
    </section>

    <!-- Order Form -->
    <section id="order" class="mt-14">
      <h3 class="text-2xl font-bold">Form Order</h3>
      <div class="mt-6 grid md:grid-cols-2 gap-6">
        <form id="orderForm" class="bg-white border border-neutral-200 rounded-2xl p-5 space-y-4">
          <div>
            <label class="text-sm font-medium">Username Roblox</label>
            <input required id="rbxUsername" type="text" class="mt-1 w-full rounded-xl border border-neutral-300 px-3 py-2 focus:outline-none focus:ring-2 focus:ring-indigo-500" placeholder="mis. NoobMaster69" />
          </div>
          <div>
            <label class="text-sm font-medium">User ID Roblox (angka)</label>
            <input required id="rbxUserId" type="number" class="mt-1 w-full rounded-xl border border-neutral-300 px-3 py-2 focus:outline-none focus:ring-2 focus:ring-indigo-500" placeholder="mis. 1234567890" />
            <p class="text-xs text-neutral-500 mt-1">Lihat di profil: roblox.com/users/&lt;<em>id</em>&gt;/profile</p>
          </div>
          <div>
            <label class="text-sm font-medium">Nomor WhatsApp kamu</label>
            <input required id="buyerWa" type="tel" class="mt-1 w-full rounded-xl border border-neutral-300 px-3 py-2 focus:outline-none focus:ring-2 focus:ring-indigo-500" placeholder="08xxxxxxxxxx" />
          </div>
          <div>
            <label class="text-sm font-medium">Paket Robux</label>
            <select required id="package" class="mt-1 w-full rounded-xl border border-neutral-300 px-3 py-2 focus:outline-none focus:ring-2 focus:ring-indigo-500"></select>
          </div>
          <div>
            <label class="text-sm font-medium">Catatan (opsional)</label>
            <textarea id="notes" rows="3" class="mt-1 w-full rounded-xl border border-neutral-300 px-3 py-2 focus:outline-none focus:ring-2 focus:ring-indigo-500" placeholder="Contoh: nickname display, prefer jam kirim, dsb."></textarea>
          </div>
          <div class="flex items-center gap-3">
            <input id="tos" type="checkbox" required class="w-4 h-4" />
            <label for="tos" class="text-sm">Saya setuju <a href="#faq" class="underline">Ketentuan Layanan</a> & kebijakan tanpa password.</label>
          </div>
          <div class="flex gap-3">
            <button type="submit" class="px-4 py-2.5 bg-indigo-600 hover:bg-indigo-700 text-white rounded-xl shadow">Buat Pesan WhatsApp</button>
            <button type="button" id="copySummary" class="px-4 py-2.5 bg-white border border-neutral-200 hover:bg-neutral-50 rounded-xl">Salin Ringkasan</button>
          </div>
          <p id="formMsg" class="text-sm text-emerald-700 hidden">Pesan WhatsApp sudah dibuat 👍</p>
        </form>

        <!-- Pembayaran / QRIS -->
        <aside id="pembayaran" class="bg-white border border-neutral-200 rounded-2xl p-5">
          <h4 class="font-semibold">Pembayaran QRIS DANA</h4>
          <ol class="list-decimal pl-5 text-sm text-neutral-700 mt-2 space-y-1">
            <li>Pilih paket & buat pesanan.</li>
            <li>Scan QRIS DANA berikut dan bayar sesuai total.</li>
            <li>Kirim bukti bayar via WhatsApp (otomatis dari tombol order).</li>
          </ol>
          <img src="/qris-dana.png" alt="QRIS DANA" class="mt-4 w-full max-w-sm rounded-xl border border-neutral-200" onerror="this.classList.add('shimmer')"/>
          <div class="mt-4 text-xs text-neutral-500">
            <p>Catatan: Jika QR statis, tulis nominal sendiri sesuai total. Bila butuh QR dinamis, ganti gambar & instruksi ini.</p>
          </div>
        </aside>
      </div>
    </section>

    <!-- FAQ -->
    <section id="faq" class="mt-16">
      <h3 class="text-2xl font-bold">FAQ</h3>
      <div class="mt-4 grid md:grid-cols-2 gap-4">
        <div class="bg-white border border-neutral-200 rounded-2xl p-5">
          <p class="font-semibold">Apakah perlu login password akun Roblox?</p>
          <p class="text-sm text-neutral-700 mt-1">Tidak. Kami <strong>tidak pernah</strong> meminta password. Cukup Username & User ID untuk proses top up.</p>
        </div>
        <div class="bg-white border border-neutral-200 rounded-2xl p-5">
          <p class="font-semibold">Bagaimana verifikasi pembayaran?</p>
          <p class="text-sm text-neutral-700 mt-1">Admin akan verifikasi manual via WhatsApp setelah kamu kirim bukti bayar.</p>
        </div>
        <div class="bg-white border border-neutral-200 rounded-2xl p-5">
          <p class="font-semibold">Apakah ada database pelanggan?</p>
          <p class="text-sm text-neutral-700 mt-1">Template ini bisa dikaitkan ke <em>Google Form</em> (gratis) agar semua order masuk ke Google Sheets milikmu. Lihat bagian "Integrasi Opsional" di bawah.</p>
        </div>
        <div class="bg-white border border-neutral-200 rounded-2xl p-5">
          <p class="font-semibold">Berapa lama proses?</p>
          <p class="text-sm text-neutral-700 mt-1">Tergantung antrean & verifikasi. Admin akan konfirmasi perkiraan setelah bukti bayar diterima.</p>
        </div>
      </div>
    </section>

    <!-- Integrasi Opsional -->
    <section class="mt-14">
      <h3 class="text-2xl font-bold">Integrasi Opsional (Gratis)</h3>
      <div class="bg-white border border-neutral-200 rounded-2xl p-5">
        <ol class="list-decimal pl-5 text-sm text-neutral-700 space-y-2">
          <li><strong>Google Form + Google Sheets</strong>: buat form dengan field yang sama (Username, User ID, WA, Paket, Catatan, Total). Salin <em>POST URL</em> & mapping <em>entry.xxxxx</em> lalu tempel ke konstanta <code>GOOGLE_FORM_POST_URL</code> & <code>GOOGLE_FORM_MAP</code> di bawah agar setiap order otomatis tercatat ke Sheets.</li>
          <li><strong>WhatsApp Admin</strong>: set nomor admin di konstanta <code>ADMIN_WA</code> agar tombol order mengarah ke chat yang benar.</li>
        </ol>
      </div>
    </section>

    <footer class="mt-16 py-10 text-center text-xs text-neutral-500">
      <p>ⓒ <span id="y"></span> Top Up Robux. Bukan situs resmi Roblox. Semua merek dagang adalah milik masing-masing pemiliknya.</p>
    </footer>
  </main>

  <script>
    // ====== KONFIGURASI ======
    // Kurs USD→IDR (per 25 Aug 2025, referensi publik). Ganti manual kapan saja.
    const USD_TO_IDR = 16254.5;
    const DISKON = 0.30; // 30%
    const ADMIN_WA = '62812xxxxxxx'; // ganti ke nomor admin (format internasional tanpa +)

    // Jika gunakan Google Form, isi URL & mapping field entry. Biarkan kosong jika tidak dipakai.
    const GOOGLE_FORM_POST_URL = '';
    const GOOGLE_FORM_MAP = {
      // contoh: username: 'entry.1111111111', userId: 'entry.2222222222', phone: 'entry.3333333333', paket: 'entry.4444444444', total: 'entry.5555555555', catatan: 'entry.6666666666'
    };

    // Paket resmi (USD). Sumber umum: 400/800/1700/4500/10000 Robux.
    const RAW_PACKS = [
      { name: '400 Robux', usd: 4.99 },
      { name: '800 Robux', usd: 9.99 },
      { name: '1.700 Robux', usd: 19.99 },
      { name: '4.500 Robux', usd: 49.99 },
      { name: '10.000 Robux', usd: 99.99 },
    ];

    function roundToThousand(v){ return Math.round(v/1000)*1000 }

    function computePacks(){
      return RAW_PACKS.map(p=>{
        const baseIdr = p.usd * USD_TO_IDR;
        const discIdr = baseIdr * (1 - DISKON);
        return {
          label: p.name,
          usd: p.usd,
          baseIdr: roundToThousand(baseIdr),
          priceIdr: roundToThousand(discIdr)
        }
      })
    }

    const packs = computePacks();

    // Render harga
    const grid = document.getElementById('priceGrid');
    grid.innerHTML = packs.map((p,i)=>`
      <div class="bg-white border border-neutral-200 rounded-2xl p-5">
        <div class="flex items-baseline justify-between">
          <h4 class="font-semibold">${p.label}</h4>
          <span class="text-xs rounded-full bg-emerald-100 text-emerald-700 px-2 py-0.5">Diskon 30%</span>
        </div>
        <p class="mt-1 text-sm line-through text-neutral-400">Rp ${p.baseIdr.toLocaleString('id-ID')}</p>
        <p class="text-2xl font-extrabold">Rp ${p.priceIdr.toLocaleString('id-ID')}</p>
        <p class="text-xs text-neutral-500">Acuan USD ${p.usd.toFixed(2)} → IDR ${USD_TO_IDR.toLocaleString('id-ID')}</p>
      </div>
    `).join('');

    // Render select
    const sel = document.getElementById('package');
    sel.innerHTML = packs.map((p,idx)=>`<option value="${idx}">${p.label} — Rp ${p.priceIdr.toLocaleString('id-ID')}</option>`).join('');

    // Order submit → WhatsApp + (opsional) Google Form
    const form = document.getElementById('orderForm');
    form.addEventListener('submit', async (e)=>{
      e.preventDefault();
      const username = document.getElementById('rbxUsername').value.trim();
      const userId = document.getElementById('rbxUserId').value.trim();
      const phone = document.getElementById('buyerWa').value.replace(/\D/g,'');
      const idx = parseInt(document.getElementById('package').value,10);
      const notes = document.getElementById('notes').value.trim();
      const pack = packs[idx];

      const order = {
        username, userId, buyerWa: phone, paket: pack.label, total: pack.priceIdr, notes
      };

      // WhatsApp deep link → admin
      const text = `Halo Admin, saya mau top up Robux:%0A\n- Username: ${encodeURIComponent(username)}%0A- User ID: ${encodeURIComponent(userId)}%0A- Paket: ${encodeURIComponent(pack.label)}%0A- Total: Rp ${pack.priceIdr.toLocaleString('id-ID')}%0A- WA Saya: ${encodeURIComponent(phone)}%0A- Catatan: ${encodeURIComponent(notes||'-')}%0A\nBukti bayar QRIS akan saya kirim.`;
      const waUrl = `https://wa.me/${ADMIN_WA}?text=${text}`;

      // Optional: kirim ke Google Form (no-cors)
      if(GOOGLE_FORM_POST_URL){
        const body = new URLSearchParams();
        if(GOOGLE_FORM_MAP.username) body.append(GOOGLE_FORM_MAP.username, username);
        if(GOOGLE_FORM_MAP.userId) body.append(GOOGLE_FORM_MAP.userId, userId);
        if(GOOGLE_FORM_MAP.phone) body.append(GOOGLE_FORM_MAP.phone, phone);
        if(GOOGLE_FORM_MAP.paket) body.append(GOOGLE_FORM_MAP.paket, pack.label);
        if(GOOGLE_FORM_MAP.total) body.append(GOOGLE_FORM_MAP.total, pack.priceIdr);
        if(GOOGLE_FORM_MAP.catatan) body.append(GOOGLE_FORM_MAP.catatan, notes);
        try{ await fetch(GOOGLE_FORM_POST_URL,{ method:'POST', mode:'no-cors', body }); }catch(err){ console.warn('Google Form error', err); }
      }

      document.getElementById('formMsg').classList.remove('hidden');
      window.open(waUrl, '_blank');
    });

    // Salin ringkasan
    document.getElementById('copySummary').addEventListener('click', ()=>{
      const idx = parseInt(document.getElementById('package').value,10);
      const pack = packs[idx];
      const username = document.getElementById('rbxUsername').value.trim();
      const userId = document.getElementById('rbxUserId').value.trim();
      const notes = document.getElementById('notes').value.trim();
      const summary = `Order Robux\n- Username: ${username}\n- User ID: ${userId}\n- Paket: ${pack.label}\n- Total: Rp ${pack.priceIdr.toLocaleString('id-ID')}\n- Catatan: ${notes||'-'}\nPembayaran via QRIS DANA.`;
      navigator.clipboard.writeText(summary).then(()=>{
        const m = document.getElementById('formMsg');
        m.textContent = 'Ringkasan tersalin ke clipboard ✅';
        m.classList.remove('hidden');
      });
    });

    // Footer year
    document.getElementById('y').textContent = new Date().getFullYear();
  </script>
</body>
</html>
