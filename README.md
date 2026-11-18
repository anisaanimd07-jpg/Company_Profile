<!DOCTYPE html>
<html lang="id" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>TKJ SMK Banjar Asri - Teknik Komputer dan Jaringan</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Google Fonts: Inter -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
    <!-- Font Awesome untuk Ikon Profesional -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
    
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                    },
                    colors: {
                        brand: {
                            50: '#eff6ff',
                            100: '#dbeafe',
                            200: '#bfdbfe',
                            300: '#93c5fd',
                            400: '#60a5fa',
                            500: '#3b82f6',
                            600: '#2563eb',
                            700: '#1d4ed8',
                            800: '#1e40af',
                            900: '#1e3a8a',
                            950: '#0f172a',
                        }
                    }
                }
            }
        }
    </script>
</head>
<body class="font-sans text-slate-800 bg-slate-50 antialiased selection:bg-brand-600 selection:text-white overflow-x-hidden">

    <!-- 1. NAVBAR RESPONSIF -->
    <header id="navbar" class="fixed top-0 left-0 right-0 z-50 bg-white/90 backdrop-blur-md border-b border-slate-200/80 transition-all duration-300">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-20">
                <!-- Logo & Judul -->
                <a href="#beranda" class="flex items-center gap-3 group">
                    <div class="w-11 h-11 rounded-xl bg-gradient-to-br from-brand-600 to-brand-800 flex items-center justify-center text-white shadow-lg shadow-brand-600/25 group-hover:scale-105 transition-transform">
                        <i class="fa-solid fa-network-wired text-lg"></i>
                    </div>
                    <div>
                        <span class="block text-lg font-extrabold tracking-tight text-slate-900 leading-none">TKJ <span class="text-brand-600">SMK BANJAR ASRI</span></span>
                        <span class="block text-xs font-medium text-slate-500 mt-1">Teknik Komputer & Jaringan</span>
                    </div>
                </a>

                <!-- Menu Navigasi Desktop -->
                <nav class="hidden lg:flex items-center space-x-1">
                    <a href="#beranda" class="px-3.5 py-2 rounded-lg text-sm font-medium text-slate-700 hover:text-brand-600 hover:bg-brand-50 transition-colors">Beranda</a>
                    <a href="#tentang" class="px-3.5 py-2 rounded-lg text-sm font-medium text-slate-700 hover:text-brand-600 hover:bg-brand-50 transition-colors">Tentang TKJ</a>
                    <a href="#kompetensi" class="px-3.5 py-2 rounded-lg text-sm font-medium text-slate-700 hover:text-brand-600 hover:bg-brand-50 transition-colors">Kompetensi & Kurikulum</a>
                    <a href="#fasilitas" class="px-3.5 py-2 rounded-lg text-sm font-medium text-slate-700 hover:text-brand-600 hover:bg-brand-50 transition-colors">Fasilitas Lab</a>
                    <a href="#karir" class="px-3.5 py-2 rounded-lg text-sm font-medium text-slate-700 hover:text-brand-600 hover:bg-brand-50 transition-colors">Prospek Karir</a>
                    <a href="#kontak" class="ml-3 px-5 py-2.5 rounded-xl text-sm font-semibold text-white bg-brand-600 hover:bg-brand-700 shadow-md shadow-brand-600/20 transition-all">Kontak</a>
                </nav>

                <!-- Tombol Hamburger Mobile -->
                <button id="mobile-menu-btn" type="button" aria-label="Buka Menu" class="lg:hidden p-3 rounded-xl text-slate-700 hover:bg-slate-100 focus:outline-none focus:ring-2 focus:ring-brand-500">
                    <i id="menu-icon" class="fa-solid fa-bars text-xl"></i>
                </button>
            </div>
        </div>

        <!-- Menu Navigasi Mobile -->
        <div id="mobile-menu" class="hidden lg:hidden bg-white border-b border-slate-200 px-4 pt-2 pb-6 space-y-1 shadow-xl">
            <a href="#beranda" class="mobile-link block px-4 py-3 rounded-xl text-base font-medium text-slate-700 hover:text-brand-600 hover:bg-brand-50">Beranda</a>
            <a href="#tentang" class="mobile-link block px-4 py-3 rounded-xl text-base font-medium text-slate-700 hover:text-brand-600 hover:bg-brand-50">Tentang TKJ</a>
            <a href="#kompetensi" class="mobile-link block px-4 py-3 rounded-xl text-base font-medium text-slate-700 hover:text-brand-600 hover:bg-brand-50">Kompetensi & Kurikulum</a>
            <a href="#fasilitas" class="mobile-link block px-4 py-3 rounded-xl text-base font-medium text-slate-700 hover:text-brand-600 hover:bg-brand-50">Fasilitas Lab</a>
            <a href="#karir" class="mobile-link block px-4 py-3 rounded-xl text-base font-medium text-slate-700 hover:text-brand-600 hover:bg-brand-50">Prospek Karir</a>
            <a href="#kontak" class="mobile-link block mt-3 text-center px-4 py-3 rounded-xl text-base font-semibold text-white bg-brand-600 hover:bg-brand-700">Hubungi Kami</a>
        </div>
    </header>

