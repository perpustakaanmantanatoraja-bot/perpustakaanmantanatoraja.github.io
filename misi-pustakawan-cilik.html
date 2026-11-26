<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Misi Pustakawan Cilik — Game Edukasi Perpustakaan</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Fredoka:wght@500;600;700&family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet">
    <style>
        :root {
            --bg-cream: #FAF6EE;
            --wood-dark: #4A3222;
            --wood-mid: #7A5236;
            --sage-main: #588157;
            --sage-dark: #3A5A40;
        }

        body {
            font-family: 'Inter', system-ui, -apple-system, sans-serif;
            background-color: var(--bg-cream);
            background-image:
                radial-gradient(circle at 12% 15%, rgba(163, 177, 138, 0.22) 0%, transparent 42%),
                radial-gradient(circle at 88% 82%, rgba(217, 119, 6, 0.12) 0%, transparent 45%);
            color: var(--wood-dark);
            overflow-x: hidden;
        }

        .font-display {
            font-family: 'Fredoka', 'Inter', cursive, sans-serif;
        }

        @keyframes popIn {
            0% {
                opacity: 0;
                transform: scale(0.92) translateY(8px);
            }
            100% {
                opacity: 1;
                transform: scale(1) translateY(0);
            }
        }

        @keyframes shake {
            0%, 100% { transform: translateX(0); }
            20% { transform: translateX(-8px) rotate(-1.5deg); }
            40% { transform: translateX(8px) rotate(1.5deg); }
            60% { transform: translateX(-6px) rotate(-1deg); }
            80% { transform: translateX(6px) rotate(1deg); }
        }

        @keyframes floatUp {
            0% {
                opacity: 1;
                transform: translate(-50%, 0) scale(0.95);
            }
            100% {
                opacity: 0;
                transform: translate(-50%, -52px) scale(1.08);
            }
        }

        .animate-pop-in {
            animation: popIn 0.28s cubic-bezier(0.22, 1, 0.36, 1) forwards;
        }

        .animate-shake {
            animation: shake 0.42s ease-in-out;
        }

        .floating-feedback {
            position: fixed;
            z-index: 70;
            pointer-events: none;
            font-family: 'Fredoka', sans-serif;
            font-weight: 700;
            font-size: 0.95rem;
            padding: 0.35rem 0.75rem;
            border-radius: 9999px;
            background: rgba(255, 255, 255, 0.96);
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.14);
            animation: floatUp 1.05s ease-out forwards;
            white-space: nowrap;
        }

        .btn-primary {
            background: linear-gradient(180deg, #6A994E 0%, #3A5A40 100%);
            box-shadow: 0 4px 0 #233827;
            transition: transform 0.12s ease, filter 0.15s ease, box-shadow 0.12s ease;
        }

        .btn-primary:hover {
            filter: brightness(1.06);
        }

        .btn-primary:active {
            transform: translateY(3px);
            box-shadow: 0 1px 0 #233827;
        }

        .shelf-card {
            transition: transform 0.16s ease, box-shadow 0.16s ease, border-color 0.16s ease;
            touch-action: manipulation;
        }

        .shelf-card:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 20px rgba(74, 50, 34, 0.14);
        }

        .shelf-card:active {
            transform: translateY(0px) scale(0.98);
        }

        .shelf-drag-over {
            transform: scale(1.03) translateY(-4px) !important;
            box-shadow: 0 0 0 4px rgba(245, 158, 11, 0.65), 0 12px 24px rgba(0, 0, 0, 0.16) !important;
        }

        /* Custom scrollbar lembut */
        ::-webkit-scrollbar {
            width: 7px;
            height: 7px;
        }
        ::-webkit-scrollbar-track {
            background: #F2E8D5;
            border-radius: 9999px;
        }
        ::-webkit-scrollbar-thumb {
            background: #B68D65;
            border-radius: 9999px;
        }
    </style>
</head>
<body class="min-h-screen flex flex-col selection:bg-amber-200 selection:text-[#4A3222]">

    <!-- HEADER APLIKASI -->
    <header class="bg-[#362216] text-[#FAF6EE] border-b-4 border-[#63432E] shadow-md sticky top-0 z-30">
        <div class="max-w-6xl mx-auto px-3 sm:px-6 py-2.5 flex items-center justify-between gap-2">
            <!-- Identitas Brand -->
            <button id="btn-brand-home" type="button" class="flex items-center gap-2.5 text-left group cursor-pointer focus:outline-none">
                <div class="w-10 h-10 sm:w-11 sm:h-11 rounded-2xl bg-amber-400 text-[#362216] flex items-center justify-center text-xl sm:text-2xl shadow-inner group-hover:scale-105 transition">
                    📚
                </div>
                <div>
                    <div class="flex items-center gap-2">
                        <span class="font-display font-bold text-base sm:text-xl tracking-tight text-amber-300">
                            Misi Pustakawan Cilik
                        </span>
                        <span class="hidden sm:inline-block text-[10px] font-bold uppercase tracking-wider bg-[#588157] text-white px-2 py-0.5 rounded-full">
                            Edukasi DDC
                        </span>
                    </div>
                    <p class="text-[11px] text-[#E6D5BE] hidden sm:block">
                        Susun rak, rawat buku rusak, &amp; bantu pengunjung perpustakaan
                    </p>
                </div>
            </button>

            <!-- Kontrol Global -->
            <div class="flex items-center gap-1.5 sm:gap-2">
                <!-- Toggle Mode Pembahasan Instan -->
                <button
                    id="btn-instant-explain"
                    type="button"
                    class="bg-[#4A3222] hover:bg-[#63432E] text-[#FAF6EE] text-xs sm:text-sm font-semibold px-2.5 sm:px-3 py-2 rounded-xl border border-[#A67B5B]/50 transition flex items-center gap-1.5 shadow-sm cursor-pointer"
                    title="Aktifkan atau nonaktifkan Pembahasan Instan saat salah"
                >
                    <span>💡</span>
                    <span class="hidden md:inline">Pembahasan:</span>
                    <span id="explain-status" class="font-extrabold text-amber-300">ON</span>
                </button>

                <!-- Tombol Panduan DDC -->
                <button
                    id="btn-guide"
                    type="button"
                    class="bg-[#588157] hover:bg-[#6A994E] text-white text-xs sm:text-sm font-semibold px-2.5 sm:px-3 py-2 rounded-xl border border-[#A3B18A]/50 transition flex items-center gap-1.5 shadow-sm cursor-pointer"
                >
                    <span>📖</span>
                    <span>Panduan DDC</span>
                </button>

                <!-- Tombol Mute / Unmute -->
                <button
                    id="btn-sound"
                    type="button"
                    aria-label="Suara"
                    class="bg-[#4A3222] hover:bg-[#63432E] text-[#FAF6EE] p-2 sm:px-3 rounded-xl border border-[#A67B5B]/50 transition shadow-sm cursor-pointer"
                    title="Aktifkan atau matikan efek suara"
                >
                    <span id="sound-icon" class="text-base sm:text-lg">🔊</span>
                </button>
            </div>
        </div>
    </header>

    <!-- KONTEN UTAMA -->
    <main class="flex-1 max-w-6xl w-full mx-auto px-3 sm:px-6 py-4 sm:py-6 flex flex-col">

        <!-- =========================================================
             LAYAR 1: MENU UTAMA / BERANDA
             ========================================================= -->
        <section id="screen-start" class="my-auto py-2 animate-pop-in">
            <div class="bg-white/90 backdrop-blur-xs border-4 border-[#D8C3A5] rounded-3xl p-5 sm:p-8 shadow-xl">
                <div class="grid grid-cols-1 lg:grid-cols-12 gap-6 lg:gap-8 items-center">
                    <!-- Kolom Kiri: Pengenalan & Pemilihan Level -->
                    <div class="lg:col-span-7 space-y-5">
                        <div class="inline-flex items-center gap-2 bg-[#E9EDC9] text-[#3A5A40] border border-[#A3B18A] px-3.5 py-1 rounded-full text-xs sm:text-sm font-bold">
                            <span>🌟</span>
                            <span>Petualangan Literasi &amp; Klasifikasi Buku</span>
                        </div>

                        <h1 class="font-display font-bold text-3xl sm:text-4xl lg:text-5xl text-[#362216] leading-tight">
                            Jadilah Pustakawan Hebat di <span class="text-[#3A5A40]">Perpustakaan Ceria!</span>
                        </h1>

                        <p class="text-sm sm:text-base text-[#5C3D28] leading-relaxed">
                            Tugasmu adalah mengembalikan buku ke rak sesuai kode <strong>DDC (500–900)</strong>, memindahkan <strong>Buku Rusak</strong> ke <em>Keranjang Perbaikan</em>, dan menjawab pertanyaan <strong>Pengunjung</strong> sebelum waktu habis!
                        </p>

                        <!-- Pemilih Tingkat Kesulitan -->
                        <div class="space-y-2">
                            <label class="block text-xs sm:text-sm font-bold uppercase tracking-wide text-[#7A5236]">
                                Pilih Tingkat Tantangan:
                            </label>
                            <div class="grid grid-cols-1 sm:grid-cols-3 gap-2.5" id="difficulty-group">
                                <button
                                    type="button"
                                    data-diff="easy"
                                    class="diff-btn text-left p-3.5 rounded-2xl border-2 border-[#3A5A40] bg-[#E9EDC9]/80 shadow-xs transition cursor-pointer"
                                >
                                    <div class="flex items-center justify-between mb-1">
                                        <span class="font-display font-bold text-base text-[#283E2C]">🌱 Pemula</span>
                                        <span class="text-[11px] font-bold bg-[#3A5A40] text-white px-2 py-0.5 rounded-full">90d</span>
                                    </div>
                                    <p class="text-xs text-[#3A5A40]">Santai &amp; ramah belajar, cocok untuk latihan awal.</p>
                                </button>

                                <button
                                    type="button"
                                    data-diff="medium"
                                    class="diff-btn text-left p-3.5 rounded-2xl border-2 border-[#D8C3A5] bg-[#FAF6EE] hover:border-[#A67B5B] transition cursor-pointer"
                                >
                                    <div class="flex items-center justify-between mb-1">
                                        <span class="font-display font-bold text-base text-[#4A3222]">⚡ Terampil</span>
                                        <span class="text-[11px] font-bold bg-[#A67B5B] text-white px-2 py-0.5 rounded-full">75d</span>
                                    </div>
                                    <p class="text-xs text-[#6B4C35]">Antrean buku &amp; pengunjung lebih aktif berdatangan.</p>
                                </button>

                                <button
                                    type="button"
                                    data-diff="hard"
                                    class="diff-btn text-left p-3.5 rounded-2xl border-2 border-[#D8C3A5] bg-[#FAF6EE] hover:border-[#A67B5B] transition cursor-pointer"
                                >
                                    <div class="flex items-center justify-between mb-1">
                                        <span class="font-display font-bold text-base text-[#4A3222]">🔥 Kepala Rak</span>
                                        <span class="text-[11px] font-bold bg-amber-600 text-white px-2 py-0.5 rounded-full">60d</span>
                                    </div>
                                    <p class="text-xs text-[#6B4C35]">Tempo cepat untuk menguji ketelitian &amp; kombo!</p>
                                </button>
                            </div>
                        </div>

                        <!-- Tombol Mulai -->
                        <div class="pt-1 flex flex-wrap items-center gap-3">
                            <button
                                id="btn-start-game"
                                type="button"
                                class="btn-primary px-8 py-4 rounded-2xl text-white font-display font-bold text-lg sm:text-xl flex items-center gap-2.5 cursor-pointer"
                            >
                                <span>🚀</span>
                                <span>Mulai Bertugas</span>
                            </button>
                            <button
                                id="btn-open-guide-start"
                                type="button"
                                class="px-5 py-4 rounded-2xl bg-[#F2E8D5] hover:bg-[#E6D5BE] text-[#4A3222] border-2 border-[#C8AE8C] font-display font-bold text-base transition flex items-center gap-2 cursor-pointer"
                            >
                                <span>📖</span>
                                <span>Lihat Kode DDC</span>
                            </button>
                        </div>
                    </div>

                    <!-- Kolom Kanan: Kartu Aturan Cepat & Peta Rak -->
                    <div class="lg:col-span-5 bg-[#FAF6EE] border-2 border-[#E2D0B6] rounded-3xl p-4 sm:p-5 space-y-3.5">
                        <h2 class="font-display font-bold text-lg text-[#4A3222] flex items-center gap-2">
                            <span>🎯</span>
                            <span>Cara Bermain Cepat</span>
                        </h2>

                        <div class="space-y-2.5 text-xs sm:text-sm text-[#5C3D28]">
                            <div class="flex items-start gap-2.5 bg-white p-3 rounded-2xl border border-[#EADBC5]">
                                <span class="text-lg">👆</span>
                                <p><strong>Klik Rak atau Seret Buku:</strong> Ketuk/klik kartu rak tujuan (nyaman di HP &amp; tablet) atau <em>drag-and-drop</em> buku ke rak yang sesuai.</p>
                            </div>
                            <div class="flex items-start gap-2.5 bg-white p-3 rounded-2xl border border-[#EADBC5]">
                                <span class="text-lg">🩹</span>
                                <p><strong>Waspada Buku Rusak:</strong> Jika ada label <em>Sobek / Halaman Lepas / Bernoda</em>, arahkan ke <strong>Keranjang Perbaikan</strong>.</p>
                            </div>
                            <div class="flex items-start gap-2.5 bg-white p-3 rounded-2xl border border-[#EADBC5]">
                                <span class="text-lg">🙋</span>
                                <p><strong>Bantu Pengunjung:</strong> Saat spanduk pengunjung muncul, klik rak yang dicari untuk bonus <strong>+150 poin &amp; +5 detik</strong>!</p>
                            </div>
                        </div>

                        <!-- Mini Preview 6 Zona -->
                        <div class="pt-1">
                            <p class="text-[11px] font-bold uppercase tracking-wider text-[#7A5236] mb-2">Zona Tujuan di Perpustakaan:</p>
                            <div class="grid grid-cols-2 gap-1.5 text-xs font-bold">
                                <span class="bg-emerald-100 text-emerald-900 px-2.5 py-1.5 rounded-xl border border-emerald-300">🔬 500 • Sains &amp; Alam</span>
                                <span class="bg-sky-100 text-sky-900 px-2.5 py-1.5 rounded-xl border border-sky-300">💻 600 • Teknologi</span>
                                <span class="bg-purple-100 text-purple-900 px-2.5 py-1.5 rounded-xl border border-purple-300">🎨 700 • Seni &amp; Musik</span>
                                <span class="bg-rose-100 text-rose-900 px-2.5 py-1.5 rounded-xl border border-rose-300">🐉 800 • Sastra &amp; Fiksi</span>
                                <span class="bg-amber-100 text-amber-950 px-2.5 py-1.5 rounded-xl border border-amber-300">🏛️ 900 • Sejarah</span>
                                <span class="bg-orange-100 text-orange-950 px-2.5 py-1.5 rounded-xl border border-dashed border-orange-500">🩹 Perbaikan Buku</span>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- =========================================================
             LAYAR 2: ARENA PERMAINAN AKTIF
             ========================================================= -->
        <section id="screen-game" class="hidden space-y-4">

            <!-- HUD / PANEL STATUS ATAS -->
            <div class="bg-white/95 border-2 border-[#D8C3A5] rounded-2xl p-3 sm:p-4 shadow-sm">
                <div class="grid grid-cols-2 sm:grid-cols-4 gap-3 items-center">
                    <!-- Skor -->
                    <div class="bg-[#FAF6EE] border border-[#E6D5BE] rounded-xl px-3 py-2">
                        <span class="text-[11px] font-bold uppercase tracking-wider text-[#7A5236] block">Skor</span>
                        <span id="hud-score" class="font-display font-bold text-xl sm:text-2xl text-[#362216]">0</span>
                    </div>

                    <!-- Kombo / Streak -->
                    <div class="bg-[#FAF6EE] border border-[#E6D5BE] rounded-xl px-3 py-2">
                        <span class="text-[11px] font-bold uppercase tracking-wider text-[#7A5236] block">Kombo (Streak)</span>
                        <span id="hud-streak" class="font-display font-bold text-xl sm:text-2xl text-amber-600">0x 🔥</span>
                    </div>

                    <!-- Nyawa / Ketelitian -->
                    <div class="bg-[#FAF6EE] border border-[#E6D5BE] rounded-xl px-3 py-2">
                        <span class="text-[11px] font-bold uppercase tracking-wider text-[#7A5236] block">Ketelitian</span>
                        <div id="hud-lives" class="text-lg sm:text-xl leading-tight mt-0.5">❤️❤️❤️</div>
                    </div>

                    <!-- Timer -->
                    <div class="bg-[#FAF6EE] border border-[#E6D5BE] rounded-xl px-3 py-2">
                        <div class="flex items-center justify-between mb-1">
                            <span class="text-[11px] font-bold uppercase tracking-wider text-[#7A5236]">Waktu</span>
                            <span id="hud-time-text" class="font-display font-bold text-base sm:text-lg text-[#3A5A40]">90d</span>
                        </div>
                        <div class="w-full h-2.5 bg-[#E6D5BE] rounded-full overflow-hidden">
                            <div id="hud-time-bar" class="h-full bg-[#588157] transition-all duration-300 rounded-full" style="width: 100%;"></div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- BANNER TANTANGAN PENGUNJUNG BERTANYA -->
            <div id="visitor-banner" class="hidden bg-amber-100 border-2 border-amber-500 rounded-2xl p-3.5 sm:p-4 shadow-md animate-pop-in">
                <div class="flex flex-col sm:flex-row sm:items-center justify-between gap-2.5">
                    <div class="flex items-center gap-3">
                        <span id="visitor-avatar" class="text-3xl bg-white w-12 h-12 rounded-2xl flex items-center justify-center border border-amber-300 shrink-0">🙋‍♂️</span>
                        <div>
                            <span class="inline-block text-[10px] font-extrabold uppercase tracking-wider bg-amber-600 text-white px-2 py-0.5 rounded-full mb-0.5">
                                Pengunjung Bertanya! (Klik Rak Tujuan)
                            </span>
                            <p id="visitor-question" class="font-bold text-sm sm:text-base text-[#362216]"></p>
                        </div>
                    </div>
                    <span class="text-xs font-bold text-amber-900 bg-amber-200/80 px-3 py-1.5 rounded-xl self-start sm:self-center shrink-0">
                        Bonus +150 Poin &amp; +5d
                    </span>
                </div>
            </div>

            <!-- AREA KERJA UTAMA: MEJA BUKU (KIRI) & RAK PERPUSTAKAAN (KANAN) -->
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-4 items-start">

                <!-- MEJA SORTIR BUKU -->
                <div class="lg:col-span-5 bg-[#F2E8D5] border-4 border-[#B68D65] rounded-3xl p-4 sm:p-5 shadow-md space-y-3.5">
                    <div class="flex items-center justify-between gap-2">
                        <div>
                            <h2 class="font-display font-bold text-lg text-[#362216] flex items-center gap-1.5">
                                <span>🪑</span>
                                <span>Meja Sortir Buku</span>
                            </h2>
                            <p class="text-xs text-[#6B4C35]">Seret ke rak atau klik salah satu rak di samping</p>
                        </div>
                        <div class="text-right">
                            <span class="text-[11px] font-bold text-[#7A5236] block">Antrean</span>
                            <span id="desk-queue-count" class="font-display font-bold text-sm text-[#362216]">1 / 5</span>
                        </div>
                    </div>

                    <!-- Indikator Antrean -->
                    <div id="desk-queue-dots" class="flex items-center gap-1.5"></div>

                    <!-- Wadah Kartu Buku Aktif -->
                    <div id="active-book-container" class="min-h-[210px] flex items-center justify-center">
                        <!-- Diisi secara dinamis oleh JavaScript -->
                    </div>

                    <!-- Tombol Selesai Lebih Awal -->
                    <div class="pt-1 flex items-center justify-between text-xs text-[#6B4C35]">
                        <span>Tips: Cek kode DDC &amp; kondisi sampul</span>
                        <button
                            id="btn-finish-early"
                            type="button"
                            class="font-bold text-[#7A5236] hover:text-[#362216] underline cursor-pointer"
                        >
                            Selesai &amp; Lihat Rekap
                        </button>
                    </div>
                </div>

                <!-- RAK KLASIFIKASI DDC & KERANJANG PERBAIKAN -->
                <div class="lg:col-span-7 bg-white/90 border-4 border-[#D8C3A5] rounded-3xl p-4 sm:p-5 shadow-md space-y-3">
                    <div class="flex items-center justify-between">
                        <h2 class="font-display font-bold text-lg text-[#362216] flex items-center gap-1.5">
                            <span>🗄️</span>
                            <span>Rak Perpustakaan &amp; Perbaikan</span>
                        </h2>
                        <span class="text-xs font-semibold text-[#5C3D28] bg-[#FAF6EE] px-2.5 py-1 rounded-full border border-[#E2D0B6]">
                            Klik atau Lepas Buku di Sini
                        </span>
                    </div>

                    <div id="shelves-grid" class="grid grid-cols-1 sm:grid-cols-2 gap-3">
                        <!-- Diisi secara dinamis oleh JavaScript -->
                    </div>
                </div>
            </div>
        </section>

        <!-- =========================================================
             LAYAR 3: RINGKASAN AKHIR & REKAP JAWABAN
             ========================================================= -->
        <section id="screen-end" class="hidden my-auto py-2 animate-pop-in">
            <div class="bg-white/95 border-4 border-[#D8C3A5] rounded-3xl p-5 sm:p-8 shadow-xl max-w-4xl mx-auto">
                <!-- Header Peringkat -->
                <div class="text-center mb-6">
                    <div id="end-badge-icon" class="w-16 h-16 mx-auto mb-2 rounded-3xl bg-amber-100 border-2 border-amber-400 flex items-center justify-center text-4xl shadow-xs">
                        🏆
                    </div>
                    <h2 id="end-rank-title" class="font-display font-bold text-2xl sm:text-4xl text-[#362216]">
                        Pustakawan Andal ⭐
                    </h2>
                    <p id="end-reason" class="text-xs sm:text-sm text-[#6B4C35] mt-1"></p>
                </div>

                <!-- 4 Kartu Metrik Utama -->
                <div class="grid grid-cols-2 sm:grid-cols-4 gap-3 mb-5">
                    <div class="bg-[#FAF6EE] border-2 border-[#E6D5BE] rounded-2xl p-3.5 text-center">
                        <span class="text-[11px] font-bold uppercase tracking-wider text-[#7A5236] block">Skor Akhir</span>
                        <span id="end-score" class="font-display font-bold text-2xl sm:text-3xl text-[#3A5A40]">0</span>
                    </div>
                    <div class="bg-[#FAF6EE] border-2 border-[#E6D5BE] rounded-2xl p-3.5 text-center">
                        <span class="text-[11px] font-bold uppercase tracking-wider text-[#7A5236] block">Akurasi</span>
                        <span id="end-accuracy" class="font-display font-bold text-2xl sm:text-3xl text-sky-700">0%</span>
                    </div>
                    <div class="bg-[#FAF6EE] border-2 border-[#E6D5BE] rounded-2xl p-3.5 text-center">
                        <span class="text-[11px] font-bold uppercase tracking-wider text-[#7A5236] block">Kombo Terbaik</span>
                        <span id="end-max-streak" class="font-display font-bold text-2xl sm:text-3xl text-amber-600">0x</span>
                    </div>
                    <div class="bg-[#FAF6EE] border-2 border-[#E6D5BE] rounded-2xl p-3.5 text-center">
                        <span class="text-[11px] font-bold uppercase tracking-wider text-[#7A5236] block">Buku Tersusun</span>
                        <span id="end-sorted" class="font-display font-bold text-2xl sm:text-3xl text-[#362216]">0</span>
                    </div>
                </div>

                <!-- Kotak Fakta Literasi -->
                <div class="bg-[#E9EDC9]/75 border-2 border-[#A3B18A] rounded-2xl p-4 mb-5 flex items-start gap-3">
                    <span class="text-2xl shrink-0 mt-0.5">💡</span>
                    <div>
                        <h3 class="font-display font-bold text-sm sm:text-base text-[#283E2C] mb-0.5">
                            Tahukah Kamu? (Fakta Literasi &amp; Perpustakaan)
                        </h3>
                        <p id="end-fun-fact" class="text-xs sm:text-sm text-[#3A5A40] leading-relaxed"></p>
                    </div>
                </div>

                <!-- Navigasi Tab: Ringkasan vs Rekap Jawaban -->
                <div class="flex flex-wrap items-center justify-center gap-2 mb-4">
                    <button
                        type="button"
                        id="tab-summary"
                        class="px-4 py-2 rounded-xl text-xs sm:text-sm font-bold bg-[#588157] text-white shadow-xs transition cursor-pointer"
                    >
                        📊 Ringkasan Sesi
                    </button>
                    <button
                        type="button"
                        id="tab-recap"
                        class="px-4 py-2 rounded-xl text-xs sm:text-sm font-bold bg-[#F2E8D5] text-[#4A3222] border border-[#A67B5B]/50 hover:bg-[#E5D8C1] transition cursor-pointer"
                    >
                        📋 Rekap Jawaban (<span id="recap-count-badge">0</span>)
                    </button>
                </div>

                <!-- Panel Ringkasan Singkat -->
                <div id="panel-summary" class="bg-[#FAF6EE] border border-[#E2D0B6] rounded-2xl p-4 mb-6 text-xs sm:text-sm text-[#5C3D28] space-y-2">
                    <p id="summary-detail-text" class="leading-relaxed"></p>
                    <p class="text-xs text-[#7A5236]">
                        Buka tab <strong>Rekap Jawaban</strong> untuk melihat rincian tiap buku atau pertanyaan pengunjung beserta alasan DDC/kondisi bukunya, menyalin ringkasan, atau mengunduh berkas <code>.txt</code>.
                    </p>
                </div>

                <!-- Panel Rekap Jawaban (Tersembunyi sampai tab diklik) -->
                <div id="panel-recap" class="hidden bg-[#F2E8D5]/75 border-2 border-[#D4C5B0] rounded-2xl p-4 mb-6 space-y-3">
                    <div class="flex flex-col sm:flex-row sm:items-center justify-between gap-2.5">
                        <!-- Filter Semua / Benar / Salah -->
                        <div class="flex flex-wrap items-center gap-1.5">
                            <button
                                type="button"
                                data-filter="all"
                                class="recap-filter-btn px-3 py-1.5 rounded-lg text-xs font-bold bg-[#4A3222] text-white cursor-pointer"
                            >
                                Semua (<span id="recap-all-count">0</span>)
                            </button>
                            <button
                                type="button"
                                data-filter="correct"
                                class="recap-filter-btn px-3 py-1.5 rounded-lg text-xs font-bold bg-white text-emerald-800 border border-emerald-400 cursor-pointer"
                            >
                                Benar (<span id="recap-correct-count">0</span>)
                            </button>
                            <button
                                type="button"
                                data-filter="wrong"
                                class="recap-filter-btn px-3 py-1.5 rounded-lg text-xs font-bold bg-white text-red-800 border border-red-400 cursor-pointer"
                            >
                                Salah (<span id="recap-wrong-count">0</span>)
                            </button>
                        </div>

                        <!-- Tombol Salin & Unduh (.txt) -->
                        <div class="flex items-center gap-2">
                            <button
                                type="button"
                                id="btn-copy-recap"
                                class="px-3 py-1.5 rounded-xl text-xs font-bold bg-white hover:bg-[#FAF6EE] text-[#4A3222] border border-[#A67B5B] transition cursor-pointer"
                            >
                                📋 Salin Rekap
                            </button>
                            <button
                                type="button"
                                id="btn-download-recap"
                                class="px-3 py-1.5 rounded-xl text-xs font-bold bg-[#3A5A40] hover:bg-[#283E2C] text-white transition cursor-pointer"
                            >
                                ⬇️ Unduh (.txt)
                            </button>
                        </div>
                    </div>

                    <!-- Pesan Notifikasi Aksi (Salin / Unduh) -->
                    <div id="recap-action-feedback" class="hidden text-xs font-bold text-[#283E2C] bg-[#E9EDC9] px-3 py-2 rounded-xl border border-[#A3B18A]"></div>

                    <!-- Daftar Item Riwayat -->
                    <div id="recap-list" class="space-y-2.5 max-h-72 overflow-y-auto pr-1"></div>
                </div>

                <!-- Tombol Aksi Utama -->
                <div class="flex flex-col sm:flex-row gap-3 justify-center">
                    <button
                        id="btn-play-again"
                        type="button"
                        class="btn-primary px-8 py-3.5 rounded-2xl text-white font-display font-bold text-lg cursor-pointer"
                    >
                        🔄 Main Lagi
                    </button>
                    <button
                        id="btn-back-home"
                        type="button"
                        class="bg-[#F2E8D5] hover:bg-[#E5D8C1] text-[#4A3222] border-2 border-[#A67B5B] px-6 py-3.5 rounded-2xl font-display font-bold text-lg transition cursor-pointer"
                    >
                        🏠 Menu Utama
                    </button>
                </div>
            </div>
        </section>

    </main>

    <!-- =========================================================
         MODAL 1: PEMBAHASAN INSTAN SAAT JAWABAN SALAH
         ========================================================= -->
    <div id="modal-explanation" class="hidden fixed inset-0 bg-black/65 backdrop-blur-xs z-50 flex items-center justify-center p-4">
        <div class="bg-[#FAF6EE] border-4 border-amber-500 rounded-3xl max-w-md w-full p-5 sm:p-6 shadow-2xl animate-pop-in">
            <div class="flex items-center gap-3 mb-3">
                <div class="w-11 h-11 rounded-2xl bg-amber-100 border border-amber-400 flex items-center justify-center text-2xl shrink-0">
                    💡
                </div>
                <div>
                    <span class="text-[11px] font-extrabold uppercase tracking-wider text-amber-800 block">
                        Pembahasan Instan (Waktu Dijeda)
                    </span>
                    <h3 id="explain-modal-title" class="font-display font-bold text-lg text-[#362216]">
                        Mari Cek Rak yang Tepat!
                    </h3>
                </div>
            </div>

            <div class="bg-white border border-[#E2D0B6] rounded-2xl p-3.5 mb-3 text-xs sm:text-sm space-y-1.5">
                <p id="explain-item-label" class="font-bold text-[#362216]"></p>
                <p id="explain-user-choice" class="text-red-700 font-semibold"></p>
                <p id="explain-correct-answer" class="text-emerald-800 font-bold"></p>
            </div>

            <div class="bg-[#E9EDC9]/70 border border-[#A3B18A] rounded-2xl p-3.5 mb-4 text-xs sm:text-sm text-[#283E2C] leading-relaxed">
                <strong>Alasan:</strong> <span id="explain-reason"></span>
            </div>

            <button
                id="btn-continue-after-explain"
                type="button"
                class="btn-primary w-full py-3 rounded-xl text-white font-display font-bold text-base cursor-pointer"
            >
                Lanjutkan Bertugas ➡️
            </button>
        </div>
    </div>

    <!-- =========================================================
         MODAL 2: PANDUAN KODE DDC & PERAWATAN BUKU
         ========================================================= -->
    <div id="modal-guide" class="hidden fixed inset-0 bg-black/60 backdrop-blur-xs z-50 flex items-center justify-center p-4">
        <div class="bg-[#FAF6EE] border-4 border-[#588157] rounded-3xl max-w-xl w-full max-h-[88vh] flex flex-col shadow-2xl animate-pop-in overflow-hidden">
            <div class="bg-[#3A5A40] text-white px-5 py-4 flex items-center justify-between">
                <div class="flex items-center gap-2">
                    <span class="text-2xl">📖</span>
                    <h3 class="font-display font-bold text-lg sm:text-xl">Panduan Singkat DDC &amp; Perawatan</h3>
                </div>
                <button
                    id="btn-close-guide"
                    type="button"
                    aria-label="Tutup panduan"
                    class="w-8 h-8 rounded-full bg-white/15 hover:bg-white/25 flex items-center justify-center font-bold cursor-pointer"
                >
                    ✕
                </button>
            </div>

            <div class="p-4 sm:p-5 overflow-y-auto space-y-2.5 text-xs sm:text-sm">
                <div class="bg-emerald-50 border border-emerald-300 rounded-2xl p-3">
                    <p class="font-bold text-emerald-950">🔬 500 — Sains &amp; Alam</p>
                    <p class="text-emerald-900">Matematika, astronomi/tata surya, fisika, kimia, biologi, hewan &amp; tumbuhan.</p>
                </div>
                <div class="bg-sky-50 border border-sky-300 rounded-2xl p-3">
                    <p class="font-bold text-sky-950">💻 600 — Teknologi</p>
                    <p class="text-sky-900">Kesehatan &amp; kedokteran, komputer/robotika, mesin, pertanian, serta rekayasa.</p>
                </div>
                <div class="bg-purple-50 border border-purple-300 rounded-2xl p-3">
                    <p class="font-bold text-purple-950">🎨 700 — Seni &amp; Musik</p>
                    <p class="text-purple-900">Melukis, origami/kriya, fotografi, alat musik, lagu, dan olahraga/permainan.</p>
                </div>
                <div class="bg-rose-50 border border-rose-300 rounded-2xl p-3">
                    <p class="font-bold text-rose-950">🐉 800 — Sastra &amp; Fiksi</p>
                    <p class="text-rose-900">Dongeng, cerita fantasi/petualangan, novel remaja, fabel, puisi, dan drama.</p>
                </div>
                <div class="bg-amber-50 border border-amber-300 rounded-2xl p-3">
                    <p class="font-bold text-amber-950">🏛️ 900 — Sejarah &amp; Geografi</p>
                    <p class="text-amber-950">Sejarah perjuangan/peradaban, biografi tokoh, atlas/peta, dan catatan perjalanan.</p>
                </div>
                <div class="bg-orange-50 border-2 border-dashed border-orange-500 rounded-2xl p-3">
                    <p class="font-bold text-orange-950">🩹 Keranjang Perbaikan (Buku Rusak)</p>
                    <p class="text-orange-900">Buku dengan sampul sobek, halaman lepas, atau noda cairan harus dipisahkan ke sini sebelum dipajang kembali.</p>
                </div>
            </div>

            <div class="px-5 py-3.5 bg-[#F2E8D5] border-t border-[#D8C3A5] flex justify-end">
                <button
                    id="btn-close-guide-bottom"
                    type="button"
                    class="btn-primary px-6 py-2.5 rounded-xl text-white font-display font-bold text-sm cursor-pointer"
                >
                    Siap, Mengerti!
                </button>
            </div>
        </div>
    </div>

    <script>
        /**
         * =====================================================================
         * 1. EFEK SUARA SINTETIS (WEB AUDIO API) — TANPA FILE EKSTERNAL
         * =====================================================================
         */
        class SoundEffects {
            constructor() {
                this.ctx = null;
                this.muted = false;
            }

            init() {
                try {
                    if (!this.ctx) {
                        const AudioCtx = window.AudioContext || window.webkitAudioContext;
                        if (AudioCtx) {
                            this.ctx = new AudioCtx();
                        }
                    }
                    if (this.ctx && this.ctx.state === 'suspended') {
                        this.ctx.resume();
                    }
                } catch (_) {
                    // Abaikan jika browser membatasi audio
                }
            }

            toggleMute() {
                this.muted = !this.muted;
                if (!this.muted) this.init();
                return this.muted;
            }

            playTone(freq, duration, type = 'sine', delay = 0, gainVal = 0.12) {
                if (this.muted) return;
                this.init();
                if (!this.ctx) return;

                try {
                    const now = this.ctx.currentTime + delay;
                    const osc = this.ctx.createOscillator();
                    const gain = this.ctx.createGain();
                    osc.type = type;
                    osc.frequency.setValueAtTime(freq, now);

                    gain.gain.setValueAtTime(0.0001, now);
                    gain.gain.exponentialRampToValueAtTime(gainVal, now + 0.015);
                    gain.gain.exponentialRampToValueAtTime(0.0001, now + duration);

                    osc.connect(gain);
                    gain.connect(this.ctx.destination);
                    osc.start(now);
                    osc.stop(now + duration + 0.02);
                } catch (_) {
                    // Aman jika terjadi error konteks audio
                }
            }

            playCorrect(streak = 1) {
                const pitchBoost = Math.min(streak * 22, 180);
                this.playTone(523.25 + pitchBoost, 0.12, 'triangle', 0, 0.13);
                this.playTone(659.25 + pitchBoost, 0.16, 'triangle', 0.08, 0.13);
            }

            playWrong() {
                this.playTone(230, 0.16, 'sawtooth', 0, 0.11);
                this.playTone(170, 0.22, 'sawtooth', 0.11, 0.11);
            }

            playVisitor() {
                this.playTone(587.33, 0.11, 'sine', 0, 0.12);
                this.playTone(880.00, 0.18, 'sine', 0.09, 0.12);
            }

            playGameOver() {
                this.playTone(523.25, 0.15, 'triangle', 0, 0.12);
                this.playTone(440.00, 0.15, 'triangle', 0.14, 0.12);
                this.playTone(392.00, 0.28, 'triangle', 0.28, 0.12);
            }
        }

        const sfx = new SoundEffects();

        /**
         * =====================================================================
         * 2. DATA RAK DDC, BANK BUKU, PERTANYAAN PENGUNJUNG & FAKTA LITERASI
         * =====================================================================
         */
        const SHELVES = [
            {
                id: 'sains',
                code: 'DDC 500',
                name: 'Sains & Alam',
                icon: '🔬',
                cardClass: 'bg-emerald-50 border-emerald-500 text-emerald-950',
                badgeClass: 'bg-emerald-700 text-white',
                reason: 'Kelas DDC 500 mencakup ilmu pengetahuan alam murni seperti matematika, astronomi, fisika, kimia, dan biologi/makhluk hidup.'
            },
            {
                id: 'teknologi',
                code: 'DDC 600',
                name: 'Teknologi',
                icon: '💻',
                cardClass: 'bg-sky-50 border-sky-500 text-sky-950',
                badgeClass: 'bg-sky-700 text-white',
                reason: 'Kelas DDC 600 mencakup ilmu terapan dan teknologi seperti kesehatan, komputer, robotika, pertanian, serta rekayasa.'
            },
            {
                id: 'seni',
                code: 'DDC 700',
                name: 'Seni & Musik',
                icon: '🎨',
                cardClass: 'bg-purple-50 border-purple-500 text-purple-950',
                badgeClass: 'bg-purple-700 text-white',
                reason: 'Kelas DDC 700 mencakup seni rupa, kriya/origami, musik, fotografi, serta permainan dan olahraga.'
            },
            {
                id: 'fiksi',
                code: 'DDC 800',
                name: 'Sastra & Fiksi',
                icon: '🐉',
                cardClass: 'bg-rose-50 border-rose-500 text-rose-950',
                badgeClass: 'bg-rose-700 text-white',
                reason: 'Kelas DDC 800 mencakup karya sastra dan cerita rekaan/fiksi seperti dongeng, petualangan fantasi, fabel, puisi, dan cerita rakyat.'
            },
            {
                id: 'sejarah',
                code: 'DDC 900',
                name: 'Sejarah',
                icon: '🏛️',
                cardClass: 'bg-amber-50 border-amber-500 text-amber-950',
                badgeClass: 'bg-amber-700 text-white',
                reason: 'Kelas DDC 900 mencakup sejarah, biografi tokoh, geografi, peta/atlas, serta catatan perjalanan.'
            },
            {
                id: 'perbaikan',
                code: 'RAWAT',
                name: 'Keranjang Perbaikan',
                icon: '🩹',
                cardClass: 'bg-orange-50 border-dashed border-orange-500 text-orange-950',
                badgeClass: 'bg-orange-600 text-white',
                reason: 'Buku yang sampulnya sobek, halamannya terlepas, atau terkena noda harus dipisahkan ke Keranjang Perbaikan sebelum dikembalikan ke rak.'
            }
        ];

        const BOOK_CATALOG = [
            // 500 Sains
            { title: 'Rahasia Tata Surya & Planet', ddc: '523', shelf: 'sains', emoji: '🪐', spine: '#059669' },
            { title: 'Daur Hidup Kupu-Kupu', ddc: '595', shelf: 'sains', emoji: '🦋', spine: '#10B981' },
            { title: 'Eksperimen Cahaya & Pelangi', ddc: '535', shelf: 'sains', emoji: '🌈', spine: '#047857' },
            { title: 'Pecahan & Pola Bilangan', ddc: '513', shelf: 'sains', emoji: '📐', spine: '#0D9488' },
            { title: 'Mengenal Sel & Fotosintesis', ddc: '581', shelf: 'sains', emoji: '🌿', spine: '#15803D' },

            // 600 Teknologi
            { title: 'Dasar Pemrograman & Komputer', ddc: '621', shelf: 'teknologi', emoji: '💻', spine: '#0284C7' },
            { title: 'Menjaga Kesehatan Gigi & Tubuh', ddc: '613', shelf: 'teknologi', emoji: '🩺', spine: '#0369A1' },
            { title: 'Merakit Robot Sederhana', ddc: '629', shelf: 'teknologi', emoji: '🤖', spine: '#0EA5E9' },
            { title: 'Bercocok Tanam Hidroponik', ddc: '635', shelf: 'teknologi', emoji: '🌱', spine: '#2563EB' },

            // 700 Seni
            { title: 'Seni Melipat Kertas Origami', ddc: '736', shelf: 'seni', emoji: '🦢', spine: '#9333EA' },
            { title: 'Belajar Notasi & Gitar Akustik', ddc: '787', shelf: 'seni', emoji: '🎸', spine: '#7E22CE' },
            { title: 'Teknik Mewarnai Cat Air', ddc: '751', shelf: 'seni', emoji: '🖌️', spine: '#A855F7' },
            { title: 'Panduan Dasar Fotografi Alam', ddc: '771', shelf: 'seni', emoji: '📷', spine: '#6D28D9' },

            // 800 Sastra & Fiksi
            { title: 'Naga Kecil di Lembah Awan', ddc: '899', shelf: 'fiksi', emoji: '🐉', spine: '#E11D48' },
            { title: 'Kancil & Musim Kemarau', ddc: '899', shelf: 'fiksi', emoji: '🦊', spine: '#BE123C' },
            { title: 'Kumpulan Puisi Hujan Sore', ddc: '899', shelf: 'fiksi', emoji: '☔', spine: '#F43F5E' },
            { title: 'Petualangan Kunci Jam Tua', ddc: '899', shelf: 'fiksi', emoji: '🗝️', spine: '#9F1239' },

            // 900 Sejarah
            { title: 'Jejak Kemerdekaan Nusantara', ddc: '959', shelf: 'sejarah', emoji: '🏛️', spine: '#D97706' },
            { title: 'Atlas Kepulauan & Benua', ddc: '912', shelf: 'sejarah', emoji: '🗺️', spine: '#B45309' },
            { title: 'Biografi Tokoh Penjelajah', ddc: '920', shelf: 'sejarah', emoji: '🧭', spine: '#F59E0B' },
            { title: 'Peradaban Kuno Lembah Sungai', ddc: '930', shelf: 'sejarah', emoji: '🏺', spine: '#92400E' }
        ];

        const DAMAGE_REASONS = [
            'Sampul depan sobek',
            'Beberapa halaman lepas',
            'Terkena noda minuman'
        ];

        const VISITOR_QUESTIONS = [
            {
                avatar: '👧',
                text: '"Kak, di mana rak buku tentang planet, bintang, dan daur air ya?"',
                target: 'sains'
            },
            {
                avatar: '👦',
                text: '"Permisi, saya mau cari buku tentang komputer dan cara merawat kesehatan."',
                target: 'teknologi'
            },
            {
                avatar: '👩‍🎨',
                text: '"Halo pustakawan! Rak untuk buku origami, lukisan, dan musik di sebelah mana?"',
                target: 'seni'
            },
            {
                avatar: '🧒',
                text: '"Kak, saya mencari cerita dongeng dan fiksi petualangan yang seru!"',
                target: 'fiksi'
            },
            {
                avatar: '👨‍🏫',
                text: '"Selamat bertugas! Saya butuh buku sejarah perjuangan dan peta/atlas."',
                target: 'sejarah'
            }
        ];

        const LITERACY_FACTS = [
            'Sistem Klasifikasi Desimal Dewey (DDC) dirancang oleh Melvil Dewey pada tahun 1876 dan membagi ilmu pengetahuan menjadi 10 kelas utama (000–999).',
            'Memisahkan buku yang sampulnya sobek atau halamannya lepas ke keranjang perbaikan membantu menjaga koleksi tetap awet dan bisa dibaca banyak orang.',
            'Membaca rutin 15–20 menit setiap hari membantu memperkaya kosakata, melatih fokus, dan menumbuhkan empati.',
            'Nomor panggil (call number) di punggung buku memudahkan pustakawan dan pembaca menemukan buku di rak secara tertib.'
        ];

        const DIFFICULTY_CONFIG = {
            easy: { duration: 90, spawnInterval: 3800, visitorInterval: 13500, damageChance: 0.22, maxQueue: 5 },
            medium: { duration: 75, spawnInterval: 3100, visitorInterval: 11500, damageChance: 0.28, maxQueue: 5 },
            hard: { duration: 60, spawnInterval: 2500, visitorInterval: 9500, damageChance: 0.34, maxQueue: 5 }
        };

        /**
         * =====================================================================
         * 3. STATE APLIKASI & REFERENSI DOM
         * =====================================================================
         */
        const state = {
            difficulty: 'easy',
            isPlaying: false,
            isPausedForExplanation: false,
            instantExplanation: true,
            recapFilter: 'all',
            score: 0,
            streak: 0,
            maxStreak: 0,
            sortedCount: 0,
            correctActions: 0,
            wrongActions: 0,
            lives: 3,
            timeLeft: 90,
            maxTime: 90,
            bookQueue: [],
            activeVisitor: null,
            history: [],
            pendingEndReason: null,
            timers: {
                clock: null,
                spawner: null,
                visitor: null
            }
        };

        const dom = {
            screenStart: document.getElementById('screen-start'),
            screenGame: document.getElementById('screen-game'),
            screenEnd: document.getElementById('screen-end'),

            hudScore: document.getElementById('hud-score'),
            hudStreak: document.getElementById('hud-streak'),
            hudLives: document.getElementById('hud-lives'),
            hudTimeText: document.getElementById('hud-time-text'),
            hudTimeBar: document.getElementById('hud-time-bar'),

            visitorBanner: document.getElementById('visitor-banner'),
            visitorAvatar: document.getElementById('visitor-avatar'),
            visitorQuestion: document.getElementById('visitor-question'),

            deskQueueCount: document.getElementById('desk-queue-count'),
            deskQueueDots: document.getElementById('desk-queue-dots'),
            activeBookContainer: document.getElementById('active-book-container'),
            shelvesGrid: document.getElementById('shelves-grid'),

            explainStatus: document.getElementById('explain-status'),
            modalExplanation: document.getElementById('modal-explanation'),
            explainModalTitle: document.getElementById('explain-modal-title'),
            explainItemLabel: document.getElementById('explain-item-label'),
            explainUserChoice: document.getElementById('explain-user-choice'),
            explainCorrectAnswer: document.getElementById('explain-correct-answer'),
            explainReason: document.getElementById('explain-reason'),

            modalGuide: document.getElementById('modal-guide'),

            endBadgeIcon: document.getElementById('end-badge-icon'),
            endRankTitle: document.getElementById('end-rank-title'),
            endReason: document.getElementById('end-reason'),
            endScore: document.getElementById('end-score'),
            endAccuracy: document.getElementById('end-accuracy'),
            endMaxStreak: document.getElementById('end-max-streak'),
            endSorted: document.getElementById('end-sorted'),
            endFunFact: document.getElementById('end-fun-fact'),
            summaryDetailText: document.getElementById('summary-detail-text'),

            tabSummary: document.getElementById('tab-summary'),
            tabRecap: document.getElementById('tab-recap'),
            panelSummary: document.getElementById('panel-summary'),
            panelRecap: document.getElementById('panel-recap'),
            recapCountBadge: document.getElementById('recap-count-badge'),
            recapAllCount: document.getElementById('recap-all-count'),
            recapCorrectCount: document.getElementById('recap-correct-count'),
            recapWrongCount: document.getElementById('recap-wrong-count'),
            recapList: document.getElementById('recap-list'),
            recapActionFeedback: document.getElementById('recap-action-feedback')
        };

        /**
         * =====================================================================
         * 4. FUNGSI BANTUAN & MANAJEMEN LAYAR
         * =====================================================================
         */
        function getShelfById(id) {
            return SHELVES.find(s => s.id === id) || { id, code: id.toUpperCase(), name: id, reason: '' };
        }

        function switchScreen(target) {
            dom.screenStart.classList.add('hidden');
            dom.screenGame.classList.add('hidden');
            dom.screenEnd.classList.add('hidden');

            if (target === 'start') dom.screenStart.classList.remove('hidden');
            else if (target === 'game') dom.screenGame.classList.remove('hidden');
            else if (target === 'end') dom.screenEnd.classList.remove('hidden');
        }

        function clearAllTimers() {
            clearInterval(state.timers.clock);
            clearInterval(state.timers.spawner);
            clearInterval(state.timers.visitor);
            state.timers.clock = null;
            state.timers.spawner = null;
            state.timers.visitor = null;
        }

        function showFloatingText(text, x, y, color = '#15803D') {
            const el = document.createElement('div');
            el.className = 'floating-feedback';
            el.style.left = `${x}px`;
            el.style.top = `${y}px`;
            el.style.color = color;
            el.textContent = text;
            document.body.appendChild(el);
            setTimeout(() => el.remove(), 1080);
        }

        function createRandomBook() {
            const cfg = DIFFICULTY_CONFIG[state.difficulty];
            const base = BOOK_CATALOG[Math.floor(Math.random() * BOOK_CATALOG.length)];
            const isDamaged = Math.random() < cfg.damageChance;
            const damageReason = isDamaged
                ? DAMAGE_REASONS[Math.floor(Math.random() * DAMAGE_REASONS.length)]
                : null;

            return {
                uid: `${Date.now()}-${Math.random().toString(36).slice(2, 7)}`,
                title: base.title,
                ddc: base.ddc,
                categoryShelf: base.shelf,
                targetShelf: isDamaged ? 'perbaikan' : base.shelf,
                emoji: base.emoji,
                spine: base.spine,
                isDamaged,
                damageReason
            };
        }

        function recordAction(entry) {
            state.history.push({
                id: `${Date.now()}-${Math.random().toString(36).slice(2, 6)}`,
                time: new Date().toLocaleTimeString('id-ID', { hour: '2-digit', minute: '2-digit', second: '2-digit' }),
                ...entry
            });
            if (entry.isCorrect) state.correctActions++;
            else state.wrongActions++;
        }

        /**
         * =====================================================================
         * 5. RENDERING HUD, KARTU BUKU & RAK
         * =====================================================================
         */
        function updateHUD() {
            dom.hudScore.textContent = state.score;
            dom.hudStreak.textContent = `${state.streak}x 🔥`;
            dom.hudLives.textContent = '❤️'.repeat(Math.max(0, state.lives)) + '🖤'.repeat(Math.max(0, 3 - state.lives));

            const safeTime = Math.max(0, state.timeLeft);
            dom.hudTimeText.textContent = `${safeTime}d`;

            const pct = Math.max(0, Math.min(100, (safeTime / state.maxTime) * 100));
            dom.hudTimeBar.style.width = `${pct}%`;

            if (pct <= 25) {
                dom.hudTimeBar.className = 'h-full bg-red-600 transition-all duration-300 rounded-full';
                dom.hudTimeText.className = 'font-display font-bold text-base sm:text-lg text-red-600';
            } else if (pct <= 50) {
                dom.hudTimeBar.className = 'h-full bg-amber-500 transition-all duration-300 rounded-full';
                dom.hudTimeText.className = 'font-display font-bold text-base sm:text-lg text-amber-600';
            } else {
                dom.hudTimeBar.className = 'h-full bg-[#588157] transition-all duration-300 rounded-full';
                dom.hudTimeText.className = 'font-display font-bold text-base sm:text-lg text-[#3A5A40]';
            }

            const maxQ = DIFFICULTY_CONFIG[state.difficulty].maxQueue;
            const currentQ = state.bookQueue.length;
            dom.deskQueueCount.textContent = `${currentQ} / ${maxQ}`;

            let dotsHtml = '';
            for (let i = 0; i < maxQ; i++) {
                if (i < currentQ) {
                    dotsHtml += `<span class="h-2.5 flex-1 rounded-full ${i === 0 ? 'bg-[#3A5A40]' : 'bg-[#A3B18A]'}"></span>`;
                } else {
                    dotsHtml += `<span class="h-2.5 flex-1 rounded-full bg-[#E2D0B6]"></span>`;
                }
            }
            dom.deskQueueDots.innerHTML = dotsHtml;
        }

        function renderActiveBook() {
            if (state.bookQueue.length === 0) {
                dom.activeBookContainer.innerHTML = `
                    <div class="text-center text-sm text-[#7A5236] py-6">
                        Menyiapkan buku berikutnya...
                    </div>
                `;
                return;
            }

            const book = state.bookQueue[0];
            const damageBadge = book.isDamaged
                ? `<div class="mt-2 inline-flex items-center gap-1.5 bg-orange-100 border border-orange-500 text-orange-900 text-xs font-extrabold px-2.5 py-1 rounded-full">
                       <span>🩹</span>
                       <span>RUSAK: ${book.damageReason}</span>
                   </div>`
                : `<div class="mt-2 inline-flex items-center gap-1.5 bg-[#FAF6EE] border border-[#DFCBB0] text-[#5C3D28] text-xs font-bold px-2.5 py-1 rounded-full">
                       <span>🏷️</span>
                       <span>Kode DDC: ${book.ddc}</span>
                   </div>`;

            dom.activeBookContainer.innerHTML = `
                <div
                    id="active-book-card"
                    draggable="true"
                    class="w-full bg-white border-2 border-[#C8AE8C] rounded-2xl p-4 shadow-md animate-pop-in cursor-grab active:cursor-grabbing select-none"
                >
                    <div class="flex items-start gap-3.5">
                        <!-- Ilustrasi Punggung Buku -->
                        <div
                            class="w-16 h-24 sm:w-20 sm:h-28 rounded-xl flex flex-col items-center justify-between p-2 text-white shadow-inner shrink-0 border-l-4 border-black/20"
                            style="background-color: ${book.spine};"
                        >
                            <span class="text-[10px] font-extrabold bg-black/25 px-1.5 py-0.5 rounded-md tracking-wider">
                                ${book.ddc}
                            </span>
                            <span class="text-2xl sm:text-3xl">${book.emoji}</span>
                            <span class="text-[9px] uppercase tracking-widest opacity-90">BUKU</span>
                        </div>

                        <!-- Detail Judul Buku -->
                        <div class="flex-1 min-w-0">
                            <span class="text-[10px] font-extrabold uppercase tracking-wider text-[#7A5236] block">
                                Buku Siap Disortir
                            </span>
                            <h3 class="font-display font-bold text-base sm:text-lg text-[#362216] leading-snug mt-0.5">
                                ${book.title}
                            </h3>
                            ${damageBadge}
                        </div>
                    </div>
                </div>
            `;

            const cardEl = document.getElementById('active-book-card');
            cardEl.addEventListener('dragstart', (e) => {
                if (!state.isPlaying || state.isPausedForExplanation) {
                    e.preventDefault();
                    return;
                }
                e.dataTransfer.setData('text/plain', book.uid);
                e.dataTransfer.effectAllowed = 'move';
                cardEl.classList.add('opacity-65');
            });

            cardEl.addEventListener('dragend', () => {
                cardEl.classList.remove('opacity-65');
                document.querySelectorAll('.shelf-card').forEach(el => el.classList.remove('shelf-drag-over'));
            });
        }

        function renderShelves() {
            dom.shelvesGrid.innerHTML = SHELVES.map(shelf => `
                <button
                    type="button"
                    data-shelf="${shelf.id}"
                    class="shelf-card text-left border-2 rounded-2xl p-3.5 sm:p-4 shadow-xs flex flex-col justify-between gap-2 cursor-pointer focus:outline-none ${shelf.cardClass}"
                >
                    <div class="flex items-center justify-between gap-2">
                        <span class="text-2xl sm:text-3xl">${shelf.icon}</span>
                        <span class="text-[11px] font-extrabold px-2.5 py-0.5 rounded-full ${shelf.badgeClass}">
                            ${shelf.code}
                        </span>
                    </div>
                    <div>
                        <div class="font-display font-bold text-base sm:text-lg leading-tight">${shelf.name}</div>
                        <p class="text-[11px] opacity-85 mt-0.5">Klik atau letakkan buku ke sini</p>
                    </div>
                </button>
            `).join('');

            document.querySelectorAll('.shelf-card').forEach(btn => {
                const shelfId = btn.getAttribute('data-shelf');

                btn.addEventListener('click', (e) => {
                    handleShelfSelection(shelfId, e);
                });

                btn.addEventListener('dragover', (e) => {
                    if (!state.isPlaying || state.isPausedForExplanation) return;
                    e.preventDefault();
                    e.dataTransfer.dropEffect = 'move';
                    btn.classList.add('shelf-drag-over');
                });

                btn.addEventListener('dragleave', () => {
                    btn.classList.remove('shelf-drag-over');
                });

                btn.addEventListener('drop', (e) => {
                    e.preventDefault();
                    btn.classList.remove('shelf-drag-over');
                    if (!state.isPlaying || state.isPausedForExplanation) return;
                    handleShelfSelection(shelfId, e);
                });
            });
        }

        /**
         * =====================================================================
         * 6. MEKANIKA GAMEPLAY & MODE PEMBAHASAN INSTAN
         * =====================================================================
         */
        function spawnBookToDesk() {
            const maxQueue = DIFFICULTY_CONFIG[state.difficulty].maxQueue;
            if (state.bookQueue.length >= maxQueue) {
                // Penalti kecil bila meja terlalu penuh
                state.score = Math.max(0, state.score - 25);
                updateHUD();
                return;
            }
            state.bookQueue.push(createRandomBook());
            updateHUD();
            if (state.bookQueue.length === 1) {
                renderActiveBook();
            }
        }

        function triggerVisitorEvent() {
            if (!state.isPlaying || state.isPausedForExplanation || state.activeVisitor) return;
            const q = VISITOR_QUESTIONS[Math.floor(Math.random() * VISITOR_QUESTIONS.length)];
            state.activeVisitor = { ...q };
            dom.visitorAvatar.textContent = q.avatar;
            dom.visitorQuestion.textContent = q.text;
            dom.visitorBanner.classList.remove('hidden');
            sfx.playVisitor();
        }

        function openInstantExplanation({ title, itemLabel, userShelfId, correctShelfId, reason, endAfterClose = false }) {
            const userShelf = getShelfById(userShelfId);
            const correctShelf = getShelfById(correctShelfId);

            state.isPausedForExplanation = true;
            state.pendingEndReason = endAfterClose
                ? 'Kesempatan ketelitian habis! Perhatikan pembahasan di atas sebagai bekal bermain lagi.'
                : null;

            dom.explainModalTitle.textContent = title;
            dom.explainItemLabel.textContent = itemLabel;
            dom.explainUserChoice.textContent = `Pilihanmu: ${userShelf.name} (${userShelf.code})`;
            dom.explainCorrectAnswer.textContent = `Jawaban Tepat: ${correctShelf.name} (${correctShelf.code})`;
            dom.explainReason.textContent = reason;

            dom.modalExplanation.classList.remove('hidden');
        }

        function closeInstantExplanation() {
            dom.modalExplanation.classList.add('hidden');
            state.isPausedForExplanation = false;

            if (state.pendingEndReason) {
                const reason = state.pendingEndReason;
                state.pendingEndReason = null;
                endGame(reason);
            }
        }

        function handleShelfSelection(shelfId, event) {
            if (!state.isPlaying || state.isPausedForExplanation) return;

            const x = event && event.clientX ? event.clientX : window.innerWidth / 2;
            const y = event && event.clientY ? event.clientY : window.innerHeight / 2;

            // Prioritas 1: Menjawab Pengunjung Bertanya
            if (state.activeVisitor) {
                const visitor = state.activeVisitor;
                const correctShelf = getShelfById(visitor.target);
                const chosenShelf = getShelfById(shelfId);

                if (shelfId === visitor.target) {
                    state.score += 150;
                    state.timeLeft = Math.min(state.maxTime, state.timeLeft + 5);
                    state.streak++;
                    if (state.streak > state.maxStreak) state.maxStreak = state.streak;

                    recordAction({
                        category: 'Pengunjung',
                        title: `Pertanyaan Pengunjung: ${visitor.text}`,
                        isCorrect: true,
                        userChoice: `${chosenShelf.name} (${chosenShelf.code})`,
                        correctChoice: `${correctShelf.name} (${correctShelf.code})`,
                        reason: correctShelf.reason
                    });

                    sfx.playCorrect(state.streak);
                    showFloatingText('Pengunjung Terbantu! +150 & +5d 🎉', x, y, '#15803D');
                    state.activeVisitor = null;
                    dom.visitorBanner.classList.add('hidden');
                    updateHUD();
                } else {
                    sfx.playWrong();
                    state.streak = 0;

                    recordAction({
                        category: 'Pengunjung',
                        title: `Pertanyaan Pengunjung: ${visitor.text}`,
                        isCorrect: false,
                        userChoice: `${chosenShelf.name} (${chosenShelf.code})`,
                        correctChoice: `${correctShelf.name} (${correctShelf.code})`,
                        reason: correctShelf.reason
                    });

                    showFloatingText('Bukan rak itu yang dicari pengunjung! 🤔', x, y, '#D97706');
                    updateHUD();

                    if (state.instantExplanation) {
                        openInstantExplanation({
                            title: 'Kurang Tepat Menjawab Pengunjung',
                            itemLabel: `Pertanyaan: ${visitor.text}`,
                            userShelfId: shelfId,
                            correctShelfId: visitor.target,
                            reason: correctShelf.reason
                        });
                    }
                }
                return;
            }

            // Prioritas 2: Menyortir Buku Aktif di Meja
            if (state.bookQueue.length === 0) return;
            const currentBook = state.bookQueue[0];
            const correctShelf = getShelfById(currentBook.targetShelf);
            const chosenShelf = getShelfById(shelfId);
            const reasonText = currentBook.isDamaged
                ? `Buku ini mengalami kondisi fisik (${currentBook.damageReason}). ${correctShelf.reason}`
                : `Buku "${currentBook.title}" berkode DDC ${currentBook.ddc}. ${correctShelf.reason}`;

            if (shelfId === currentBook.targetShelf) {
                state.streak++;
                if (state.streak > state.maxStreak) state.maxStreak = state.streak;
                state.sortedCount++;

                const comboBonus = Math.min(state.streak * 10, 100);
                const points = 100 + comboBonus;
                state.score += points;

                recordAction({
                    category: currentBook.isDamaged ? 'Buku Rusak' : 'Buku DDC',
                    title: `${currentBook.title} (${currentBook.isDamaged ? `Rusak: ${currentBook.damageReason}` : `DDC ${currentBook.ddc}`})`,
                    isCorrect: true,
                    userChoice: `${chosenShelf.name} (${chosenShelf.code})`,
                    correctChoice: `${correctShelf.name} (${correctShelf.code})`,
                    reason: reasonText
                });

                sfx.playCorrect(state.streak);
                showFloatingText(`+${points} Tepat! ✨`, x, y, '#15803D');

                state.bookQueue.shift();
                if (state.bookQueue.length === 0) {
                    state.bookQueue.push(createRandomBook());
                }

                updateHUD();
                renderActiveBook();
            } else {
                sfx.playWrong();
                state.streak = 0;
                state.lives--;

                recordAction({
                    category: currentBook.isDamaged ? 'Buku Rusak' : 'Buku DDC',
                    title: `${currentBook.title} (${currentBook.isDamaged ? `Rusak: ${currentBook.damageReason}` : `DDC ${currentBook.ddc}`})`,
                    isCorrect: false,
                    userChoice: `${chosenShelf.name} (${chosenShelf.code})`,
                    correctChoice: `${correctShelf.name} (${correctShelf.code})`,
                    reason: reasonText
                });

                const cardEl = document.getElementById('active-book-card');
                if (cardEl) {
                    cardEl.classList.remove('animate-pop-in');
                    void cardEl.offsetWidth;
                    cardEl.classList.add('animate-shake');
                }

                const hint = currentBook.isDamaged
                    ? 'Buku rusak! Arahkan ke Keranjang Perbaikan 🩹'
                    : `Salah rak! Cek kode DDC ${currentBook.ddc}`;
                showFloatingText(hint, x, y, '#DC2626');
                updateHUD();

                const outOfLives = state.lives <= 0;
                if (state.instantExplanation) {
                    openInstantExplanation({
                        title: currentBook.isDamaged ? 'Perhatikan Kondisi Fisik Buku!' : 'Salah Penempatan Rak DDC',
                        itemLabel: `Buku: "${currentBook.title}" — ${currentBook.isDamaged ? `Rusak (${currentBook.damageReason})` : `Kode DDC ${currentBook.ddc}`}`,
                        userShelfId: shelfId,
                        correctShelfId: currentBook.targetShelf,
                        reason: reasonText,
                        endAfterClose: outOfLives
                    });
                } else if (outOfLives) {
                    endGame('Kesempatan ketelitian habis! Coba aktifkan Pembahasan Instan untuk belajar dari tiap kesalahan.');
                }
            }
        }

        function startGame() {
            sfx.init();
            clearAllTimers();

            const cfg = DIFFICULTY_CONFIG[state.difficulty];
            state.isPlaying = true;
            state.isPausedForExplanation = false;
            state.recapFilter = 'all';
            state.score = 0;
            state.streak = 0;
            state.maxStreak = 0;
            state.sortedCount = 0;
            state.correctActions = 0;
            state.wrongActions = 0;
            state.lives = 3;
            state.timeLeft = cfg.duration;
            state.maxTime = cfg.duration;
            state.bookQueue = [createRandomBook()];
            state.activeVisitor = null;
            state.history = [];
            state.pendingEndReason = null;

            dom.visitorBanner.classList.add('hidden');
            dom.modalExplanation.classList.add('hidden');

            switchScreen('game');
            updateHUD();
            renderActiveBook();

            state.timers.clock = setInterval(() => {
                if (!state.isPlaying || state.isPausedForExplanation) return;
                state.timeLeft--;
                updateHUD();
                if (state.timeLeft <= 0) {
                    endGame('Waktu tugas perpustakaan telah selesai!');
                }
            }, 1000);

            state.timers.spawner = setInterval(() => {
                if (!state.isPlaying || state.isPausedForExplanation) return;
                spawnBookToDesk();
            }, cfg.spawnInterval);

            state.timers.visitor = setInterval(() => {
                if (!state.isPlaying || state.isPausedForExplanation || state.activeVisitor) return;
                triggerVisitorEvent();
            }, cfg.visitorInterval);
        }

        /**
         * =====================================================================
         * 7. LAYAR AKHIR, AKURASI, REKAP JAWABAN & EKSPOR (.TXT)
         * =====================================================================
         */
        function renderRecapList() {
            const total = state.history.length;
            const correctList = state.history.filter(h => h.isCorrect);
            const wrongList = state.history.filter(h => !h.isCorrect);

            dom.recapCountBadge.textContent = total;
            dom.recapAllCount.textContent = total;
            dom.recapCorrectCount.textContent = correctList.length;
            dom.recapWrongCount.textContent = wrongList.length;

            const items = state.recapFilter === 'correct'
                ? correctList
                : state.recapFilter === 'wrong'
                    ? wrongList
                    : state.history;

            if (items.length === 0) {
                dom.recapList.innerHTML = `
                    <div class="text-center text-xs sm:text-sm text-[#7A5236] bg-white/80 border border-[#E2D0B6] rounded-xl py-6">
                        Tidak ada catatan jawaban untuk filter ini.
                    </div>
                `;
                return;
            }

            dom.recapList.innerHTML = items.map((item, idx) => {
                const badge = item.isCorrect
                    ? `<span class="bg-emerald-700 text-white text-[10px] font-extrabold px-2 py-0.5 rounded-full shrink-0">✓ BENAR</span>`
                    : `<span class="bg-red-700 text-white text-[10px] font-extrabold px-2 py-0.5 rounded-full shrink-0">✕ SALAH</span>`;

                const boxStyle = item.isCorrect
                    ? 'bg-white border-emerald-300'
                    : 'bg-red-50/80 border-red-300';

                return `
                    <div class="${boxStyle} border rounded-xl p-3 text-xs space-y-1 shadow-2xs">
                        <div class="flex items-start justify-between gap-2">
                            <span class="font-bold text-[#362216]">${idx + 1}. [${item.category}] ${item.title}</span>
                            ${badge}
                        </div>
                        <p class="text-[#5C3D28]">
                            Jawabanmu: <strong>${item.userChoice}</strong> • Kunci: <strong class="text-emerald-800">${item.correctChoice}</strong>
                        </p>
                        <p class="text-[#362216]/90 leading-relaxed">
                            💡 ${item.reason}
                        </p>
                    </div>
                `;
            }).join('');
        }

        function setRecapTab(tab) {
            if (tab === 'recap') {
                dom.panelSummary.classList.add('hidden');
                dom.panelRecap.classList.remove('hidden');
                dom.tabRecap.className = 'px-4 py-2 rounded-xl text-xs sm:text-sm font-bold bg-[#588157] text-white shadow-xs transition cursor-pointer';
                dom.tabSummary.className = 'px-4 py-2 rounded-xl text-xs sm:text-sm font-bold bg-[#F2E8D5] text-[#4A3222] border border-[#A67B5B]/50 hover:bg-[#E5D8C1] transition cursor-pointer';
                renderRecapList();
            } else {
                dom.panelRecap.classList.add('hidden');
                dom.panelSummary.classList.remove('hidden');
                dom.tabSummary.className = 'px-4 py-2 rounded-xl text-xs sm:text-sm font-bold bg-[#588157] text-white shadow-xs transition cursor-pointer';
                dom.tabRecap.className = 'px-4 py-2 rounded-xl text-xs sm:text-sm font-bold bg-[#F2E8D5] text-[#4A3222] border border-[#A67B5B]/50 hover:bg-[#E5D8C1] transition cursor-pointer';
            }
        }

        function buildRecapPlainText() {
            const total = state.history.length;
            const accuracy = total > 0 ? Math.round((state.correctActions / total) * 100) : 0;

            const lines = [
                '==============================================',
                'REKAP HASIL — MISI PUSTAKAWAN CILIK',
                '==============================================',
                `Skor Akhir     : ${state.score}`,
                `Akurasi        : ${accuracy}% (${state.correctActions} Benar dari ${total} Aksi)`,
                `Kombo Terbaik : ${state.maxStreak}x`,
                `Buku Tersusun  : ${state.sortedCount}`,
                '----------------------------------------------',
                'RINCIAN JAWABAN:'
            ];

            if (state.history.length === 0) {
                lines.push('Belum ada aksi yang tercatat pada sesi ini.');
            } else {
                state.history.forEach((h, i) => {
                    lines.push(`${i + 1}. [${h.isCorrect ? 'BENAR' : 'SALAH'}] [${h.category}] ${h.title}`);
                    lines.push(`   Jawabanmu : ${h.userChoice}`);
                    lines.push(`   Kunci     : ${h.correctChoice}`);
                    lines.push(`   Alasan    : ${h.reason}`);
                });
            }

            return lines.join('\n');
        }

        function endGame(reasonText) {
            state.isPlaying = false;
            state.isPausedForExplanation = false;
            state.pendingEndReason = null;
            dom.modalExplanation.classList.add('hidden');
            clearAllTimers();
            sfx.playGameOver();

            const totalActions = state.history.length;
            const accuracy = totalActions > 0
                ? Math.round((state.correctActions / totalActions) * 100)
                : 0;

            let badge = '📘';
            let rank = 'Pustakawan Magang 🌱';
            if (state.score >= 2000 && accuracy >= 75) {
                badge = '👑';
                rank = 'Kepala Pustakawan Teladan';
            } else if (state.score >= 1100) {
                badge = '🥇';
                rank = 'Pustakawan Andal ⭐';
            } else if (state.score >= 450) {
                badge = '🎖️';
                rank = 'Pustakawan Muda 📚';
            }

            dom.endBadgeIcon.textContent = badge;
            dom.endRankTitle.textContent = rank;
            dom.endReason.textContent = reasonText;
            dom.endScore.textContent = state.score;
            dom.endAccuracy.textContent = `${accuracy}%`;
            dom.endMaxStreak.textContent = `${state.maxStreak}x`;
            dom.endSorted.textContent = state.sortedCount;
            dom.endFunFact.textContent = LITERACY_FACTS[Math.floor(Math.random() * LITERACY_FACTS.length)];

            dom.summaryDetailText.textContent = totalActions > 0
                ? `Kamu menyelesaikan ${totalActions} aksi penyortiran & pelayanan pengunjung dengan tingkat akurasi ${accuracy}% (${state.correctActions} tepat, ${state.wrongActions} kurang tepat) dan menyusun ${state.sortedCount} buku ke rak atau keranjang perbaikan.`
                : 'Belum ada buku yang sempat disortir pada sesi ini. Yuk coba mulai bertugas lagi!';

            dom.recapActionFeedback.classList.add('hidden');
            state.recapFilter = 'all';
            document.querySelectorAll('.recap-filter-btn').forEach(btn => {
                const f = btn.getAttribute('data-filter');
                if (f === 'all') {
                    btn.className = 'recap-filter-btn px-3 py-1.5 rounded-lg text-xs font-bold bg-[#4A3222] text-white cursor-pointer';
                } else if (f === 'correct') {
                    btn.className = 'recap-filter-btn px-3 py-1.5 rounded-lg text-xs font-bold bg-white text-emerald-800 border border-emerald-400 cursor-pointer';
                } else {
                    btn.className = 'recap-filter-btn px-3 py-1.5 rounded-lg text-xs font-bold bg-white text-red-800 border border-red-400 cursor-pointer';
                }
            });

            renderRecapList();
            setRecapTab('summary');
            switchScreen('end');
        }

        /**
         * =====================================================================
         * 8. INISIALISASI EVENT LISTENER
         * =====================================================================
         */
        function bindEvents() {
            // Pilih tingkat kesulitan
            document.querySelectorAll('.diff-btn').forEach(btn => {
                btn.addEventListener('click', () => {
                    state.difficulty = btn.getAttribute('data-diff');
                    document.querySelectorAll('.diff-btn').forEach(b => {
                        const active = b.getAttribute('data-diff') === state.difficulty;
                        b.className = active
                            ? 'diff-btn text-left p-3.5 rounded-2xl border-2 border-[#3A5A40] bg-[#E9EDC9]/80 shadow-xs transition cursor-pointer'
                            : 'diff-btn text-left p-3.5 rounded-2xl border-2 border-[#D8C3A5] bg-[#FAF6EE] hover:border-[#A67B5B] transition cursor-pointer';
                    });
                });
            });

            // Mulai & main lagi
            document.getElementById('btn-start-game').addEventListener('click', startGame);
            document.getElementById('btn-play-again').addEventListener('click', startGame);

            // Kembali ke menu utama
            const goHome = () => {
                state.isPlaying = false;
                state.isPausedForExplanation = false;
                dom.modalExplanation.classList.add('hidden');
                clearAllTimers();
                switchScreen('start');
            };
            document.getElementById('btn-brand-home').addEventListener('click', goHome);
            document.getElementById('btn-back-home').addEventListener('click', goHome);

            // Selesai lebih awal
            document.getElementById('btn-finish-early').addEventListener('click', () => {
                if (!state.isPlaying) return;
                endGame('Kamu mengakhiri shift lebih awal untuk memeriksa rekap hasil.');
            });

            // Toggle Mode Pembahasan Instan
            document.getElementById('btn-instant-explain').addEventListener('click', () => {
                state.instantExplanation = !state.instantExplanation;
                dom.explainStatus.textContent = state.instantExplanation ? 'ON' : 'OFF';
                dom.explainStatus.className = state.instantExplanation
                    ? 'font-extrabold text-amber-300'
                    : 'font-extrabold text-stone-300';
            });

            // Tutup modal pembahasan instan
            document.getElementById('btn-continue-after-explain').addEventListener('click', closeInstantExplanation);

            // Modal Panduan DDC
            const openGuide = () => dom.modalGuide.classList.remove('hidden');
            const closeGuide = () => dom.modalGuide.classList.add('hidden');
            document.getElementById('btn-guide').addEventListener('click', openGuide);
            document.getElementById('btn-open-guide-start').addEventListener('click', openGuide);
            document.getElementById('btn-close-guide').addEventListener('click', closeGuide);
            document.getElementById('btn-close-guide-bottom').addEventListener('click', closeGuide);
            dom.modalGuide.addEventListener('click', (e) => {
                if (e.target === dom.modalGuide) closeGuide();
            });

            // Tombol suara mute/unmute
            document.getElementById('btn-sound').addEventListener('click', () => {
                const muted = sfx.toggleMute();
                document.getElementById('sound-icon').textContent = muted ? '🔇' : '🔊';
            });

            // Tab Ringkasan & Rekap Jawaban
            dom.tabSummary.addEventListener('click', () => setRecapTab('summary'));
            dom.tabRecap.addEventListener('click', () => setRecapTab('recap'));

            // Filter rekap jawaban
            document.querySelectorAll('.recap-filter-btn').forEach(btn => {
                btn.addEventListener('click', () => {
                    state.recapFilter = btn.getAttribute('data-filter');
                    document.querySelectorAll('.recap-filter-btn').forEach(b => {
                        const f = b.getAttribute('data-filter');
                        if (f === state.recapFilter) {
                            b.className = 'recap-filter-btn px-3 py-1.5 rounded-lg text-xs font-bold bg-[#4A3222] text-white cursor-pointer';
                        } else if (f === 'correct') {
                            b.className = 'recap-filter-btn px-3 py-1.5 rounded-lg text-xs font-bold bg-white text-emerald-800 border border-emerald-400 cursor-pointer';
                        } else {
                            b.className = 'recap-filter-btn px-3 py-1.5 rounded-lg text-xs font-bold bg-white text-red-800 border border-red-400 cursor-pointer';
                        }
                    });
                    renderRecapList();
                });
            });

            // Salin rekap ke clipboard
            document.getElementById('btn-copy-recap').addEventListener('click', () => {
                const text = buildRecapPlainText();
                const notify = (msg) => {
                    dom.recapActionFeedback.textContent = msg;
                    dom.recapActionFeedback.classList.remove('hidden');
                };

                if (navigator.clipboard && navigator.clipboard.writeText) {
                    navigator.clipboard.writeText(text).then(() => {
                        notify('✓ Rekap hasil berhasil disalin ke papan klip!');
                    }).catch(() => {
                        const ta = document.createElement('textarea');
                        ta.value = text;
                        document.body.appendChild(ta);
                        ta.select();
                        document.execCommand('copy');
                        ta.remove();
                        notify('✓ Rekap hasil berhasil disalin!');
                    });
                } else {
                    const ta = document.createElement('textarea');
                    ta.value = text;
                    document.body.appendChild(ta);
                    ta.select();
                    document.execCommand('copy');
                    ta.remove();
                    notify('✓ Rekap hasil berhasil disalin!');
                }
            });

            // Unduh rekap sebagai berkas .txt
            document.getElementById('btn-download-recap').addEventListener('click', () => {
                const text = buildRecapPlainText();
                const blob = new Blob([text], { type: 'text/plain;charset=utf-8' });
                const url = URL.createObjectURL(blob);
                const link = document.createElement('a');
                link.href = url;
                link.download = `rekap-misi-pustakawan-cilik-${Date.now()}.txt`;
                document.body.appendChild(link);
                link.click();
                link.remove();
                URL.revokeObjectURL(url);

                dom.recapActionFeedback.textContent = '✓ Berkas rekap (.txt) berhasil diunduh!';
                dom.recapActionFeedback.classList.remove('hidden');
            });
        }

        window.addEventListener('DOMContentLoaded', () => {
            renderShelves();
            bindEvents();
            switchScreen('start');
        });
    </script>
</body>
</html>