<!-- 2. HERO SECTION -->
    <section id="beranda" class="relative pt-28 pb-20 lg:pt-36 lg:pb-28 bg-slate-950 text-white overflow-hidden">
        <!-- Dekorasi Latar Belakang Grid & Glow -->
        <div class="absolute inset-0 bg-[radial-gradient(#1e3a8a_1px,transparent_1px)] [background-size:24px_24px] opacity-30"></div>
        <div class="absolute -top-24 -right-24 w-96 h-96 bg-brand-600/20 rounded-full blur-3xl pointer-events-none"></div>
        <div class="absolute -bottom-24 -left-24 w-96 h-96 bg-cyan-500/15 rounded-full blur-3xl pointer-events-none"></div>

        <div class="relative max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 items-center">
                <!-- Konten Kiri -->
                <div class="lg:col-span-7 text-center lg:text-left">
                    <div class="inline-flex items-center gap-2 px-4 py-2 rounded-full bg-brand-900/60 border border-brand-500/30 text-brand-300 text-xs sm:text-sm font-semibold mb-6">
                        <span class="w-2 h-2 rounded-full bg-cyan-400 animate-pulse"></span>
                        Kompetensi Keahlian Unggulan • SMK Banjar Asri Cimaung
                    </div>
                    <h1 class="text-3xl sm:text-5xl lg:text-6xl font-extrabold tracking-tight leading-tight mb-6">
                        Mencetak Generasi Ahli <span class="text-transparent bg-clip-text bg-gradient-to-r from-brand-400 to-cyan-300">Infrastruktur Jaringan</span> & Teknologi Masa Depan
                    </h1>
                    <p class="text-base sm:text-lg text-slate-300 leading-relaxed mb-8 max-w-2xl mx-auto lg:mx-0">
                        Jurusan Teknik Komputer dan Jaringan (TKJ) SMK Banjar Asri membekali siswa dengan keahlian praktis merancang jaringan komputer, administrasi server Linux/Windows, instalasi fiber optik, hingga keamanan siber berstandar industri.
                    </p>
                    <div class="flex flex-col sm:flex-row items-center justify-center lg:justify-start gap-4">
                        <a href="#kompetensi" class="w-full sm:w-auto px-7 py-4 rounded-xl bg-brand-600 hover:bg-brand-500 text-white font-semibold text-base shadow-lg shadow-brand-600/30 transition-all flex items-center justify-center gap-2">
                            <span>Jelajahi Kurikulum</span>
                            <i class="fa-solid fa-arrow-right text-sm"></i>
                        </a>
                        <a href="#fasilitas" class="w-full sm:w-auto px-7 py-4 rounded-xl bg-slate-800/80 hover:bg-slate-800 border border-slate-700 text-slate-200 font-semibold text-base transition-all flex items-center justify-center gap-2">
                            <i class="fa-solid fa-server text-brand-400"></i>
                            <span>Lihat Fasilitas Lab</span>
                        </a>
                    </div>

                    <!-- Highlight Poin Singkat -->
                    <div class="grid grid-cols-3 gap-4 mt-12 pt-8 border-t border-slate-800/80 max-w-lg mx-auto lg:mx-0">
                        <div>
                            <p class="text-2xl sm:text-3xl font-extrabold text-white">70%</p>
                            <p class="text-xs sm:text-sm text-slate-400 mt-1">Praktik Lab & Proyek</p>
                        </div>
                        <div>
                            <p class="text-2xl sm:text-3xl font-extrabold text-brand-400">MikroTik</p>
                            <p class="text-xs sm:text-sm text-slate-400 mt-1">& Cisco Academy</p>
                        </div>
                        <div>
                            <p class="text-2xl sm:text-3xl font-extrabold text-cyan-400">Siap</p>
                            <p class="text-xs sm:text-sm text-slate-400 mt-1">Kerja, Kuliah & Usaha</p>
                        </div>
                    </div>
                </div>

                <!-- Visual Kanan (Ilustrasi Kartu Topologi & Server) -->
                <div class="lg:col-span-5">
                    <div class="relative rounded-2xl bg-slate-900/90 border border-slate-800 p-6 sm:p-8 shadow-2xl">
                        <!-- Header Terminal/Dashboard Mockup -->
                        <div class="flex items-center justify-between pb-4 mb-6 border-b border-slate-800">
                            <div class="flex items-center gap-2">
                                <span class="w-3 h-3 rounded-full bg-rose-500"></span>
                                <span class="w-3 h-3 rounded-full bg-amber-400"></span>
                                <span class="w-3 h-3 rounded-full bg-emerald-500"></span>
                            </div>
                            <span class="text-xs font-mono text-slate-400">tkj-core-router@banjarasri</span>
                        </div>

                        <!-- Gambar Ilustrasi Jaringan -->
                        <div class="relative rounded-xl overflow-hidden mb-6 bg-slate-800 aspect-video">
                            <img src="https://images.unsplash.com/photo-1558494949-ef010cbdcc31?auto=format&fit=crop&w=900&q=80" 
                                 onerror="this.src='https://placehold.co/800x450/1e3a8a/ffffff?text=Laboratorium+Jaringan+TKJ'" 
                                 alt="Infrastruktur Server dan Jaringan TKJ SMK Banjar Asri" 
                                 class="w-full h-full object-cover opacity-90">
                            <div class="absolute inset-0 bg-gradient-to-t from-slate-950/90 via-slate-950/20 to-transparent flex items-end p-4">
                                <div class="flex items-center gap-3">
                                    <div class="w-10 h-10 rounded-lg bg-brand-600 flex items-center justify-center text-white shrink-0">
                                        <i class="fa-solid fa-shield-halved"></i>
                                    </div>
                                    <div>
                                        <p class="text-sm font-bold text-white">Praktikum Infrastruktur Nyata</p>
                                        <p class="text-xs text-slate-300">Konfigurasi Router, Switch Manageable & Fiber Optik</p>
                                    </div>
                                </div>
                            </div>
                        </div>

                        <!-- Status Bar Interaktif Statis -->
                        <div class="space-y-3 font-mono text-xs">
                            <div class="flex items-center justify-between p-3 rounded-xl bg-slate-800/70 border border-slate-700/60">
                                <span class="text-slate-300"><i class="fa-solid fa-circle-check text-emerald-400 mr-2"></i>Routing & Switching</span>
                                <span class="px-2 py-0.5 rounded bg-emerald-500/10 text-emerald-400">AKTIF</span>
                            </div>
                            <div class="flex items-center justify-between p-3 rounded-xl bg-slate-800/70 border border-slate-700/60">
                                <span class="text-slate-300"><i class="fa-solid fa-circle-check text-brand-400 mr-2"></i>Linux Server & Cloud</span>
                                <span class="px-2 py-0.5 rounded bg-brand-500/10 text-brand-300">TERINTEGRASI</span>
                            </div>
                            <div class="flex items-center justify-between p-3 rounded-xl bg-slate-800/70 border border-slate-700/60">
                                <span class="text-slate-300"><i class="fa-solid fa-circle-check text-cyan-400 mr-2"></i>FTTH Fiber Optic Splicing</span>
                                <span class="px-2 py-0.5 rounded bg-cyan-500/10 text-cyan-300">STANDAR ISP</span>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

  <!-- 3. TENTANG JURUSAN TKJ -->
    <section id="tentang" class="py-20 lg:py-28 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 items-center">
                <!-- Kolom Gambar -->
                <div class="lg:col-span-5 order-2 lg:order-1">
                    <div class="relative">
                        <div class="rounded-2xl overflow-hidden shadow-xl border border-slate-200">
                            <img src="https://images.unsplash.com/photo-1581092921461-eab62e97a780?auto=format&fit=crop&w=900&q=80" 
                                 onerror="this.src='https://placehold.co/800x600/eff6ff/1e3a8a?text=Praktikum+Siswa+TKJ'" 
                                 alt="Kegiatan Praktikum Siswa TKJ SMK Banjar Asri" 
                                 class="w-full h-auto object-cover">
                        </div>
                        <!-- Kartu Badge Mengambang -->
                        <div class="mt-4 sm:mt-0 sm:absolute sm:-bottom-6 sm:-right-6 bg-slate-900 text-white p-5 rounded-2xl shadow-xl border border-slate-800 max-w-xs">
                            <div class="flex items-center gap-3 mb-2">
                                <div class="w-10 h-10 rounded-xl bg-brand-600 flex items-center justify-center text-white">
                                    <i class="fa-solid fa-award text-lg"></i>
                                </div>
                                <h4 class="font-bold text-sm">Kurikulum Link & Match</h4>
                            </div>
                            <p class="text-xs text-slate-300 leading-relaxed">
                                Materi pembelajaran diselaraskan langsung dengan kebutuhan perusahaan penyedia layanan internet (ISP) dan industri TI modern.
                            </p>
                        </div>
                    </div>
                </div>

                <!-- Kolom Deskripsi & Visi -->
                <div class="lg:col-span-7 order-1 lg:order-2">
                    <span class="inline-block px-3.5 py-1.5 rounded-lg bg-brand-50 text-brand-700 text-xs font-bold uppercase tracking-wider mb-3">
                        Tentang Jurusan TKJ
                    </span>
                    <h2 class="text-3xl sm:text-4xl font-extrabold text-slate-900 tracking-tight mb-6">
                        Pusat Pendidikan Vokasi Teknologi Informasi & Jaringan di Cimaung
                    </h2>
                    <p class="text-slate-600 text-base sm:text-lg leading-relaxed mb-6">
                        Program Keahlian <strong>Teknik Komputer dan Jaringan (TKJ) SMK Banjar Asri</strong> dirancang untuk menyiapkan tenaga teknis menengah yang kompeten, berkarakter, dan adaptif terhadap perkembangan teknologi digital. Siswa tidak hanya mempelajari teori perakitan perangkat keras, tetapi juga mendalami arsitektur jaringan skala luas (WAN), manajemen server, hingga teknologi fiber optik.
                    </p>

                    <!-- Kotak Visi Singkat -->
                    <div class="p-6 rounded-2xl bg-gradient-to-br from-brand-50 to-slate-50 border border-brand-100 mb-8">
                        <div class="flex items-start gap-4">
                            <div class="w-12 h-12 rounded-xl bg-brand-600 text-white flex items-center justify-center shrink-0 mt-1">
                                <i class="fa-solid fa-eye text-lg"></i>
                            </div>
                            <div>
                                <h3 class="text-lg font-bold text-slate-900 mb-1">Visi Kompetensi Keahlian</h3>
                                <p class="text-sm sm:text-base text-slate-600 leading-relaxed">
                                    "Menjadi program keahlian unggulan yang menghasilkan lulusan profesional di bidang teknik komputer, jaringan, dan administrasi server yang berakhlak mulia, inovatif, serta siap bersaing di era transformasi digital."
                                </p>
                            </div>
                        </div>
                    </div>

<!-- 3 Pilar Fokus Pembelajaran -->
                    <div class="grid grid-cols-1 sm:grid-cols-3 gap-4">
                        <div class="p-4 rounded-xl bg-slate-50 border border-slate-200/80">
                            <i class="fa-solid fa-network-wired text-brand-600 text-xl mb-2"></i>
                            <h4 class="font-bold text-slate-900 text-sm">Jaringan Komputer</h4>
                            <p class="text-xs text-slate-500 mt-1">Perancangan LAN, WLAN, VLAN, Routing & Fiber Optik.</p>
                        </div>
                        <div class="p-4 rounded-xl bg-slate-50 border border-slate-200/80">
                            <i class="fa-solid fa-server text-brand-600 text-xl mb-2"></i>
                            <h4 class="font-bold text-slate-900 text-sm">Administrasi Server</h4>
                            <p class="text-xs text-slate-500 mt-1">Pengelolaan server berbasis Linux Debian/Ubuntu & Windows.</p>
                        </div>
                        <div class="p-4 rounded-xl bg-slate-50 border border-slate-200/80">
                            <i class="fa-solid fa-microchip text-brand-600 text-xl mb-2"></i>
                            <h4 class="font-bold text-slate-900 text-sm">Teknologi Informasi</h4>
                            <p class="text-xs text-slate-500 mt-1">Perakitan PC, troubleshooting hardware, & dasar IoT.</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 4. KOMPETENSI KEAHLIAN / MATERI UTAMA -->
    <section id="kompetensi" class="py-20 lg:py-28 bg-slate-50 border-y border-slate-200/70">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <span class="inline-block px-3.5 py-1.5 rounded-lg bg-brand-100 text-brand-700 text-xs font-bold uppercase tracking-wider mb-3">
                    Kompetensi & Kurikulum
                </span>
                <h2 class="text-3xl sm:text-4xl font-extrabold text-slate-900 tracking-tight mb-4">
                    Materi Utama Keahlian TKJ
                </h2>
                <p class="text-slate-600 text-base sm:text-lg">
                    Struktur pembelajaran komprehensif yang mengombinasikan dasar teknologi komputer hingga rekayasa jaringan tingkat lanjut.
                </p>
            </div>

            <!-- Grid Kartu Kompetensi -->
            <div class="grid grid-cols-1 md:grid-cols-2 gap-6 lg:gap-8">
                <!-- Kompetensi 1 -->
                <div class="group bg-white rounded-2xl p-7 sm:p-8 border border-slate-200/90 shadow-sm hover:shadow-xl hover:border-brand-300 transition-all duration-300">
                    <div class="flex items-start justify-between mb-6">
                        <div class="w-14 h-14 rounded-2xl bg-brand-50 text-brand-600 group-hover:bg-brand-600 group-hover:text-white flex items-center justify-center transition-colors">
                            <i class="fa-solid fa-sitemap text-2xl"></i>
                        </div>
                        <span class="px-3 py-1 rounded-full bg-slate-100 text-slate-600 text-xs font-semibold">Modul 01</span>
                    </div>
                    <h3 class="text-xl font-bold text-slate-900 mb-3">Administrasi Infrastruktur Jaringan (AIJ)</h3>
                    <p class="text-slate-600 text-sm sm:text-base leading-relaxed mb-5">
                        Mempelajari konfigurasi perangkat jaringan skala kecil hingga enterprise menggunakan router dan switch manageable.
                    </p>
                    <ul class="space-y-2.5 text-sm text-slate-700">
                        <li class="flex items-center gap-2.5">
                            <i class="fa-solid fa-check text-brand-600 text-xs"></i>
                            <span>Konfigurasi VLAN, Trunking, dan Inter-VLAN Routing</span>
                        </li>
                        <li class="flex items-center gap-2.5">
                            <i class="fa-solid fa-check text-brand-600 text-xs"></i>
                            <span>Routing Statis & Dinamis (OSPF, BGP dasar) pada MikroTik & Cisco</span>
                        </li>
                        <li class="flex items-center gap-2.5">
                            <i class="fa-solid fa-check text-brand-600 text-xs"></i>
                            <span>Manajemen Bandwidth (QoS), Hotspot, dan Load Balancing</span>
                        </li>
                    </ul>
                </div>

                <!-- Kompetensi 2 -->
                <div class="group bg-white rounded-2xl p-7 sm:p-8 border border-slate-200/90 shadow-sm hover:shadow-xl hover:border-brand-300 transition-all duration-300">
                    <div class="flex items-start justify-between mb-6">
                        <div class="w-14 h-14 rounded-2xl bg-brand-50 text-brand-600 group-hover:bg-brand-600 group-hover:text-white flex items-center justify-center transition-colors">
                            <i class="fa-solid fa-database text-2xl"></i>
                        </div>
                        <span class="px-3 py-1 rounded-full bg-slate-100 text-slate-600 text-xs font-semibold">Modul 02</span>
                    </div>
                    <h3 class="text-xl font-bold text-slate-900 mb-3">Administrasi Sistem Jaringan (ASJ)</h3>
                    <p class="text-slate-600 text-sm sm:text-base leading-relaxed mb-5">
                        Membangun, mengelola, dan memelihara layanan server berbasis sistem operasi jaringan untuk kebutuhan perusahaan maupun web hosting.
                    </p>
                    <ul class="space-y-2.5 text-sm text-slate-700">
                        <li class="flex items-center gap-2.5">
                            <i class="fa-solid fa-check text-brand-600 text-xs"></i>
                            <span>Instalasi & Konfigurasi Linux Server (Debian / Ubuntu Server)</span>
                        </li>
                        <li class="flex items-center gap-2.5">
                            <i class="fa-solid fa-check text-brand-600 text-xs"></i>
                            <span>Implementasi DHCP, DNS, Web Server (Apache/Nginx), & Database</span>
                        </li>
                        <li class="flex items-center gap-2.5">
                            <i class="fa-solid fa-check text-brand-600 text-xs"></i>
                            <span>Manajemen Control Panel Hosting, FTP, Mail Server & Virtualisasi</span>
                        </li>
                    </ul>
                </div>

                <!-- Kompetensi 3 -->
                <div class="group bg-white rounded-2xl p-7 sm:p-8 border border-slate-200/90 shadow-sm hover:shadow-xl hover:border-brand-300 transition-all duration-300">
                    <div class="flex items-start justify-between mb-6">
                        <div class="w-14 h-14 rounded-2xl bg-brand-50 text-brand-600 group-hover:bg-brand-600 group-hover:text-white flex items-center justify-center transition-colors">
                            <i class="fa-solid fa-tower-broadcast text-2xl"></i>
                        </div>
                        <span class="px-3 py-1 rounded-full bg-slate-100 text-slate-600 text-xs font-semibold">Modul 03</span>
                    </div>
                    <h3 class="text-xl font-bold text-slate-900 mb-3">Teknologi Layanan Jaringan (TLJ)</h3>
                    <p class="text-slate-600 text-sm sm:text-base leading-relaxed mb-5">
                        Menguasai teknologi transmisi data modern berbasis serat optik (Fiber Optic) dan komunikasi suara berbasis IP.
                    </p>
                    <ul class="space-y-2.5 text-sm text-slate-700">
                        <li class="flex items-center gap-2.5">
                            <i class="fa-solid fa-check text-brand-600 text-xs"></i>
                            <span>Instalasi Jaringan FTTH (Fiber To The Home) & Terminasi ODP/ONT</span>
                        </li>
                        <li class="flex items-center gap-2.5">
                            <i class="fa-solid fa-check text-brand-600 text-xs"></i>
                            <span>Penyambungan Kabel Serat Optik (Fusion Splicing) & Uji OTDR/OPM</span>
                        </li>
                        <li class="flex items-center gap-2.5">
                            <i class="fa-solid fa-check text-brand-600 text-xs"></i>
                            <span>Konfigurasi Server VoIP (Voice over IP) & Sistem Komunikasi Digital</span>
                        </li>
                    </ul>
                </div>

                <!-- Kompetensi 4 -->
                <div class="group bg-white rounded-2xl p-7 sm:p-8 border border-slate-200/90 shadow-sm hover:shadow-xl hover:border-brand-300 transition-all duration-300">
                    <div class="flex items-start justify-between mb-6">
                        <div class="w-14 h-14 rounded-2xl bg-brand-50 text-brand-600 group-hover:bg-brand-600 group-hover:text-white flex items-center justify-center transition-colors">
                            <i class="fa-solid fa-user-shield text-2xl"></i>
                        </div>
                        <span class="px-3 py-1 rounded-full bg-slate-100 text-slate-600 text-xs font-semibold">Modul 04</span>
                    </div>
                    <h3 class="text-xl font-bold text-slate-900 mb-3">Keamanan Jaringan & Troubleshooting</h3>
                    <p class="text-slate-600 text-sm sm:text-base leading-relaxed mb-5">
                        Mampu mengamankan infrastruktur TI dari ancaman siber serta mendiagnosis kerusakan perangkat keras maupun lunak secara cepat.
                    </p>
                    <ul class="space-y-2.5 text-sm text-slate-700">
                        <li class="flex items-center gap-2.5">
                            <i class="fa-solid fa-check text-brand-600 text-xs"></i>
                            <span>Konfigurasi Firewall, NAT, VPN (PPTP/L2TP/WireGuard), & Proxy</span>
                        </li>
                        <li class="flex items-center gap-2.5">
                            <i class="fa-solid fa-check text-brand-600 text-xs"></i>
                            <span>Perakitan Komputer, Instalasi OS, BIOS, & Perawatan Hardware</span>
                        </li>
                        <li class="flex items-center gap-2.5">
                            <i class="fa-solid fa-check text-brand-600 text-xs"></i>
                            <span>Monitoring Trafik Jaringan & Analisis Gangguan Konektivitas</span>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- 5. FASILITAS LABORATORIUM & PRAKTIKUM -->
    <section id="fasilitas" class="py-20 lg:py-28 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex flex-col md:flex-row md:items-end justify-between mb-14 gap-6">
                <div class="max-w-2xl">
                    <span class="inline-block px-3.5 py-1.5 rounded-lg bg-brand-50 text-brand-700 text-xs font-bold uppercase tracking-wider mb-3">
                        Sarana & Prasarana
                    </span>
                    <h2 class="text-3xl sm:text-4xl font-extrabold text-slate-900 tracking-tight">
                        Fasilitas Laboratorium & Perangkat Praktikum
                    </h2>
                </div>
                <p class="text-slate-600 text-sm sm:text-base max-w-md">
                    Menunjang pembelajaran berbasis praktik langsung dengan peralatan standar industri jaringan komputer modern.
                </p>
            </div>

            <!-- Grid Kartu Fasilitas -->
            <div class="grid grid-cols-1 lg:grid-cols-3 gap-8">
                <!-- Fasilitas 1 -->
                <div class="rounded-2xl overflow-hidden bg-slate-50 border border-slate-200 flex flex-col">
                    <div class="h-56 overflow-hidden relative bg-slate-200">
                        <img src="https://images.unsplash.com/photo-1591799264318-7e6ef8ddb7ea?auto=format&fit=crop&w=800&q=80" 
                             onerror="this.src='https://placehold.co/800x500/1e293b/ffffff?text=Lab+Perakitan+%26+PC'" 
                             alt="Lab Perakitan dan Troubleshooting PC" 
                             class="w-full h-full object-cover hover:scale-105 transition-transform duration-500">
                        <span class="absolute top-4 left-4 px-3 py-1 rounded-lg bg-slate-900/85 text-white text-xs font-semibold backdrop-blur-sm">
                            Hardware & Software
                        </span>
                    </div>
                    <div class="p-6 flex-1 flex flex-col">
                        <h3 class="text-xl font-bold text-slate-900 mb-2">Lab Perakitan & Troubleshooting PC</h3>
                        <p class="text-slate-600 text-sm leading-relaxed mb-4 flex-1">
                            Dilengkapi unit komputer praktikum bongkar-pasang, toolkit teknisi lengkap, alat ukur kelistrikan, serta workstation berkecepatan tinggi untuk simulasi jaringan.
                        </p>
                        <div class="pt-4 border-t border-slate-200 flex flex-wrap gap-2">
                            <span class="px-2.5 py-1 rounded-md bg-white border border-slate-200 text-xs font-medium text-slate-700">PC Rakitan Praktik</span>
                            <span class="px-2.5 py-1 rounded-md bg-white border border-slate-200 text-xs font-medium text-slate-700">Toolkit Lengkap</span>
                        </div>
                    </div>
                </div>

<!-- Fasilitas 2 -->
                <div class="rounded-2xl overflow-hidden bg-slate-50 border border-slate-200 flex flex-col">
                    <div class="h-56 overflow-hidden relative bg-slate-200">
                        <img src="https://images.unsplash.com/photo-1544197150-b99a580bb7a8?auto=format&fit=crop&w=800&q=80" 
                             onerror="this.src='https://placehold.co/800x500/1e3a8a/ffffff?text=Lab+Jaringan+%26+Fiber+Optik'" 
                             alt="Lab Jaringan dan Fiber Optik" 
                             class="w-full h-full object-cover hover:scale-105 transition-transform duration-500">
                        <span class="absolute top-4 left-4 px-3 py-1 rounded-lg bg-brand-600/90 text-white text-xs font-semibold backdrop-blur-sm">
                            Infrastruktur FTTH
                        </span>
                    </div>
                    <div class="p-6 flex-1 flex flex-col">
                        <h3 class="text-xl font-bold text-slate-900 mb-2">Lab Jaringan & Fiber Optik</h3>
                        <p class="text-slate-600 text-sm leading-relaxed mb-4 flex-1">
                            Fasilitas instalasi pengkabelan UTP/STP dan serat optik lengkap dengan mesin Fusion Splicer, Optical Power Meter (OPM), Visual Fault Locator (VFL), serta panel ODP.
                        </p>
                        <div class="pt-4 border-t border-slate-200 flex flex-wrap gap-2">
                            <span class="px-2.5 py-1 rounded-md bg-white border border-slate-200 text-xs font-medium text-slate-700">Fusion Splicer</span>
                            <span class="px-2.5 py-1 rounded-md bg-white border border-slate-200 text-xs font-medium text-slate-700">OPM & Cleaver</span>
                        </div>
                    </div>
                </div>

                <!-- Fasilitas 3 -->
                <div class="rounded-2xl overflow-hidden bg-slate-50 border border-slate-200 flex flex-col">
                    <div class="h-56 overflow-hidden relative bg-slate-200">
                        <img src="https://images.unsplash.com/photo-1606765962248-7ff407b51667?auto=format&fit=crop&w=800&q=80" 
                             onerror="this.src='https://placehold.co/800x500/0f172a/ffffff?text=Perangkat+MikroTik+%26+Cisco'" 
                             alt="Perangkat Router MikroTik dan Cisco" 
                             class="w-full h-full object-cover hover:scale-105 transition-transform duration-500">
                        <span class="absolute top-4 left-4 px-3 py-1 rounded-lg bg-slate-900/85 text-white text-xs font-semibold backdrop-blur-sm">
                            Enterprise Rack
                        </span>
                    </div>
                    <div class="p-6 flex-1 flex flex-col">
                        <h3 class="text-xl font-bold text-slate-900 mb-2">Perangkat Router MikroTik & Cisco</h3>
                        <p class="text-slate-600 text-sm leading-relaxed mb-4 flex-1">
                            Tersedia rack server dengan beragam seri RouterBoard MikroTik, Cisco Router & Switch Manageable, Access Point dual-band, serta koneksi internet dedicated untuk uji coba.
                        </p>
                        <div class="pt-4 border-t border-slate-200 flex flex-wrap gap-2">
                            <span class="px-2.5 py-1 rounded-md bg-white border border-slate-200 text-xs font-medium text-slate-700">MikroTik RouterBoard</span>
                            <span class="px-2.5 py-1 rounded-md bg-white border border-slate-200 text-xs font-medium text-slate-700">Cisco Switch</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 6. PROSPEK KARIR LULUSAN -->
    <section id="karir" class="py-20 lg:py-28 bg-slate-950 text-white relative overflow-hidden">
        <div class="absolute inset-0 bg-[radial-gradient(#2563eb_1px,transparent_1px)] [background-size:28px_28px] opacity-15"></div>
        
        <div class="relative max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <span class="inline-block px-3.5 py-1.5 rounded-lg bg-brand-900/80 border border-brand-700/50 text-brand-300 text-xs font-bold uppercase tracking-wider mb-3">
                    Masa Depan Lulusan
                </span>
                <h2 class="text-3xl sm:text-4xl font-extrabold tracking-tight mb-4">
                    Prospek Karir Lulusan TKJ SMK Banjar Asri
                </h2>
                <p class="text-slate-300 text-base sm:text-lg">
                    Lulusan TKJ memiliki peluang karir yang sangat luas di berbagai instansi pemerintah, perusahaan swasta, penyedia layanan internet (ISP), hingga berwirausaha mandiri.
                </p>
            </div>

            <!-- Grid Karir -->
            <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6">
                <!-- Karir 1 -->
                <div class="p-6 rounded-2xl bg-slate-900/90 border border-slate-800 hover:border-brand-500/50 transition-all">
                    <div class="w-12 h-12 rounded-xl bg-brand-600/20 text-brand-400 flex items-center justify-center mb-4">
                        <i class="fa-solid fa-route text-xl"></i>
                    </div>
                    <h3 class="text-lg font-bold text-white mb-2">Network Engineer</h3>
                    <p class="text-sm text-slate-400 leading-relaxed">
                        Merancang, membangun, dan mengoptimalkan arsitektur jaringan lokal maupun luas pada perusahaan dan penyedia layanan telekomunikasi.
                    </p>
                </div>

                <!-- Karir 2 -->
                <div class="p-6 rounded-2xl bg-slate-900/90 border border-slate-800 hover:border-brand-500/50 transition-all">
                    <div class="w-12 h-12 rounded-xl bg-cyan-500/20 text-cyan-400 flex items-center justify-center mb-4">
                        <i class="fa-solid fa-server text-xl"></i>
                    </div>
                    <h3 class="text-lg font-bold text-white mb-2">System Administrator</h3>
                    <p class="text-sm text-slate-400 leading-relaxed">
                        Mengelola operasional server, layanan cloud, pencadangan data (backup), serta menjaga keamanan dan ketersediaan sistem TI perusahaan.
                    </p>
                </div>

                <!-- Karir 3 -->
                <div class="p-6 rounded-2xl bg-slate-900/90 border border-slate-800 hover:border-brand-500/50 transition-all">
                    <div class="w-12 h-12 rounded-xl bg-emerald-500/20 text-emerald-400 flex items-center justify-center mb-4">
                        <i class="fa-solid fa-headset text-xl"></i>
                    </div>
                    <h3 class="text-lg font-bold text-white mb-2">IT Support & Helpdesk</h3>
                    <p class="text-sm text-slate-400 leading-relaxed">
                        Menangani pemeliharaan perangkat komputer kantor, instalasi perangkat lunak, serta penyelesaian kendala teknis pengguna secara profesional.
                    </p>
                </div>

                <!-- Karir 4 -->
                <div class="p-6 rounded-2xl bg-slate-900/90 border border-slate-800 hover:border-brand-500/50 transition-all">
                    <div class="w-12 h-12 rounded-xl bg-amber-500/20 text-amber-400 flex items-center justify-center mb-4">
                        <i class="fa-solid fa-wave-square text-xl"></i>
                    </div>
                    <h3 class="text-lg font-bold text-white mb-2">Teknisi Jaringan Fiber Optik</h3>
                    <p class="text-sm text-slate-400 leading-relaxed">
                        Melakukan instalasi jalur kabel serat optik, penyambungan (splicing), aktivasi pelanggan baru, dan pemeliharaan jaringan FTTH di perusahaan ISP.
                    </p>
                </div>

                <!-- Karir 5 -->
                <div class="p-6 rounded-2xl bg-slate-900/90 border border-slate-800 hover:border-brand-500/50 transition-all">
                    <div class="w-12 h-12 rounded-xl bg-purple-500/20 text-purple-400 flex items-center justify-center mb-4">
                        <i class="fa-solid fa-store text-xl"></i>
                    </div>
                    <h3 class="text-lg font-bold text-white mb-2">Wirausaha IT (Technopreneur)</h3>
                    <p class="text-sm text-slate-400 leading-relaxed">
                        Membuka usaha mandiri di bidang jasa servis komputer/laptop, penyedia layanan RT/RW Net, instalasi CCTV, hingga pengadaan perangkat TI.
                    </p>
                </div>

                <!-- Karir 6 -->
                <div class="p-6 rounded-2xl bg-gradient-to-br from-brand-700 to-brand-900 border border-brand-500/40 flex flex-col justify-between">
                    <div>
                        <div class="w-12 h-12 rounded-xl bg-white/15 text-white flex items-center justify-center mb-4">
                            <i class="fa-solid fa-graduation-cap text-xl"></i>
                        </div>
                        <h3 class="text-lg font-bold text-white mb-2">Melanjutkan Pendidikan Tinggi</h3>
                        <p class="text-sm text-brand-100 leading-relaxed">
                            Memiliki pondasi kuat untuk kuliah di jurusan Teknik Informatika, Sistem Informasi, Teknik Telekomunikasi, maupun Rekayasa Keamanan Siber.
                        </p>
                    </div>
                    <a href="#kontak" class="mt-5 inline-flex items-center gap-2 text-sm font-semibold text-white hover:underline">
                        <span>Informasi Pendaftaran & Konsultasi</span>
                        <i class="fa-solid fa-arrow-right text-xs"></i>
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- 7. FOOTER & KONTAK INFORMASI -->
    <footer id="kontak" class="bg-slate-900 text-slate-300 border-t border-slate-800">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-16">
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-12 gap-10">
                <!-- Kolom Identitas Sekolah -->
                <div class="lg:col-span-5">
                    <div class="flex items-center gap-3 mb-5">
                        <div class="w-11 h-11 rounded-xl bg-brand-600 flex items-center justify-center text-white">
                            <i class="fa-solid fa-network-wired text-lg"></i>
                        </div>
                        <div>
                            <span class="block text-lg font-extrabold text-white leading-none">TKJ SMK BANJAR ASRI</span>
                            <span class="block text-xs text-slate-400 mt-1">Kompetensi Keahlian Teknik Komputer & Jaringan</span>
                        </div>
                    </div>
                    <p class="text-sm text-slate-400 leading-relaxed mb-6 max-w-md">
                        Mewujudkan lulusan yang unggul dalam penguasaan teknologi jaringan komputer, administrasi sistem, dan siap berkontribusi nyata di dunia industri maupun masyarakat.
                    </p>
                    <!-- Ikon Sosial Media Statis -->
                    <div class="flex items-center gap-3">
                        <a href="#kontak" aria-label="Instagram" class="w-10 h-10 rounded-xl bg-slate-800 hover:bg-brand-600 text-slate-300 hover:text-white flex items-center justify-center transition-colors">
                            <i class="fa-brands fa-instagram"></i>
                        </a>
                        <a href="#kontak" aria-label="Facebook" class="w-10 h-10 rounded-xl bg-slate-800 hover:bg-brand-600 text-slate-300 hover:text-white flex items-center justify-center transition-colors">
                            <i class="fa-brands fa-facebook-f"></i>
                        </a>
                        <a href="#kontak" aria-label="YouTube" class="w-10 h-10 rounded-xl bg-slate-800 hover:bg-brand-600 text-slate-300 hover:text-white flex items-center justify-center transition-colors">
                            <i class="fa-brands fa-youtube"></i>
                        </a>
                    </div>
                </div>

                <!-- Kolom Navigasi Cepat -->
                <div class="lg:col-span-3">
                    <h4 class="text-sm font-bold uppercase tracking-wider text-white mb-4">Navigasi Halaman</h4>
                    <ul class="space-y-3 text-sm">
                        <li><a href="#beranda" class="hover:text-brand-400 transition-colors">Beranda</a></li>
                        <li><a href="#tentang" class="hover:text-brand-400 transition-colors">Tentang TKJ</a></li>
                        <li><a href="#kompetensi" class="hover:text-brand-400 transition-colors">Kompetensi & Kurikulum</a></li>
                        <li><a href="#fasilitas" class="hover:text-brand-400 transition-colors">Fasilitas Laboratorium</a></li>
                        <li><a href="#karir" class="hover:text-brand-400 transition-colors">Prospek Karir Lulusan</a></li>
                    </ul>
                </div>

                <!-- Kolom Alamat & Kontak -->
                <div class="lg:col-span-4">
                    <h4 class="text-sm font-bold uppercase tracking-wider text-white mb-4">Informasi Kontak & Lokasi</h4>
                    <ul class="space-y-4 text-sm">
                        <li class="flex items-start gap-3">
                            <i class="fa-solid fa-location-dot text-brand-400 mt-1 shrink-0"></i>
                            <span>
                                <strong class="text-white block">Kampus SMK Banjar Asri</strong>
                                Jl. Raya Banjaran - Pangalengan, Kec. Cimaung, Kabupaten Bandung, Jawa Barat 40374
                            </span>
                        </li>
                        <li class="flex items-center gap-3">
                            <i class="fa-solid fa-phone text-brand-400 shrink-0"></i>
                            <span>(022) 594-XXXX / Info Sekretariat Sekolah</span>
                        </li>
                        <li class="flex items-center gap-3">
                            <i class="fa-solid fa-envelope text-brand-400 shrink-0"></i>
                            <span>tkj@smkbanjarasri.sch.id</span>
                        </li>
                        <li class="flex items-center gap-3">
                            <i class="fa-solid fa-clock text-brand-400 shrink-0"></i>
                            <span>Senin – Jumat: 07.00 – 15.30 WIB</span>
                        </li>
                    </ul>
                </div>
            </div>

            <!-- Garis Bawah & Hak Cipta -->
            <div class="mt-12 pt-8 border-t border-slate-800/90 flex flex-col sm:flex-row items-center justify-between gap-4 text-xs text-slate-400">
                <p>&copy; <span id="current-year">2026</span> Jurusan Teknik Komputer dan Jaringan (TKJ) - SMK Banjar Asri Cimaung. Hak Cipta Dilindungi.</p>
                <p class="text-slate-500">Profil Resmi Kompetensi Keahlian TKJ</p>
            </div>
        </div>
    </footer>

    <!-- Script Interaktivitas UI Statis (Menu Mobile & Tahun Otomatis) -->
    <script>
        document.addEventListener('DOMContentLoaded', () => {
            const mobileMenuBtn = document.getElementById('mobile-menu-btn');
            const mobileMenu = document.getElementById('mobile-menu');
            const menuIcon = document.getElementById('menu-icon');
            const mobileLinks = document.querySelectorAll('.mobile-link');

            // Toggle menu mobile saat tombol hamburger diklik/disentuh
            mobileMenuBtn.addEventListener('click', () => {
                const isHidden = mobileMenu.classList.contains('hidden');
                if (isHidden) {
                    mobileMenu.classList.remove('hidden');
                    menuIcon.classList.remove('fa-bars');
                    menuIcon.classList.add('fa-xmark');
                } else {
                    mobileMenu.classList.add('hidden');
                    menuIcon.classList.remove('fa-xmark');
                    menuIcon.classList.add('fa-bars');
                }
            });

            // Tutup menu mobile otomatis setelah salah satu link navigasi dipilih
            mobileLinks.forEach(link => {
                link.addEventListener('click', () => {
                    mobileMenu.classList.add('hidden');
                    menuIcon.classList.remove('fa-xmark');
                    menuIcon.classList.add('fa-bars');
                });
            });

            // Perbarui tahun pada footer secara dinamis (tanpa penyimpanan data)
            const yearEl = document.getElementById('current-year');
            if (yearEl) {
                yearEl.textContent = new Date().getFullYear();
            }
        });
    </script>
</body>
</html>
