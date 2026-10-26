<!DOCTYPE html>
<html lang="vi" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CÔNG TY CỔ PHẦN ĐẦU TƯ XÂY DỰNG ACON | acondn.vn - Build On Trust</title>
    <meta name="description" content="Công ty Cổ phần Đầu tư Xây dựng ACON (acondn.vn) - Tổng thầu Thiết kế & Thi công xây dựng công trình Dân dụng, Công nghiệp và Hạ tầng uy tín tại Đà Nẵng & Miền Trung. Địa chỉ: 145-147 Trung Lương 14, Hòa Xuân, Đà Nẵng. Hotline: 0916.104.099">
    
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    
    <!-- Google Fonts: Inter & Montserrat (Newtecons Corporate Typography) -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&family=Montserrat:wght@600;700;800;900&display=swap" rel="stylesheet">
    
    <!-- Font Awesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">

    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                        display: ['Montserrat', 'sans-serif'],
                    },
                    colors: {
                        acon: {
                            navy: '#002B5B',      /* Màu xanh đậm chủ đạo kiểu Newtecons */
                            blue: '#0054A6',      /* Màu xanh thương hiệu ACON */
                            cyan: '#0095DA',      /* Màu xanh sáng điểm nhấn */
                            red: '#E31837',       /* Đỏ năng lượng kết cấu */
                            gold: '#F59E0B',      /* Vàng cam công trường */
                            dark: '#0A192F',      /* Nền tối kiến trúc */
                            light: '#F4F7FA'      /* Nền xám sáng hiện đại */
                        }
                    }
                }
            }
        }
    </script>

    <style>
        /* Custom Newtecons-inspired Architectural Styles & Effects */
        :root {
            --acon-navy: #002B5B;
            --acon-blue: #0054A6;
            --acon-cyan: #0095DA;
            --acon-red: #E31837;
        }

        body {
            font-family: 'Inter', sans-serif;
            overflow-x: hidden;
            background-color: #ffffff;
            color: #1e293b;
        }

        .font-display {
            font-family: 'Montserrat', sans-serif;
        }

        /* Architectural Blueprint Grid Pattern */
        .bg-blueprint {
            background-image: 
                linear-gradient(to right, rgba(0, 84, 166, 0.05) 1px, transparent 1px),
                linear-gradient(to bottom, rgba(0, 84, 166, 0.05) 1px, transparent 1px);
            background-size: 48px 48px;
        }

        .bg-blueprint-dark {
            background-image: 
                linear-gradient(to right, rgba(255, 255, 255, 0.04) 1px, transparent 1px),
                linear-gradient(to bottom, rgba(255, 255, 255, 0.04) 1px, transparent 1px);
            background-size: 56px 56px;
        }

        /* Ken Burns Hero Zoom Effect (Newtecons Hero Signature) */
        @keyframes kenBurns {
            0% { transform: scale(1) translate(0, 0); }
            50% { transform: scale(1.08) translate(-1%, -1%); }
            100% { transform: scale(1) translate(0, 0); }
        }

        .animate-kenburns {
            animation: kenBurns 18s ease-in-out infinite;
        }

        /* Reveal on Scroll Animations */
        .reveal-up {
            opacity: 0;
            transform: translateY(36px);
            transition: all 0.85s cubic-bezier(0.16, 1, 0.3, 1);
        }
        .reveal-up.active {
            opacity: 1;
            transform: translateY(0);
        }

        .reveal-left {
            opacity: 0;
            transform: translateX(-40px);
            transition: all 0.85s cubic-bezier(0.16, 1, 0.3, 1);
        }
        .reveal-left.active {
            opacity: 1;
            transform: translateX(0);
        }

        .reveal-right {
            opacity: 0;
            transform: translateX(40px);
            transition: all 0.85s cubic-bezier(0.16, 1, 0.3, 1);
        }
        .reveal-right.active {
            opacity: 1;
            transform: translateX(0);
        }

        /* Newtecons Expanding Accordion Pillars (Lĩnh vực hoạt động) */
        .service-pillar {
            transition: flex 0.6s cubic-bezier(0.25, 1, 0.5, 1), filter 0.4s ease;
        }
        @media (min-width: 1024px) {
            .service-pillars-container:hover .service-pillar {
                flex: 1;
            }
            .service-pillars-container .service-pillar:hover {
                flex: 2.4;
            }
        }

        /* Project Card Hover Effect */
        .project-card .project-overlay {
            background: linear-gradient(to top, rgba(0, 43, 91, 0.95) 0%, rgba(0, 43, 91, 0.45) 55%, rgba(0, 43, 91, 0.1) 100%);
            transition: all 0.45s ease;
        }
        .project-card:hover .project-overlay {
            background: linear-gradient(to top, rgba(0, 43, 91, 0.98) 0%, rgba(0, 84, 166, 0.75) 65%, rgba(0, 149, 218, 0.25) 100%);
        }
        .project-card img {
            transition: transform 0.75s cubic-bezier(0.16, 1, 0.3, 1);
        }
        .project-card:hover img {
            transform: scale(1.09);
        }

        /* Right Side Fixed Numbered Navigation (01 - 07 like Newtecons) */
        .side-dot-nav .nav-item .line-indicator {
            width: 16px;
            transition: all 0.35s ease;
        }
        .side-dot-nav .nav-item.active .line-indicator {
            width: 36px;
            background-color: #0095DA;
        }
        .side-dot-nav .nav-item.active .num-label {
            color: #0095DA;
            font-weight: 800;
            transform: scale(1.15);
        }

        /* Stroke Text Watermark */
        .stroke-text {
            -webkit-text-stroke: 1.5px rgba(0, 84, 166, 0.13);
            color: transparent;
        }
        .stroke-text-light {
            -webkit-text-stroke: 1.5px rgba(255, 255, 255, 0.14);
            color: transparent;
        }

        /* Custom Scrollbar */
        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-track {
            background: #0A192F;
        }
        ::-webkit-scrollbar-thumb {
            background: #0054A6;
            border-radius: 4px;
        }
        ::-webkit-scrollbar-thumb:hover {
            background: #0095DA;
        }

        /* Animated Button Sweep Effect */
        .btn-newtecons {
            position: relative;
            overflow: hidden;
            z-index: 1;
        }
        .btn-newtecons::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255,255,255,0.22), transparent);
            transition: left 0.6s ease;
            z-index: -1;
        }
        .btn-newtecons:hover::before {
            left: 100%;
        }
    </style>
</head>
<body class="selection:bg-acon-blue selection:text-white">

    <!-- ==========================================
         FLOATING RIGHT-SIDE PAGINATION (01 - 07)
         (Hiệu ứng đặc trưng của website Newtecons)
    =========================================== -->
    <aside class="side-dot-nav fixed right-4 xl:right-7 top-1/2 -translate-y-1/2 z-40 hidden md:flex flex-col gap-3 bg-acon-navy/80 backdrop-blur-md px-3 py-4 rounded-2xl border border-white/15 shadow-2xl">
        <a href="#sec-01" data-section="sec-01" class="nav-item active group flex items-center justify-end gap-2.5 py-1" title="Trang chủ">
            <span class="num-label text-xs font-display font-bold text-white/70 group-hover:text-white transition-all">01</span>
            <span class="line-indicator h-[2px] bg-white/40 rounded-full"></span>
        </a>
        <a href="#sec-02" data-section="sec-02" class="nav-item group flex items-center justify-end gap-2.5 py-1" title="Giới thiệu ACON">
            <span class="num-label text-xs font-display font-bold text-white/70 group-hover:text-white transition-all">02</span>
            <span class="line-indicator h-[2px] bg-white/40 rounded-full"></span>
        </a>
        <a href="#sec-03" data-section="sec-03" class="nav-item group flex items-center justify-end gap-2.5 py-1" title="Lĩnh vực hoạt động">
            <span class="num-label text-xs font-display font-bold text-white/70 group-hover:text-white transition-all">03</span>
            <span class="line-indicator h-[2px] bg-white/40 rounded-full"></span>
        </a>
        <a href="#sec-04" data-section="sec-04" class="nav-item group flex items-center justify-end gap-2.5 py-1" title="Dấu ấn & Năng lực">
            <span class="num-label text-xs font-display font-bold text-white/70 group-hover:text-white transition-all">04</span>
            <span class="line-indicator h-[2px] bg-white/40 rounded-full"></span>
        </a>
        <a href="#sec-05" data-section="sec-05" class="nav-item group flex items-center justify-end gap-2.5 py-1" title="Dự án tiêu biểu">
            <span class="num-label text-xs font-display font-bold text-white/70 group-hover:text-white transition-all">05</span>
            <span class="line-indicator h-[2px] bg-white/40 rounded-full"></span>
        </a>
        <a href="#sec-06" data-section="sec-06" class="nav-item group flex items-center justify-end gap-2.5 py-1" title="Tin tức Fanpage & Tuyển dụng">
            <span class="num-label text-xs font-display font-bold text-white/70 group-hover:text-white transition-all">06</span>
            <span class="line-indicator h-[2px] bg-white/40 rounded-full"></span>
        </a>
        <a href="#sec-07" data-section="sec-07" class="nav-item group flex items-center justify-end gap-2.5 py-1" title="Liên hệ">
            <span class="num-label text-xs font-display font-bold text-white/70 group-hover:text-white transition-all">07</span>
            <span class="line-indicator h-[2px] bg-white/40 rounded-full"></span>
        </a>
    </aside>

    <!-- ==========================================
         FLOATING QUICK ACTION BUTTONS (Gọi ngay / Fanpage)
    =========================================== -->
    <div class="fixed left-4 bottom-5 z-40 flex flex-col gap-3">
        <a href="tel:0916104099" class="group flex items-center gap-3 bg-acon-red text-white px-4 py-3 rounded-full shadow-lg shadow-acon-red/40 hover:bg-red-700 transition-all">
            <span class="w-8 h-8 rounded-full bg-white/20 flex items-center justify-center animate-bounce">
                <i class="fa-solid fa-phone-volume text-sm"></i>
            </span>
            <div class="pr-1">
                <span class="block text-[10px] uppercase tracking-wider text-white/80 leading-none">Hotline 24/7</span>
                <span class="font-display font-bold text-sm">0916.104.099</span>
            </div>
        </a>
        <a href="https://www.facebook.com/aconvn.construction" target="_blank" rel="noopener noreferrer" class="flex items-center gap-3 bg-[#1877F2] text-white px-4 py-2.5 rounded-full shadow-lg shadow-blue-600/30 hover:bg-blue-700 transition-all">
            <i class="fa-brands fa-facebook-f text-lg w-6 text-center"></i>
            <span class="text-xs font-semibold pr-1 hidden sm:inline">Fanpage ACON Construction</span>
        </a>
    </div>

    <!-- ==========================================
         TOP CORPORATE BAR & STICKY HEADER
    =========================================== -->
    <header id="main-header" class="fixed top-0 left-0 right-0 z-50 transition-all duration-300 bg-acon-navy/95 backdrop-blur-md border-b border-white/10">
        <!-- Top Info Bar -->
        <div class="bg-acon-dark/90 text-white/80 text-xs py-1.5 px-4 border-b border-white/10 hidden lg:block">
            <div class="max-w-7xl mx-auto flex items-center justify-between">
                <div class="flex items-center gap-6">
                    <span class="flex items-center gap-2">
                        <i class="fa-solid fa-globe text-acon-cyan"></i>
                        <strong class="text-white">acondn.vn</strong> — CÔNG TY CỔ PHẦN ĐẦU TƯ XÂY DỰNG ACON
                    </span>
                    <span class="flex items-center gap-2">
                        <i class="fa-solid fa-location-dot text-acon-red"></i>
                        145-147 Trung Lương 14, Hòa Xuân, Đà Nẵng
                    </span>
                    <span class="flex items-center gap-2">
                        <i class="fa-solid fa-certificate text-amber-400"></i>
                        Mã chứng chỉ năng lực HĐXD: <strong class="text-white">00076275</strong> | MST: <strong class="text-white">0401676571</strong>
                    </span>
                </div>
                <div class="flex items-center gap-5">
                    <a href="mailto:acon.dng@gmail.com" class="hover:text-acon-cyan transition-colors">
                        <i class="fa-regular fa-envelope mr-1"></i> acon.dng@gmail.com
                    </a>
                    <a href="https://www.facebook.com/aconvn.construction" target="_blank" rel="noopener noreferrer" class="hover:text-acon-cyan transition-colors flex items-center gap-1.5">
                        <i class="fa-brands fa-facebook text-blue-400"></i> fb.com/aconvn.construction
                    </a>
                    <div class="flex items-center gap-1.5 border-l border-white/20 pl-4 font-semibold">
                        <button onclick="switchLang('VN')" id="lang-vn" class="text-acon-cyan">VN</button>
                        <span class="text-white/30">|</span>
                        <button onclick="switchLang('EN')" id="lang-en" class="text-white/60 hover:text-white">EN</button>
                    </div>
                </div>
            </div>
        </div>

        <!-- Main Navbar -->
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 h-20 flex items-center justify-between">
            <!-- ACON Official Brand Logo (Chuẩn nhận diện ΛCON Construction trên Fanpage + Hỗ trợ tải logo tuỳ chỉnh) -->
            <div class="flex items-center gap-3">
                <a href="#sec-01" class="flex items-center gap-3 group" title="CÔNG TY CỔ PHẦN ĐẦU TƯ XÂY DỰNG ACON - acondn.vn">
                    <div id="logo-container" class="relative w-14 h-14 rounded-xl bg-white flex items-center justify-center shadow-md p-1.5 border-2 border-acon-cyan/40 group-hover:border-acon-cyan transition-all overflow-hidden">
                        <!-- Custom Image Logo if user uploads/links from Fanpage -->
                        <img id="custom-logo-img" src="" alt="ACON Logo" class="hidden w-full h-full object-contain" />
                        <!-- Architectural Vector Logo matching Fanpage ΛCON Construction -->
                        <svg id="default-logo-svg" viewBox="0 0 120 100" class="w-full h-full">
                            <defs>
                                <linearGradient id="aconBlueGrad" x1="0%" y1="0%" x2="100%" y2="100%">
                                    <stop offset="0%" stop-color="#002B5B" />
                                    <stop offset="55%" stop-color="#0054A6" />
                                    <stop offset="100%" stop-color="#0095DA" />
                                </linearGradient>
                                <linearGradient id="aconRedGrad" x1="0%" y1="0%" x2="100%" y2="100%">
                                    <stop offset="0%" stop-color="#E31837" />
                                    <stop offset="100%" stop-color="#F59E0B" />
                                </linearGradient>
                            </defs>
                            <!-- Biểu tượng đỉnh tháp chữ A (Λ) kiến trúc đặc trưng của ACON -->
                            <polygon points="60,6 16,74 35,74 60,33 85,74 104,74" fill="url(#aconBlueGrad)" />
                            <polygon points="60,42 43,74 77,74" fill="url(#aconRedGrad)" />
                            <!-- Dòng chữ ΛCON CONSTRUCTION -->
                            <text x="60" y="94" text-anchor="middle" font-family="Montserrat, sans-serif" font-weight="900" font-size="18" fill="#002B5B" letter-spacing="2">ΛCON</text>
                        </svg>
                    </div>
                    <div>
                        <div class="flex items-center gap-1.5">
                            <span class="font-display font-black text-2xl sm:text-3xl tracking-wider text-white leading-none">
                                <span class="text-acon-cyan">Λ</span>CON
                            </span>
                            <span class="text-[10px] font-display font-bold uppercase px-1.5 py-0.5 rounded bg-acon-red text-white tracking-widest">JSC</span>
                        </div>
                        <span class="block text-[10px] sm:text-[11px] font-semibold tracking-widest text-white/80 uppercase mt-0.5">
                            Đầu Tư Xây Dựng ACON • <span class="text-acon-cyan">acondn.vn</span>
                        </span>
                    </div>
                </a>
            </div>

            <!-- Desktop Menu Links -->
            <nav class="hidden xl:flex items-center gap-7 text-sm font-semibold text-white/90">
                <a href="#sec-02" class="hover:text-acon-cyan transition-colors py-2 relative after:content-[''] after:absolute after:bottom-0 after:left-0 after:w-0 after:h-0.5 after:bg-acon-cyan hover:after:w-full after:transition-all">GIỚI THIỆU</a>
                <a href="#sec-03" class="hover:text-acon-cyan transition-colors py-2 relative after:content-[''] after:absolute after:bottom-0 after:left-0 after:w-0 after:h-0.5 after:bg-acon-cyan hover:after:w-full after:transition-all">LĨNH VỰC HOẠT ĐỘNG</a>
                <a href="#sec-05" class="hover:text-acon-cyan transition-colors py-2 relative after:content-[''] after:absolute after:bottom-0 after:left-0 after:w-0 after:h-0.5 after:bg-acon-cyan hover:after:w-full after:transition-all">DỰ ÁN TIÊU BIỂU</a>
                <a href="#sec-04" class="hover:text-acon-cyan transition-colors py-2 relative after:content-[''] after:absolute after:bottom-0 after:left-0 after:w-0 after:h-0.5 after:bg-acon-cyan hover:after:w-full after:transition-all">NĂNG LỰC & CHỨNG CHỈ</a>
                <a href="#sec-06" class="hover:text-acon-cyan transition-colors py-2 relative after:content-[''] after:absolute after:bottom-0 after:left-0 after:w-0 after:h-0.5 after:bg-acon-cyan hover:after:w-full after:transition-all">TIN TỨC & TUYỂN DỤNG</a>
                <a href="#sec-07" class="hover:text-acon-cyan transition-colors py-2 relative after:content-[''] after:absolute after:bottom-0 after:left-0 after:w-0 after:h-0.5 after:bg-acon-cyan hover:after:w-full after:transition-all">LIÊN HỆ</a>
            </nav>

            <!-- Action Buttons & Newtecons-style Fullscreen Menu Trigger -->
            <div class="flex items-center gap-3">
                <button onclick="openLogoModal()" class="hidden sm:inline-flex items-center gap-2 text-xs font-semibold text-white/90 bg-white/10 hover:bg-white/20 border border-white/20 px-3.5 py-2.5 rounded-xl transition-all" title="Cập nhật ảnh Logo hoặc ảnh dự án từ Fanpage">
                    <i class="fa-solid fa-images text-acon-cyan"></i>
                    <span class="hidden md:inline">Đồng bộ Fanpage</span>
                </button>

                <a href="tel:0916104099" class="hidden md:inline-flex items-center gap-2 bg-acon-cyan hover:bg-sky-500 text-white font-display font-bold text-xs uppercase tracking-wider px-4 py-3 rounded-xl shadow-lg shadow-acon-cyan/25 transition-all btn-newtecons">
                    <i class="fa-solid fa-phone"></i>
                    0916.104.099
                </a>

                <!-- Hamburger Button (Mở Mega Menu toàn màn hình giống Newtecons) -->
                <button onclick="toggleMegaMenu()" class="w-11 h-11 rounded-xl bg-white/10 hover:bg-acon-cyan text-white flex flex-col items-center justify-center gap-1.5 transition-all border border-white/15" aria-label="Menu">
                    <span class="w-5 h-0.5 bg-white rounded-full"></span>
                    <span class="w-3.5 h-0.5 bg-white rounded-full self-end mr-3"></span>
                    <span class="w-5 h-0.5 bg-white rounded-full"></span>
                </button>
            </div>
        </div>
    </header>

    <!-- ==========================================
         NEWTECONS-STYLE FULLSCREEN OVERLAY MEGA MENU
    =========================================== -->
    <div id="mega-menu" class="fixed inset-0 z-50 bg-acon-dark/98 backdrop-blur-xl hidden opacity-0 transition-opacity duration-300 bg-blueprint-dark overflow-y-auto">
        <div class="max-w-7xl mx-auto px-6 py-8 min-h-screen flex flex-col justify-between">
            <!-- Top Bar inside Overlay -->
            <div class="flex items-center justify-between border-b border-white/10 pb-6">
                <div class="flex items-center gap-3">
                    <div class="w-12 h-12 rounded-xl bg-white flex items-center justify-center p-1.5">
                        <span class="font-display font-black text-acon-navy text-lg"><span class="text-acon-red">Λ</span>CON</span>
                    </div>
                    <div>
                        <h3 class="font-display font-bold text-white text-lg">CÔNG TY CỔ PHẦN ĐẦU TƯ XÂY DỰNG ACON</h3>
                        <p class="text-xs text-acon-cyan">acondn.vn • Build On Trust • Kiến Tạo Giá Trị Bền Vững</p>
                    </div>
                </div>
                <button onclick="toggleMegaMenu()" class="w-12 h-12 rounded-full bg-white/10 hover:bg-acon-red text-white flex items-center justify-center text-xl transition-all">
                    <i class="fa-solid fa-xmark"></i>
                </button>
            </div>

            <!-- Center Grid Navigation -->
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-10 py-10 my-auto">
                <div class="lg:col-span-7 space-y-4">
                    <p class="text-xs font-display uppercase tracking-widest text-acon-cyan mb-4">DANH MỤC ĐIỀU HƯỚNG</p>
                    <a href="#sec-01" onclick="toggleMegaMenu()" class="group flex items-baseline gap-5 py-2 border-b border-white/10 hover:border-acon-cyan transition-all">
                        <span class="text-sm font-display font-bold text-acon-cyan">01</span>
                        <span class="text-2xl sm:text-4xl font-display font-extrabold text-white group-hover:text-acon-cyan group-hover:translate-x-3 transition-all">TRANG CHỦ ACON</span>
                    </a>
                    <a href="#sec-02" onclick="toggleMegaMenu()" class="group flex items-baseline gap-5 py-2 border-b border-white/10 hover:border-acon-cyan transition-all">
                        <span class="text-sm font-display font-bold text-acon-cyan">02</span>
                        <span class="text-2xl sm:text-4xl font-display font-extrabold text-white group-hover:text-acon-cyan group-hover:translate-x-3 transition-all">GIỚI THIỆU & LỊCH SỬ PHÁT TRIỂN</span>
                    </a>
                    <a href="#sec-03" onclick="toggleMegaMenu()" class="group flex items-baseline gap-5 py-2 border-b border-white/10 hover:border-acon-cyan transition-all">
                        <span class="text-sm font-display font-bold text-acon-cyan">03</span>
                        <span class="text-2xl sm:text-4xl font-display font-extrabold text-white group-hover:text-acon-cyan group-hover:translate-x-3 transition-all">LĨNH VỰC HOẠT ĐỘNG (D&B)</span>
                    </a>
                    <a href="#sec-04" onclick="toggleMegaMenu()" class="group flex items-baseline gap-5 py-2 border-b border-white/10 hover:border-acon-cyan transition-all">
                        <span class="text-sm font-display font-bold text-acon-cyan">04</span>
                        <span class="text-2xl sm:text-4xl font-display font-extrabold text-white group-hover:text-acon-cyan group-hover:translate-x-3 transition-all">CHỨNG CHỈ NĂNG LỰC (00076275)</span>
                    </a>
                    <a href="#sec-05" onclick="toggleMegaMenu()" class="group flex items-baseline gap-5 py-2 border-b border-white/10 hover:border-acon-cyan transition-all">
                        <span class="text-sm font-display font-bold text-acon-cyan">05</span>
                        <span class="text-2xl sm:text-4xl font-display font-extrabold text-white group-hover:text-acon-cyan group-hover:translate-x-3 transition-all">DỰ ÁN TIÊU BIỂU</span>
                    </a>
                    <a href="#sec-06" onclick="toggleMegaMenu()" class="group flex items-baseline gap-5 py-2 border-b border-white/10 hover:border-acon-cyan transition-all">
                        <span class="text-sm font-display font-bold text-acon-cyan">06</span>
                        <span class="text-2xl sm:text-4xl font-display font-extrabold text-white group-hover:text-acon-cyan group-hover:translate-x-3 transition-all">TIN TỨC FANPAGE & TUYỂN DỤNG</span>
                    </a>
                    <a href="#sec-07" onclick="toggleMegaMenu()" class="group flex items-baseline gap-5 py-2 border-b border-white/10 hover:border-acon-cyan transition-all">
                        <span class="text-sm font-display font-bold text-acon-cyan">07</span>
                        <span class="text-2xl sm:text-4xl font-display font-extrabold text-white group-hover:text-acon-cyan group-hover:translate-x-3 transition-all">LIÊN HỆ & ĐẤU THẦU</span>
                    </a>
                </div>

                <!-- Right Column: Corporate Info Card -->
                <div class="lg:col-span-5 bg-white/5 border border-white/10 rounded-3xl p-8 flex flex-col justify-between">
                    <div>
                        <span class="inline-block px-3 py-1 rounded-full bg-acon-cyan/20 text-acon-cyan text-xs font-bold uppercase tracking-wider mb-4">
                            Thông tin chính thức
                        </span>
                        <h4 class="font-display font-bold text-xl text-white mb-6">
                            CÔNG TY CỔ PHẦN ĐẦU TƯ XÂY DỰNG ACON
                        </h4>
                        <ul class="space-y-4 text-sm text-white/80">
                            <li class="flex items-start gap-3">
                                <i class="fa-solid fa-location-dot text-acon-cyan mt-1"></i>
                                <span><strong>Trụ sở văn phòng:</strong> 145-147 Trung Lương 14, Phường Hòa Xuân, Quận Cẩm Lệ, TP. Đà Nẵng</span>
                            </li>
                            <li class="flex items-start gap-3">
                                <i class="fa-solid fa-phone-volume text-acon-cyan mt-1"></i>
                                <span><strong>Hotline:</strong> <a href="tel:0916104099" class="text-white font-bold hover:text-acon-cyan">0916.104.099</a> | Điện thoại VP: 02363.789.769</span>
                            </li>
                            <li class="flex items-start gap-3">
                                <i class="fa-solid fa-envelope text-acon-cyan mt-1"></i>
                                <span><strong>Email:</strong> acon.dng@gmail.com | contact@acondn.vn</span>
                            </li>
                            <li class="flex items-start gap-3">
                                <i class="fa-solid fa-globe text-acon-cyan mt-1"></i>
                                <span><strong>Website:</strong> https://acondn.vn</span>
                            </li>
                            <li class="flex items-start gap-3">
                                <i class="fa-brands fa-facebook text-acon-cyan mt-1"></i>
                                <span><strong>Fanpage:</strong> <a href="https://www.facebook.com/aconvn.construction" target="_blank" rel="noopener noreferrer" class="underline hover:text-acon-cyan">facebook.com/aconvn.construction</a></span>
                            </li>
                        </ul>
                    </div>

                    <div class="mt-8 pt-6 border-t border-white/10 flex flex-wrap gap-3">
                        <a href="https://www.facebook.com/aconvn.construction" target="_blank" rel="noopener noreferrer" class="flex-1 text-center bg-[#1877F2] hover:bg-blue-600 text-white font-semibold py-3 px-4 rounded-xl text-sm transition-all">
                            <i class="fa-brands fa-facebook-f mr-2"></i>Mở Fanpage ACON
                        </a>
                        <button onclick="toggleMegaMenu(); openProfileModal();" class="flex-1 text-center bg-acon-cyan hover:bg-sky-500 text-white font-semibold py-3 px-4 rounded-xl text-sm transition-all">
                            <i class="fa-solid fa-file-pdf mr-2"></i>Hồ Sơ Năng Lực
                        </button>
                    </div>
                </div>
            </div>

            <!-- Bottom Copyright inside Overlay -->
            <div class="text-xs text-white/50 flex flex-wrap justify-between items-center pt-4 border-t border-white/10">
                <span>© 2015 - 2026 CÔNG TY CỔ PHẦN ĐẦU TƯ XÂY DỰNG ACON (acondn.vn). All rights reserved.</span>
                <span>Giám đốc đại diện pháp luật: Ông Huỳnh Bá Quý • MST: 0401676571</span>
            </div>
        </div>
    </div>

    <!-- ==========================================
         SECTION 01: FULLSCREEN HERO SLIDER (NEWTECONS STYLE)
    =========================================== -->
    <section id="sec-01" class="relative min-h-screen w-full overflow-hidden bg-acon-dark flex items-center pt-24 pb-16">
        <!-- Dynamic Hero Background Slides -->
        <div id="hero-slides" class="absolute inset-0 z-0">
            <!-- Slide 1 -->
            <div class="hero-slide absolute inset-0 transition-opacity duration-1000 opacity-100">
                <img src="https://images.unsplash.com/photo-1541888946425-d09bb18086f6?auto=format&fit=crop&w=1920&q=85" 
                     onerror="this.src='https://placehold.co/1920x1080/002B5B/FFFFFF?text=ACON+CONSTRUCTION+DA+NANG'"
                     alt="Tổng thầu Thiết kế & Thi công ACON Construction Đà Nẵng" 
                     class="w-full h-full object-cover animate-kenburns" />
                <div class="absolute inset-0 bg-gradient-to-r from-acon-dark/95 via-acon-navy/80 to-acon-dark/40"></div>
            </div>
            <!-- Slide 2 -->
            <div class="hero-slide absolute inset-0 transition-opacity duration-1000 opacity-0">
                <img src="https://images.unsplash.com/photo-1503387762-592deb58ef4e?auto=format&fit=crop&w=1920&q=85" 
                     onerror="this.src='https://placehold.co/1920x1080/0054A6/FFFFFF?text=DESIGN+AND+BUILD+ACON'"
                     alt="Kiến tạo những công trình biểu tượng bền vững" 
                     class="w-full h-full object-cover animate-kenburns" />
                <div class="absolute inset-0 bg-gradient-to-r from-acon-dark/95 via-acon-navy/80 to-acon-dark/40"></div>
            </div>
            <!-- Slide 3 -->
            <div class="hero-slide absolute inset-0 transition-opacity duration-1000 opacity-0">
                <img src="https://images.unsplash.com/photo-1581094794329-c8112a89af12?auto=format&fit=crop&w=1920&q=85" 
                     onerror="this.src='https://placehold.co/1920x1080/0A192F/FFFFFF?text=CONG+TRINH+CONG+NGHIEP+VA+DAN+DUNG'"
                     alt="Thi công công trình Dân dụng và Công nghiệp Hạng II" 
                     class="w-full h-full object-cover animate-kenburns" />
                <div class="absolute inset-0 bg-gradient-to-r from-acon-dark/95 via-acon-navy/80 to-acon-dark/40"></div>
            </div>
        </div>

        <!-- Architectural Grid Overlay -->
        <div class="absolute inset-0 bg-blueprint-dark pointer-events-none z-0"></div>

        <!-- Giant Stroke Text Watermark -->
        <div class="absolute bottom-24 right-10 pointer-events-none select-none hidden lg:block z-0">
            <span class="font-display font-black text-[130px] leading-none stroke-text-light tracking-tighter">ACON D&B</span>
        </div>

        <!-- Hero Content Container -->
        <div class="relative z-10 max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 w-full my-auto">
            <div class="max-w-3xl">
                <!-- Badge -->
                <div class="inline-flex items-center gap-2.5 px-4 py-2 rounded-full bg-white/10 backdrop-blur-md border border-white/20 text-white text-xs font-semibold uppercase tracking-widest mb-6">
                    <span class="w-2.5 h-2.5 rounded-full bg-acon-cyan animate-ping"></span>
                    <span>BUILD ON TRUST • KIẾN TẠO GIÁ TRỊ VỮNG BỀN</span>
                </div>

                <!-- Dynamic Slide Headline -->
                <h1 id="hero-title" class="font-display font-black text-3xl sm:text-5xl lg:text-6xl text-white leading-[1.12] tracking-tight mb-6 transition-all duration-500">
                    CÔNG TY CỔ PHẦN <br/>
                    <span class="text-transparent bg-clip-text bg-gradient-to-r from-acon-cyan via-sky-300 to-white">ĐẦU TƯ XÂY DỰNG ACON</span>
                </h1>

                <p id="hero-subtitle" class="text-base sm:text-lg text-white/85 leading-relaxed mb-8 max-w-2xl font-normal">
                    Sự tin tưởng của Chủ đầu tư là chuẩn mực cho giá trị của ACON Construction. Chúng tôi tự hào là Tổng thầu Thiết kế & Thi công (Design & Build) các công trình Dân dụng, Thương mại, Khách sạn và Công nghiệp uy tín hàng đầu tại Đà Nẵng & khu vực Miền Trung.
                </p>

                <!-- CTA Buttons -->
                <div class="flex flex-wrap items-center gap-4 mb-12">
                    <a href="#sec-05" class="btn-newtecons inline-flex items-center gap-3 bg-acon-cyan hover:bg-sky-500 text-white font-display font-bold text-sm uppercase tracking-wider px-7 py-4 rounded-2xl shadow-xl shadow-acon-cyan/30 transition-all">
                        <span>Khám phá Dự án ACON</span>
                        <i class="fa-solid fa-arrow-right"></i>
                    </a>
                    <button onclick="openProfileModal()" class="inline-flex items-center gap-3 bg-white/10 hover:bg-white/20 backdrop-blur-md text-white font-display font-bold text-sm uppercase tracking-wider px-7 py-4 rounded-2xl border border-white/25 transition-all">
                        <i class="fa-solid fa-award text-amber-400"></i>
                        <span>Hồ sơ năng lực (00076275)</span>
                    </button>
                </div>

                <!-- Slide Controls & Progress Indicators (Newtecons Hero Bottom Controls) -->
                <div class="flex items-center gap-6 pt-4 border-t border-white/15">
                    <button onclick="setHeroSlide(0)" class="hero-dot group flex items-center gap-2 text-left">
                        <span class="text-xs font-display font-bold text-acon-cyan">01</span>
                        <div class="w-14 sm:w-20 h-1 bg-white/20 rounded-full overflow-hidden">
                            <div id="hero-bar-0" class="h-full bg-acon-cyan w-full transition-all duration-500"></div>
                        </div>
                        <span class="hidden sm:inline text-xs text-white/80 group-hover:text-white">Tổng thầu D&B</span>
                    </button>
                    <button onclick="setHeroSlide(1)" class="hero-dot group flex items-center gap-2 text-left">
                        <span class="text-xs font-display font-bold text-white/60">02</span>
                        <div class="w-14 sm:w-20 h-1 bg-white/20 rounded-full overflow-hidden">
                            <div id="hero-bar-1" class="h-full bg-acon-cyan w-0 transition-all duration-500"></div>
                        </div>
                        <span class="hidden sm:inline text-xs text-white/80 group-hover:text-white">Công trình Biểu tượng</span>
                    </button>
                    <button onclick="setHeroSlide(2)" class="hero-dot group flex items-center gap-2 text-left">
                        <span class="text-xs font-display font-bold text-white/60">03</span>
                        <div class="w-14 sm:w-20 h-1 bg-white/20 rounded-full overflow-hidden">
                            <div id="hero-bar-2" class="h-full bg-acon-cyan w-0 transition-all duration-500"></div>
                        </div>
                        <span class="hidden sm:inline text-xs text-white/80 group-hover:text-white">Chuẩn mực Kỹ - Mỹ thuật</span>
                    </button>
                </div>
            </div>
        </div>

        <!-- Bottom Quick Info Bar -->
        <div class="absolute bottom-0 left-0 right-0 z-10 bg-acon-navy/85 backdrop-blur-md border-t border-white/10 py-3.5 px-4 hidden md:block">
            <div class="max-w-7xl mx-auto flex items-center justify-between text-xs text-white/85">
                <div class="flex items-center gap-8">
                    <span><strong class="text-acon-cyan uppercase">Tên viết tắt:</strong> ACON INVESTMENT CONSTRUCTION.,JSC</span>
                    <span><strong class="text-acon-cyan uppercase">Trụ sở:</strong> 145-147 Trung Lương 14, P. Hòa Xuân, Đà Nẵng</span>
                    <span><strong class="text-acon-cyan uppercase">Hotline:</strong> 0916.104.099 - 02363.789.769</span>
                </div>
                <a href="#sec-02" class="flex items-center gap-2 text-acon-cyan font-bold hover:underline">
                    <span>Cuộn xuống khám phá</span>
                    <i class="fa-solid fa-angles-down animate-bounce"></i>
                </a>
            </div>
        </div>
    </section>

    <!-- ==========================================
         SECTION 02: GIỚI THIỆU ACON ("BUILD ON TRUST" & LỊCH SỬ HÌNH THÀNH)
         (Thiết kế bố cục bất đối xứng + Timeline giống trang mẫu Newtecons)
    =========================================== -->
    <section id="sec-02" class="relative py-24 lg:py-32 bg-white bg-blueprint overflow-hidden">
        <!-- Background Decorative Watermark -->
        <div class="absolute top-10 left-6 pointer-events-none select-none hidden lg:block">
            <span class="font-display font-black text-[110px] stroke-text leading-none">ABOUT ACON</span>
        </div>

        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 lg:gap-16 items-center">
                <!-- Left Column: Story & Philosophy -->
                <div class="lg:col-span-6 reveal-left">
                    <div class="flex items-center gap-3 mb-4">
                        <span class="w-10 h-1 bg-acon-blue rounded-full"></span>
                        <span class="font-display font-bold text-xs uppercase tracking-widest text-acon-blue">02 • VỀ CHÚNG TÔI</span>
                    </div>

                    <h2 class="font-display font-black text-3xl sm:text-4xl lg:text-5xl text-acon-navy leading-tight mb-4">
                        ACON CONSTRUCTION
                    </h2>
                    <p class="font-display font-bold text-lg text-acon-cyan mb-6">
                        “Build on Trust – Sự tin tưởng của bạn là chuẩn mực cho giá trị của chúng tôi”
                    </p>

                    <div class="space-y-4 text-slate-600 leading-relaxed text-base">
                        <p>
                            Được thành lập từ ngày <strong>14/05/2015</strong> (Mã số thuế: <strong>0401676571</strong>), dưới sự dẫn dắt của Giám đốc – Người đại diện pháp luật <strong>Ông Huỳnh Bá Quý</strong> cùng đội ngũ kỹ sư, kiến trúc sư tâm huyết, <strong>CÔNG TY CỔ PHẦN ĐẦU TƯ XÂY DỰNG ACON</strong> đã vươn mình trở thành một trong những thương hiệu nhà thầu xây dựng uy tín tại Đà Nẵng và khu vực Miền Trung.
                        </p>
                        <p>
                            Với triết lý <strong>“Uy tín – Chuyên nghiệp – Bền vững”</strong>, ACON sở hữu Chứng chỉ năng lực hoạt động xây dựng số <strong>00076275</strong> do cơ quan có thẩm quyền cấp (có hiệu lực đến năm 2033), đáp ứng đầy đủ năng lực <strong>Thiết kế, Thẩm tra thiết kế, Tư vấn Quản lý dự án, Tư vấn Giám sát và Thi công xây dựng công trình Dân dụng (Hạng II) & Nhà công nghiệp</strong>.
                        </p>
                    </div>

                    <!-- 3 Signature Action Cards like Newtecons ("Lịch sử hình thành", "Company Profile", "Hệ giá trị") -->
                    <div class="grid grid-cols-1 sm:grid-cols-3 gap-4 mt-8">
                        <button onclick="switchAboutTab('history')" id="tab-btn-history" class="about-tab-btn group text-left p-5 rounded-2xl bg-acon-navy text-white shadow-lg transition-all">
                            <i class="fa-solid fa-clock-rotate-left text-2xl text-acon-cyan mb-3 block"></i>
                            <span class="font-display font-extrabold text-xs uppercase tracking-wider block">LỊCH SỬ</span>
                            <span class="font-display font-bold text-sm">HÌNH THÀNH</span>
                        </button>

                        <button onclick="switchAboutTab('values')" id="tab-btn-values" class="about-tab-btn group text-left p-5 rounded-2xl bg-slate-100 hover:bg-acon-navy hover:text-white text-acon-navy transition-all">
                            <i class="fa-solid fa-gem text-2xl text-acon-cyan mb-3 block"></i>
                            <span class="font-display font-extrabold text-xs uppercase tracking-wider block">TẦM NHÌN &</span>
                            <span class="font-display font-bold text-sm">GIÁ TRỊ CỐT LÕI</span>
                        </button>

                        <button onclick="openProfileModal()" class="group text-left p-5 rounded-2xl bg-slate-100 hover:bg-acon-red hover:text-white text-acon-navy transition-all">
                            <i class="fa-solid fa-file-shield text-2xl text-acon-red group-hover:text-white mb-3 block"></i>
                            <span class="font-display font-extrabold text-xs uppercase tracking-wider block">COMPANY</span>
                            <span class="font-display font-bold text-sm">PROFILE & HỒ SƠ</span>
                        </button>
                    </div>
                </div>

                <!-- Right Column: Visual Collage & Interactive Milestone Box -->
                <div class="lg:col-span-6 reveal-right">
                    <div class="relative">
                        <!-- Main Architectural Image -->
                        <div class="rounded-3xl overflow-hidden shadow-2xl border-4 border-white relative">
                            <img src="https://images.unsplash.com/photo-1504307651254-35680f356dfd?auto=format&fit=crop&w=1000&q=85" 
                                 onerror="this.src='https://placehold.co/900x650/002B5B/FFFFFF?text=ACON+CONSTRUCTION+TEAM'"
                                 alt="Đội ngũ kỹ sư Công ty Cổ phần Đầu tư Xây dựng ACON" 
                                 class="w-full h-[420px] object-cover" />
                            <div class="absolute inset-0 bg-gradient-to-t from-acon-navy/90 via-acon-navy/20 to-transparent"></div>
                            <div class="absolute bottom-6 left-6 right-6 text-white">
                                <span class="px-3 py-1 rounded-full bg-acon-cyan text-xs font-bold uppercase tracking-wider">Trụ sở Đà Nẵng</span>
                                <h3 class="font-display font-bold text-xl mt-2">145-147 Trung Lương 14, Phường Hòa Xuân, TP. Đà Nẵng</h3>
                                <p class="text-xs text-white/80 mt-1">Không gian làm việc mở, hiện đại của đội ngũ Kỹ sư, Kiến trúc sư & Chuyên viên QS ACON</p>
                            </div>
                        </div>

                        <!-- Dynamic Tab Content Card Overlapping Bottom -->
                        <div id="about-tab-content" class="mt-6 bg-white rounded-3xl p-6 sm:p-8 shadow-xl border border-slate-200/80">
                            <!-- Default: History Timeline (2015 - 2026) -->
                            <div id="tab-panel-history" class="space-y-4">
                                <div class="flex items-center justify-between border-b border-slate-100 pb-3">
                                    <h4 class="font-display font-extrabold text-acon-navy text-base uppercase tracking-wider">
                                        Chặng đường phát triển ACON (2015 – 2026)
                                    </h4>
                                    <span class="text-xs font-bold text-acon-blue bg-blue-50 px-3 py-1 rounded-full">MST: 0401676571</span>
                                </div>
                                <div class="grid grid-cols-1 sm:grid-cols-2 gap-4 text-xs sm:text-sm">
                                    <div class="p-3.5 rounded-2xl bg-slate-50 border-l-4 border-acon-blue">
                                        <span class="font-display font-black text-acon-blue text-base">2015</span>
                                        <p class="font-semibold text-slate-800 mt-0.5">Thành lập doanh nghiệp (14/05/2015)</p>
                                        <p class="text-slate-500 text-xs mt-1">Khởi đầu hành trình thi công xây dựng & nội thất tại TP. Đà Nẵng.</p>
                                    </div>
                                    <div class="p-3.5 rounded-2xl bg-slate-50 border-l-4 border-acon-cyan">
                                        <span class="font-display font-black text-acon-cyan text-base">2019</span>
                                        <p class="font-semibold text-slate-800 mt-0.5">Mở rộng quy mô Tổng thầu</p>
                                        <p class="text-slate-500 text-xs mt-1">Khai trương văn phòng tại Hòa Xuân, đẩy mạnh thi công khách sạn, biệt thự & nhà xưởng.</p>
                                    </div>
                                    <div class="p-3.5 rounded-2xl bg-slate-50 border-l-4 border-amber-500">
                                        <span class="font-display font-black text-amber-600 text-base">2023</span>
                                        <p class="font-semibold text-slate-800 mt-0.5">Chứng chỉ năng lực HĐXD Hạng II</p>
                                        <p class="text-slate-500 text-xs mt-1">Được cấp mã chứng chỉ 00076275 đa lĩnh vực Thiết kế, QLDA, Giám sát & Thi công.</p>
                                    </div>
                                    <div class="p-3.5 rounded-2xl bg-slate-50 border-l-4 border-acon-red">
                                        <span class="font-display font-black text-acon-red text-base">2026</span>
                                        <p class="font-semibold text-slate-800 mt-0.5">Khẳng định vị thế Design & Build</p>
                                        <p class="text-slate-500 text-xs mt-1">Trụ sở 145-147 Trung Lương 14, quy tụ đội ngũ 25–99 kỹ sư & chuyên gia giàu kinh nghiệm.</p>
                                    </div>
                                </div>
                            </div>

                            <!-- Values Tab Panel -->
                            <div id="tab-panel-values" class="hidden space-y-4">
                                <div class="flex items-center justify-between border-b border-slate-100 pb-3">
                                    <h4 class="font-display font-extrabold text-acon-navy text-base uppercase tracking-wider">
                                        Sứ mệnh & Giá trị cốt lõi ACON
                                    </h4>
                                    <span class="text-xs font-bold text-acon-red bg-red-50 px-3 py-1 rounded-full">Build On Trust</span>
                                </div>
                                <div class="grid grid-cols-1 sm:grid-cols-3 gap-3 text-xs">
                                    <div class="p-4 rounded-2xl bg-blue-50/70">
                                        <i class="fa-solid fa-shield-halved text-acon-blue text-lg mb-2"></i>
                                        <h5 class="font-display font-bold text-acon-navy text-sm">UY TÍN HÀNG ĐẦU</h5>
                                        <p class="text-slate-600 mt-1">Cam kết đúng tiến độ, minh bạch vật tư và tối ưu ngân sách cho Chủ đầu tư.</p>
                                    </div>
                                    <div class="p-4 rounded-2xl bg-sky-50/70">
                                        <i class="fa-solid fa-compass-drafting text-acon-cyan text-lg mb-2"></i>
                                        <h5 class="font-display font-bold text-acon-navy text-sm">CHUYÊN NGHIỆP</h5>
                                        <p class="text-slate-600 mt-1">Ứng dụng mô hình BIM, Revit và quy trình kiểm soát chất lượng QA/QC – HSE nghiêm ngặt.</p>
                                    </div>
                                    <div class="p-4 rounded-2xl bg-amber-50/70">
                                        <i class="fa-solid fa-handshake-angle text-amber-600 text-lg mb-2"></i>
                                        <h5 class="font-display font-bold text-acon-navy text-sm">TỬ TẾ & BỀN VỮNG</h5>
                                        <p class="text-slate-600 mt-1">Đồng hành dài lâu cùng đối tác, bảo hành tận tâm và kiến tạo môi trường làm việc nhân văn.</p>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- ==========================================
         SECTION 03: LĨNH VỰC HOẠT ĐỘNG (NEWTECONS EXPANDING PILLARS EFFECT)
    =========================================== -->
    <section id="sec-03" class="relative py-24 lg:py-28 bg-acon-dark text-white overflow-hidden">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 mb-12">
            <div class="flex flex-col md:flex-row md:items-end justify-between gap-6 reveal-up">
                <div>
                    <div class="flex items-center gap-3 mb-3">
                        <span class="w-10 h-1 bg-acon-cyan rounded-full"></span>
                        <span class="font-display font-bold text-xs uppercase tracking-widest text-acon-cyan">03 • LĨNH VỰC HOẠT ĐỘNG</span>
                    </div>
                    <h2 class="font-display font-black text-3xl sm:text-4xl lg:text-5xl leading-tight">
                        GIẢI PHÁP XÂY DỰNG <span class="text-acon-cyan">TOÀN DIỆN</span>
                    </h2>
                </div>
                <p class="text-white/75 max-w-xl text-sm sm:text-base">
                    Mô hình Thiết kế và Thi công (Design & Build) kết hợp năng lực Quản lý dự án & Giám sát đạt chuẩn Bộ Xây dựng (Mã chứng chỉ <strong>00076275</strong>), giúp dự án rút ngắn tiến độ và tối ưu chi phí.
                </p>
            </div>
        </div>

        <!-- Expanding Horizontal Accordion Pillars (Hiệu ứng di chuột mở rộng cột đặc trưng của Newtecons) -->
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="service-pillars-container flex flex-col lg:flex-row gap-4 min-h-[480px] reveal-up">
                
                <!-- Pillar 1: Tổng thầu Thiết kế & Thi công (Design & Build) -->
                <div class="service-pillar relative rounded-3xl overflow-hidden flex-1 min-h-[300px] lg:min-h-[480px] group cursor-pointer border border-white/15">
                    <img src="https://images.unsplash.com/photo-1541888946425-d09bb18086f6?auto=format&fit=crop&w=1000&q=80" 
                         onerror="this.src='https://placehold.co/800x600/002B5B/FFFFFF?text=DESIGN+AND+BUILD'"
                         alt="Tổng thầu Thiết kế và Thi công Xây dựng" 
                         class="absolute inset-0 w-full h-full object-cover group-hover:scale-110 transition-transform duration-700" />
                    <div class="absolute inset-0 bg-gradient-to-t from-acon-dark via-acon-navy/75 to-acon-dark/30 group-hover:via-acon-blue/70 transition-all"></div>
                    <div class="relative z-10 p-7 h-full flex flex-col justify-between">
                        <div class="flex items-center justify-between">
                            <span class="font-display font-black text-4xl text-white/30 group-hover:text-acon-cyan transition-colors">01</span>
                            <span class="px-3 py-1 rounded-full bg-acon-cyan/20 border border-acon-cyan/40 text-acon-cyan text-xs font-bold">Mũi nhọn</span>
                        </div>
                        <div>
                            <div class="w-12 h-12 rounded-2xl bg-acon-cyan text-white flex items-center justify-center text-xl mb-4 shadow-lg">
                                <i class="fa-solid fa-building-Flag"></i>
                            </div>
                            <h3 class="font-display font-extrabold text-xl sm:text-2xl text-white mb-3">
                                TỔNG THẦU THIẾT KẾ & THI CÔNG (DESIGN & BUILD)
                            </h3>
                            <p class="text-sm text-white/85 leading-relaxed mb-4">
                                Kết hợp đồng bộ trách nhiệm Thiết kế kiến trúc - kết cấu và Thi công xây dựng công trình Dân dụng (Hạng II): Khách sạn, Tòa nhà văn phòng, Khu nghỉ dưỡng, Biệt thự cao cấp.
                            </p>
                            <span onclick="filterProjects('all'); document.getElementById('sec-05').scrollIntoView({behavior:'smooth'});" class="inline-flex items-center gap-2 text-xs font-display font-bold uppercase tracking-wider text-acon-cyan group-hover:translate-x-2 transition-transform">
                                Xem dự án thực tế <i class="fa-solid fa-arrow-right"></i>
                            </span>
                        </div>
                    </div>
                </div>

                <!-- Pillar 2: Thi công Công trình Công nghiệp & Nhà xưởng -->
                <div class="service-pillar relative rounded-3xl overflow-hidden flex-1 min-h-[300px] lg:min-h-[480px] group cursor-pointer border border-white/15">
                    <img src="https://images.unsplash.com/photo-1581092160607-ee22621dd758?auto=format&fit=crop&w=1000&q=80" 
                         onerror="this.src='https://placehold.co/800x600/0054A6/FFFFFF?text=CONG+NGHIEP+NHA+XUONG'"
                         alt="Thi công Nhà công nghiệp và Kết cấu thép" 
                         class="absolute inset-0 w-full h-full object-cover group-hover:scale-110 transition-transform duration-700" />
                    <div class="absolute inset-0 bg-gradient-to-t from-acon-dark via-acon-navy/75 to-acon-dark/30 group-hover:via-acon-blue/70 transition-all"></div>
                    <div class="relative z-10 p-7 h-full flex flex-col justify-between">
                        <div class="flex items-center justify-between">
                            <span class="font-display font-black text-4xl text-white/30 group-hover:text-acon-cyan transition-colors">02</span>
                            <span class="px-3 py-1 rounded-full bg-white/10 text-white/90 text-xs font-bold">Công nghiệp</span>
                        </div>
                        <div>
                            <div class="w-12 h-12 rounded-2xl bg-acon-blue text-white flex items-center justify-center text-xl mb-4 shadow-lg">
                                <i class="fa-solid fa-industry"></i>
                            </div>
                            <h3 class="font-display font-extrabold text-xl sm:text-2xl text-white mb-3">
                                THI CÔNG NHÀ CÔNG NGHIỆP & HẠ TẦNG KỸ THUẬT
                            </h3>
                            <p class="text-sm text-white/85 leading-relaxed mb-4">
                                Thiết kế, thẩm tra và thi công trọn gói Nhà máy sản xuất, Kho vận Logistics, Kết cấu thép tiền chế và hạ tầng KCN tại Đà Nẵng, Quảng Nam và Miền Trung.
                            </p>
                            <span onclick="filterProjects('industrial'); document.getElementById('sec-05').scrollIntoView({behavior:'smooth'});" class="inline-flex items-center gap-2 text-xs font-display font-bold uppercase tracking-wider text-acon-cyan group-hover:translate-x-2 transition-transform">
                                Xem dự án công nghiệp <i class="fa-solid fa-arrow-right"></i>
                            </span>
                        </div>
                    </div>
                </div>

                <!-- Pillar 3: Thi công Cơ điện (M&E) & Lắp đặt thiết bị -->
                <div class="service-pillar relative rounded-3xl overflow-hidden flex-1 min-h-[300px] lg:min-h-[480px] group cursor-pointer border border-white/15">
                    <img src="https://images.unsplash.com/photo-1621905251189-08b45d6a269e?auto=format&fit=crop&w=1000&q=80" 
                         onerror="this.src='https://placehold.co/800x600/0A192F/FFFFFF?text=CO+DIEN+MEP+NOI+THAT'"
                         alt="Thi công lắp đặt thiết bị công trình và Nội thất" 
                         class="absolute inset-0 w-full h-full object-cover group-hover:scale-110 transition-transform duration-700" />
                    <div class="absolute inset-0 bg-gradient-to-t from-acon-dark via-acon-navy/75 to-acon-dark/30 group-hover:via-acon-blue/70 transition-all"></div>
                    <div class="relative z-10 p-7 h-full flex flex-col justify-between">
                        <div class="flex items-center justify-between">
                            <span class="font-display font-black text-4xl text-white/30 group-hover:text-acon-cyan transition-colors">03</span>
                            <span class="px-3 py-1 rounded-full bg-white/10 text-white/90 text-xs font-bold">M&E • Fit-out</span>
                        </div>
                        <div>
                            <div class="w-12 h-12 rounded-2xl bg-amber-500 text-white flex items-center justify-center text-xl mb-4 shadow-lg">
                                <i class="fa-solid fa-bolt-lightning"></i>
                            </div>
                            <h3 class="font-display font-extrabold text-xl sm:text-2xl text-white mb-3">
                                THI CÔNG LẮP ĐẶT THIẾT BỊ (M&E) & NỘI THẤT
                            </h3>
                            <p class="text-sm text-white/85 leading-relaxed mb-4">
                                Thi công hệ thống Cơ điện (MEP), điều hòa thông gió, PCCC, cấp thoát nước và hoàn thiện nội thất cao cấp cho văn phòng, khách sạn, showroom và biệt thự.
                            </p>
                            <span onclick="filterProjects('commercial'); document.getElementById('sec-05').scrollIntoView({behavior:'smooth'});" class="inline-flex items-center gap-2 text-xs font-display font-bold uppercase tracking-wider text-acon-cyan group-hover:translate-x-2 transition-transform">
                                Xem công trình hoàn thiện <i class="fa-solid fa-arrow-right"></i>
                            </span>
                        </div>
                    </div>
                </div>

                <!-- Pillar 4: Tư vấn Quản lý dự án & Giám sát xây dựng -->
                <div class="service-pillar relative rounded-3xl overflow-hidden flex-1 min-h-[300px] lg:min-h-[480px] group cursor-pointer border border-white/15">
                    <img src="https://images.unsplash.com/photo-1454165804606-c3d57bc86b40?auto=format&fit=crop&w=1000&q=80" 
                         onerror="this.src='https://placehold.co/800x600/002B5B/FFFFFF?text=TU+VAN+QUAN+LY+DU+AN'"
                         alt="Tư vấn Quản lý dự án và Tư vấn giám sát" 
                         class="absolute inset-0 w-full h-full object-cover group-hover:scale-110 transition-transform duration-700" />
                    <div class="absolute inset-0 bg-gradient-to-t from-acon-dark via-acon-navy/75 to-acon-dark/30 group-hover:via-acon-blue/70 transition-all"></div>
                    <div class="relative z-10 p-7 h-full flex flex-col justify-between">
                        <div class="flex items-center justify-between">
                            <span class="font-display font-black text-4xl text-white/30 group-hover:text-acon-cyan transition-colors">04</span>
                            <span class="px-3 py-1 rounded-full bg-white/10 text-white/90 text-xs font-bold">Tư vấn & QS</span>
                        </div>
                        <div>
                            <div class="w-12 h-12 rounded-2xl bg-acon-red text-white flex items-center justify-center text-xl mb-4 shadow-lg">
                                <i class="fa-solid fa-clipboard-check"></i>
                            </div>
                            <h3 class="font-display font-extrabold text-xl sm:text-2xl text-white mb-3">
                                TƯ VẤN QUẢN LÝ DỰ ÁN & GIÁM SÁT THI CÔNG
                            </h3>
                            <p class="text-sm text-white/85 leading-relaxed mb-4">
                                Tư vấn quản lý dự án đầu tư xây dựng, thẩm tra thiết kế - dự toán (QS) và tư vấn giám sát công trình Dân dụng & Công nghiệp theo chứng chỉ năng lực của Bộ Xây dựng.
                            </p>
                            <span onclick="openProfileModal()" class="inline-flex items-center gap-2 text-xs font-display font-bold uppercase tracking-wider text-acon-cyan group-hover:translate-x-2 transition-transform">
                                Xem bảng chứng chỉ năng lực <i class="fa-solid fa-arrow-right"></i>
                            </span>
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- ==========================================
         SECTION 04: CON SỐ ẤN TƯỢNG & CHỨNG CHỈ NĂNG LỰC HĐXD
         (Hiệu ứng đếm số tự động khi cuộn trang giống Newtecons)
    =========================================== -->
    <section id="sec-04" class="relative py-20 lg:py-28 bg-gradient-to-br from-acon-navy via-acon-blue to-acon-dark text-white overflow-hidden">
        <div class="absolute inset-0 bg-blueprint-dark pointer-events-none"></div>
        
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">
            <div class="text-center max-w-3xl mx-auto mb-16 reveal-up">
                <span class="inline-block px-4 py-1.5 rounded-full bg-white/10 text-acon-cyan font-display font-bold text-xs uppercase tracking-widest mb-4">
                    04 • DẤU ẤN & NĂNG LỰC PHÁP LÝ
                </span>
                <h2 class="font-display font-black text-3xl sm:text-4xl lg:text-5xl leading-tight">
                    CÙNG NHAU CHÚNG TÔI KIẾN TẠO <br class="hidden sm:inline" />
                    <span class="text-acon-cyan">NHỮNG CÔNG TRÌNH BIỂU TƯỢNG</span>
                </h2>
            </div>

            <!-- 4 Animated Counters (Newtecons Style) -->
            <div id="counters-grid" class="grid grid-cols-2 lg:grid-cols-4 gap-6 mb-16 reveal-up">
                <div class="bg-white/10 backdrop-blur-md border border-white/15 rounded-3xl p-7 text-center hover:bg-white/15 transition-all">
                    <div class="font-display font-black text-4xl sm:text-5xl lg:text-6xl text-acon-cyan mb-2">
                        +<span class="counter-value" data-target="11">0</span>
                    </div>
                    <div class="font-display font-bold text-sm uppercase tracking-wider text-white">NĂM HOẠT ĐỘNG</div>
                    <p class="text-xs text-white/70 mt-1">Thành lập từ 14/05/2015</p>
                </div>

                <div class="bg-white/10 backdrop-blur-md border border-white/15 rounded-3xl p-7 text-center hover:bg-white/15 transition-all">
                    <div class="font-display font-black text-4xl sm:text-5xl lg:text-6xl text-white mb-2">
                        +<span class="counter-value" data-target="85">0</span>
                    </div>
                    <div class="font-display font-bold text-sm uppercase tracking-wider text-white">NHÂN SỰ KỸ SƯ & KTS</div>
                    <p class="text-xs text-white/70 mt-1">Chỉ huy trưởng, Kỹ sư QS, MEP</p>
                </div>

                <div class="bg-white/10 backdrop-blur-md border border-white/15 rounded-3xl p-7 text-center hover:bg-white/15 transition-all">
                    <div class="font-display font-black text-4xl sm:text-5xl lg:text-6xl text-amber-400 mb-2">
                        +<span class="counter-value" data-target="120">0</span>
                    </div>
                    <div class="font-display font-bold text-sm uppercase tracking-wider text-white">DỰ ÁN & GÓI THẦU</div>
                    <p class="text-xs text-white/70 mt-1">Tại Đà Nẵng & Miền Trung</p>
                </div>

                <div class="bg-white/10 backdrop-blur-md border border-white/15 rounded-3xl p-7 text-center hover:bg-white/15 transition-all">
                    <div class="font-display font-black text-3xl sm:text-4xl lg:text-5xl text-acon-red bg-white px-4 py-1 rounded-2xl inline-block mb-2">
                        HẠNG II
                    </div>
                    <div class="font-display font-bold text-sm uppercase tracking-wider text-white">CHỨNG CHỈ NĂNG LỰC</div>
                    <p class="text-xs text-white/70 mt-1">Mã số HĐXD: 00076275</p>
                </div>
            </div>

            <!-- Official Construction Capacity Certificate Summary Box -->
            <div class="bg-white text-slate-800 rounded-3xl p-6 sm:p-10 shadow-2xl reveal-up">
                <div class="flex flex-col lg:flex-row lg:items-center justify-between gap-6 pb-6 border-b border-slate-200">
                    <div>
                        <div class="flex items-center gap-2 text-acon-blue font-display font-bold text-xs uppercase tracking-widest mb-1">
                            <i class="fa-solid fa-certificate text-amber-500 text-base"></i>
                            <span>DỮ LIỆU NĂNG LỰC HOẠT ĐỘNG XÂY DỰNG ĐƯỢC CHỨNG NHẬN</span>
                        </div>
                        <h3 class="font-display font-black text-xl sm:text-2xl text-acon-navy">
                            CÔNG TY CỔ PHẦN ĐẦU TƯ XÂY DỰNG ACON — MÃ SỐ: <span class="text-acon-red">00076275</span>
                        </h3>
                        <p class="text-xs sm:text-sm text-slate-500 mt-1">
                            Người đại diện theo pháp luật: <strong>Ông Huỳnh Bá Quý</strong> (Giám đốc) • Mã số thuế: <strong>0401676571</strong> • Hiệu lực đến: <strong>27/09/2033</strong>
                        </p>
                    </div>
                    <button onclick="openProfileModal()" class="shrink-0 bg-acon-navy hover:bg-acon-blue text-white font-display font-bold text-xs uppercase tracking-wider px-6 py-3.5 rounded-xl transition-all shadow-md">
                        <i class="fa-solid fa-table-list mr-2"></i>Xem chi tiết 10 lĩnh vực cấp phép
                    </button>
                </div>

                <div class="grid grid-cols-1 md:grid-cols-3 lg:grid-cols-5 gap-4 mt-6 text-xs">
                    <div class="p-4 rounded-2xl bg-slate-50 border border-slate-200/80">
                        <span class="px-2 py-0.5 rounded bg-acon-red text-white font-bold text-[10px]">HẠNG II</span>
                        <h4 class="font-display font-bold text-acon-navy text-sm mt-2">Thi công Xây dựng Dân dụng</h4>
                        <p class="text-slate-500 mt-1">Số CC: HCM-00076275 (Hiệu lực 27/09/2033)</p>
                    </div>
                    <div class="p-4 rounded-2xl bg-slate-50 border border-slate-200/80">
                        <span class="px-2 py-0.5 rounded bg-acon-blue text-white font-bold text-[10px]">HẠNG III</span>
                        <h4 class="font-display font-bold text-acon-navy text-sm mt-2">Thi công Nhà Công nghiệp</h4>
                        <p class="text-slate-500 mt-1">Nhà xưởng, kho bãi, kết cấu công nghiệp</p>
                    </div>
                    <div class="p-4 rounded-2xl bg-slate-50 border border-slate-200/80">
                        <span class="px-2 py-0.5 rounded bg-acon-blue text-white font-bold text-[10px]">HẠNG III</span>
                        <h4 class="font-display font-bold text-acon-navy text-sm mt-2">Thiết kế & Thẩm tra Thiết kế</h4>
                        <p class="text-slate-500 mt-1">Công trình Dân dụng & Nhà công nghiệp</p>
                    </div>
                    <div class="p-4 rounded-2xl bg-slate-50 border border-slate-200/80">
                        <span class="px-2 py-0.5 rounded bg-acon-blue text-white font-bold text-[10px]">HẠNG III</span>
                        <h4 class="font-display font-bold text-acon-navy text-sm mt-2">Tư vấn Quản lý Dự án</h4>
                        <p class="text-slate-500 mt-1">Quản lý dự án Dân dụng & Công nghiệp</p>
                    </div>
                    <div class="p-4 rounded-2xl bg-slate-50 border border-slate-200/80">
                        <span class="px-2 py-0.5 rounded bg-acon-blue text-white font-bold text-[10px]">HẠNG III</span>
                        <h4 class="font-display font-bold text-acon-navy text-sm mt-2">Tư vấn Giám sát & Lắp đặt</h4>
                        <p class="text-slate-500 mt-1">Giám sát thi công & Lắp đặt thiết bị công trình</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- ==========================================
         SECTION 05: DỰ ÁN TIÊU BIỂU (LẤY TỪ HÌNH ẢNH & DỰ ÁN FANPAGE ACON)
         (Hiệu ứng lọc danh mục + Card Hover Zoom giống Newtecons)
    =========================================== -->
    <section id="sec-05" class="relative py-24 lg:py-32 bg-acon-light bg-blueprint overflow-hidden">
        <!-- Giant Stroke Watermark -->
        <div class="absolute top-10 right-8 pointer-events-none select-none hidden lg:block">
            <span class="font-display font-black text-[110px] stroke-text leading-none">PROJECTS</span>
        </div>

        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">
            <!-- Section Header & Category Filter -->
            <div class="flex flex-col lg:flex-row lg:items-end justify-between gap-6 mb-12 reveal-up">
                <div>
                    <div class="flex items-center gap-3 mb-3">
                        <span class="w-10 h-1 bg-acon-blue rounded-full"></span>
                        <span class="font-display font-bold text-xs uppercase tracking-widest text-acon-blue">05 • CÔNG TRÌNH KIẾN TẠO</span>
                    </div>
                    <h2 class="font-display font-black text-3xl sm:text-4xl lg:text-5xl text-acon-navy leading-tight">
                        DỰ ÁN <span class="text-acon-cyan">TIÊU BIỂU</span>
                    </h2>
                </div>

                <!-- Filter Buttons -->
                <div class="flex flex-wrap gap-2">
                    <button onclick="filterProjects('all')" data-filter="all" class="proj-filter-btn active px-4 py-2.5 rounded-xl font-display font-bold text-xs uppercase tracking-wider bg-acon-navy text-white shadow-md transition-all">
                        Tất cả dự án
                    </button>
                    <button onclick="filterProjects('commercial')" data-filter="commercial" class="proj-filter-btn px-4 py-2.5 rounded-xl font-display font-bold text-xs uppercase tracking-wider bg-white text-slate-700 hover:bg-acon-blue hover:text-white transition-all border border-slate-200">
                        Khách sạn & Văn phòng
                    </button>
                    <button onclick="filterProjects('residential')" data-filter="residential" class="proj-filter-btn px-4 py-2.5 rounded-xl font-display font-bold text-xs uppercase tracking-wider bg-white text-slate-700 hover:bg-acon-blue hover:text-white transition-all border border-slate-200">
                        Biệt thự & Dân dụng
                    </button>
                    <button onclick="filterProjects('industrial')" data-filter="industrial" class="proj-filter-btn px-4 py-2.5 rounded-xl font-display font-bold text-xs uppercase tracking-wider bg-white text-slate-700 hover:bg-acon-blue hover:text-white transition-all border border-slate-200">
                        Nhà xưởng & Công nghiệp
                    </button>
                </div>
            </div>

            <!-- Projects Grid (Rendered dynamically via JS so user can also add/edit Fanpage projects) -->
            <div id="projects-grid" class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-7 reveal-up">
                <!-- Populated by JavaScript -->
            </div>

            <!-- Bottom Banner to Fanpage Albums -->
            <div class="mt-12 bg-white rounded-3xl p-6 sm:p-8 shadow-lg border border-slate-200/80 flex flex-col sm:flex-row items-center justify-between gap-6 reveal-up">
                <div class="flex items-center gap-4">
                    <div class="w-14 h-14 rounded-2xl bg-[#1877F2]/10 text-[#1877F2] flex items-center justify-center text-2xl shrink-0">
                        <i class="fa-brands fa-facebook"></i>
                    </div>
                    <div>
                        <h4 class="font-display font-bold text-lg text-acon-navy">Cập nhật hình ảnh nhật ký công trường hàng ngày trên Fanpage</h4>
                        <p class="text-xs sm:text-sm text-slate-600">Xem toàn bộ album ảnh khởi công, đổ bê tông sàn, cất nóc và bàn giao dự án tại Fanpage chính thức của ACON Construction.</p>
                    </div>
                </div>
                <div class="flex items-center gap-3 shrink-0">
                    <button onclick="openLogoModal()" class="px-4 py-3 rounded-xl bg-slate-100 hover:bg-slate-200 text-acon-navy font-display font-bold text-xs uppercase tracking-wider transition-all">
                        <i class="fa-solid fa-plus mr-1.5"></i>Thêm ảnh dự án
                    </button>
                    <a href="https://www.facebook.com/aconvn.construction" target="_blank" rel="noopener noreferrer" class="px-6 py-3 rounded-xl bg-[#1877F2] hover:bg-blue-700 text-white font-display font-bold text-xs uppercase tracking-wider shadow-md transition-all">
                        Xem trên Fanpage <i class="fa-solid fa-arrow-up-right-from-square ml-1.5"></i>
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- ==========================================
         SECTION 06: TIN TỨC FANPAGE & TUYỂN DỤNG NHÂN SỰ ACON
         (Bố cục Tin tức Newtecons: 1 tin tiêu điểm lớn + cột tin/tuyển dụng bên phải)
    =========================================== -->
    <section id="sec-06" class="relative py-24 lg:py-32 bg-white overflow-hidden">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex flex-col md:flex-row md:items-end justify-between gap-6 mb-12 reveal-up">
                <div>
                    <div class="flex items-center gap-3 mb-3">
                        <span class="w-10 h-1 bg-acon-red rounded-full"></span>
                        <span class="font-display font-bold text-xs uppercase tracking-widest text-acon-red">06 • NHỊP ĐẬP CÔNG TRƯỜNG & NHÂN SỰ</span>
                    </div>
                    <h2 class="font-display font-black text-3xl sm:text-4xl lg:text-5xl text-acon-navy leading-tight">
                        TIN TỨC <span class="text-acon-blue">ACON</span> & TUYỂN DỤNG
                    </h2>
                </div>
                <a href="https://www.facebook.com/aconvn.construction" target="_blank" rel="noopener noreferrer" class="inline-flex items-center gap-2 text-sm font-display font-bold text-acon-blue hover:text-acon-cyan uppercase tracking-wider">
                    <span>Xem tất cả bài đăng Fanpage</span>
                    <i class="fa-solid fa-arrow-right"></i>
                </a>
            </div>

            <!-- Asymmetric Newtecons News Layout -->
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-8 reveal-up">
                <!-- Left Featured News (7 Cols) -->
                <div class="lg:col-span-7 group cursor-pointer" onclick="openNewsModal(0)">
                    <div class="rounded-3xl overflow-hidden shadow-xl border border-slate-200 bg-white h-full flex flex-col">
                        <div class="relative h-72 sm:h-96 overflow-hidden">
                            <img src="https://images.unsplash.com/photo-1541888946425-d09bb18086f6?auto=format&fit=crop&w=1200&q=85" 
                                 onerror="this.src='https://placehold.co/900x600/002B5B/FFFFFF?text=ACON+CAT+NOC+DU+AN'"
                                 alt="ACON đẩy mạnh tiến độ các công trình trọng điểm tại Đà Nẵng" 
                                 class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-700" />
                            <div class="absolute top-4 left-4 bg-acon-navy text-white rounded-2xl px-4 py-2 text-center shadow-lg">
                                <span class="block font-display font-black text-2xl leading-none text-acon-cyan">15</span>
                                <span class="text-[11px] font-semibold uppercase">Tháng 10, 2026</span>
                            </div>
                            <span class="absolute bottom-4 left-4 px-3 py-1 rounded-full bg-acon-red text-white text-xs font-bold uppercase">
                                Tin công trường Fanpage
                            </span>
                        </div>
                        <div class="p-6 sm:p-8 flex-1 flex flex-col justify-between">
                            <div>
                                <h3 class="font-display font-extrabold text-xl sm:text-2xl text-acon-navy group-hover:text-acon-blue transition-colors mb-3">
                                    ACON CONSTRUCTION ĐẨY MẠNH TIẾN ĐỘ THI CÔNG & NGHIỆM THU CÁC DỰ ÁN DÂN DỤNG – THƯƠNG MẠI TẠI ĐÀ NẴNG
                                </h3>
                                <p class="text-slate-600 text-sm sm:text-base leading-relaxed">
                                    Với tinh thần kiểm soát chặt chẽ an toàn lao động (HSE) và chất lượng kỹ - mỹ thuật trên từng hạng mục kết cấu & hoàn thiện, Ban chỉ huy các công trường ACON Construction liên tục hoàn thành vượt mốc tiến độ cam kết với Chủ đầu tư...
                                </p>
                            </div>
                            <div class="mt-6 pt-4 border-t border-slate-100 flex items-center justify-between text-xs font-bold text-acon-blue">
                                <span><i class="fa-brands fa-facebook mr-1.5"></i>Nguồn: Fanpage ACON Construction</span>
                                <span class="group-hover:translate-x-2 transition-transform">Đọc chi tiết <i class="fa-solid fa-arrow-right ml-1"></i></span>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Right Stacked News & Recruitment Posts (5 Cols) -->
                <div class="lg:col-span-5 flex flex-col justify-between gap-5">
                    
                    <!-- News Item 1: Recruitment (Real Fanpage Info) -->
                    <div onclick="openNewsModal(1)" class="group cursor-pointer bg-slate-50 hover:bg-acon-navy hover:text-white rounded-3xl p-5 sm:p-6 transition-all border border-slate-200/80 shadow-sm">
                        <div class="flex items-start gap-4">
                            <div class="bg-acon-red text-white rounded-2xl px-3.5 py-2.5 text-center shrink-0">
                                <span class="block font-display font-black text-xl leading-none">HOT</span>
                                <span class="text-[10px] uppercase font-bold">Tuyển dụng</span>
                            </div>
                            <div>
                                <span class="text-xs font-bold text-acon-cyan uppercase tracking-wider">Cơ hội nghề nghiệp tại Đà Nẵng</span>
                                <h4 class="font-display font-bold text-base text-acon-navy group-hover:text-white mt-1 leading-snug">
                                    ACON TUYỂN DỤNG: KỸ SƯ QS, CHỈ HUY TRƯỞNG CÔNG TRÌNH, KỸ SƯ HIỆN TRƯỜNG & KẾ TOÁN XÂY DỰNG
                                </h4>
                                <p class="text-xs text-slate-500 group-hover:text-white/80 mt-2">
                                    Làm việc tại: 145-147 Trung Lương 14, P. Hòa Xuân, Đà Nẵng • Nhận hồ sơ qua: acon.dng@gmail.com hoặc SĐT: 0916.104.099
                                </p>
                            </div>
                        </div>
                    </div>

                    <!-- News Item 2 -->
                    <div onclick="openNewsModal(2)" class="group cursor-pointer bg-slate-50 hover:bg-acon-navy hover:text-white rounded-3xl p-5 sm:p-6 transition-all border border-slate-200/80 shadow-sm">
                        <div class="flex items-start gap-4">
                            <div class="bg-acon-blue text-white rounded-2xl px-3.5 py-2.5 text-center shrink-0">
                                <span class="block font-display font-black text-xl leading-none">28</span>
                                <span class="text-[10px] uppercase font-bold">Th08, 2026</span>
                            </div>
                            <div>
                                <span class="text-xs font-bold text-acon-cyan uppercase tracking-wider">Hoạt động doanh nghiệp</span>
                                <h4 class="font-display font-bold text-base text-acon-navy group-hover:text-white mt-1 leading-snug">
                                    CHUẨN HÓA QUY TRÌNH QUẢN LÝ CHẤT LƯỢNG & AN TOÀN VỆ SINH LAO ĐỘNG TRÊN TOÀN HỆ THỐNG CÔNG TRƯỜNG ACON
                                </h4>
                                <p class="text-xs text-slate-500 group-hover:text-white/80 mt-2">
                                    Đào tạo nội bộ định kỳ cho đội ngũ Kỹ sư giám sát & Chỉ huy trưởng tại trụ sở Hòa Xuân, Đà Nẵng.
                                </p>
                            </div>
                        </div>
                    </div>

                    <!-- News Item 3 -->
                    <div onclick="openNewsModal(3)" class="group cursor-pointer bg-slate-50 hover:bg-acon-navy hover:text-white rounded-3xl p-5 sm:p-6 transition-all border border-slate-200/80 shadow-sm">
                        <div class="flex items-start gap-4">
                            <div class="bg-acon-navy group-hover:bg-acon-cyan text-white rounded-2xl px-3.5 py-2.5 text-center shrink-0 transition-colors">
                                <span class="block font-display font-black text-xl leading-none">14</span>
                                <span class="text-[10px] uppercase font-bold">Th05, 2026</span>
                            </div>
                            <div>
                                <span class="text-xs font-bold text-acon-cyan uppercase tracking-wider">Kỷ niệm thành lập</span>
                                <h4 class="font-display font-bold text-base text-acon-navy group-hover:text-white mt-1 leading-snug">
                                    KỶ NIỆM 11 NĂM HÌNH THÀNH VÀ PHÁT TRIỂN CÔNG TY CỔ PHẦN ĐẦU TƯ XÂY DỰNG ACON (14/05/2015 – 14/05/2026)
                                </h4>
                                <p class="text-xs text-slate-500 group-hover:text-white/80 mt-2">
                                    Hơn một thập kỷ gắn bó và kiến tạo những công trình chất lượng, bền vững cùng khách hàng và đối tác.
                                </p>
                            </div>
                        </div>
                    </div>

                </div>
            </div>
        </div>
    </section>

    <!-- ==========================================
         SECTION 07: LIÊN HỆ, BÁO GIÁ ĐẤU THẦU & BẢN ĐỒ TRỤ SỞ
         (145-147 Trung Lương 14, Hoà Xuân, Đà Nẵng - 0916.104.099)
    =========================================== -->
    <section id="sec-07" class="relative py-24 bg-acon-light border-t border-slate-200">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-10 items-start">
                
                <!-- Left Column: Official Contact Information & Map -->
                <div class="lg:col-span-6 space-y-6 reveal-left">
                    <div>
                        <div class="flex items-center gap-3 mb-3">
                            <span class="w-10 h-1 bg-acon-blue rounded-full"></span>
                            <span class="font-display font-bold text-xs uppercase tracking-widest text-acon-blue">07 • THÔNG TIN LIÊN HỆ</span>
                        </div>
                        <h2 class="font-display font-black text-3xl sm:text-4xl text-acon-navy">
                            KẾT NỐI CÙNG <span class="text-acon-cyan">ACON</span>
                        </h2>
                        <p class="text-slate-600 text-sm sm:text-base mt-2">
                            Quý Chủ đầu tư, Đối tác và Ứng viên vui lòng liên hệ trực tiếp tại văn phòng trụ sở Đà Nẵng hoặc gửi yêu cầu tư vấn thiết kế – báo giá thi công dưới đây.
                        </p>
                    </div>

                    <!-- Contact Cards -->
                    <div class="bg-white rounded-3xl p-6 sm:p-8 shadow-lg border border-slate-200/80 space-y-5">
                        <div class="flex items-start gap-4">
                            <div class="w-12 h-12 rounded-2xl bg-acon-navy text-acon-cyan flex items-center justify-center text-xl shrink-0">
                                <i class="fa-solid fa-building-columns"></i>
                            </div>
                            <div>
                                <span class="text-xs font-bold uppercase text-acon-blue tracking-wider">Trụ sở văn phòng Đà Nẵng</span>
                                <h4 class="font-display font-bold text-acon-navy text-base mt-0.5">
                                    145-147 Trung Lương 14, Phường Hòa Xuân, Quận Cẩm Lệ, TP. Đà Nẵng
                                </h4>
                                <p class="text-xs text-slate-500 mt-1">Mã số thuế: 0401676571 • Mã chứng chỉ HĐXD: 00076275</p>
                            </div>
                        </div>

                        <div class="grid grid-cols-1 sm:grid-cols-2 gap-4 pt-4 border-t border-slate-100">
                            <div class="flex items-center gap-3.5">
                                <div class="w-11 h-11 rounded-2xl bg-red-50 text-acon-red flex items-center justify-center text-lg shrink-0">
                                    <i class="fa-solid fa-phone-volume"></i>
                                </div>
                                <div>
                                    <span class="text-[11px] font-semibold text-slate-400 uppercase block">Hotline trực tiếp</span>
                                    <a href="tel:0916104099" class="font-display font-extrabold text-acon-navy hover:text-acon-red text-base">0916.104.099</a>
                                    <span class="block text-[11px] text-slate-500">ĐT VP: 02363.789.769</span>
                                </div>
                            </div>

                            <div class="flex items-center gap-3.5">
                                <div class="w-11 h-11 rounded-2xl bg-blue-50 text-acon-blue flex items-center justify-center text-lg shrink-0">
                                    <i class="fa-solid fa-envelope-open-text"></i>
                                </div>
                                <div>
                                    <span class="text-[11px] font-semibold text-slate-400 uppercase block">Email & Website</span>
                                    <a href="mailto:acon.dng@gmail.com" class="font-bold text-acon-navy hover:text-acon-blue text-sm block">acon.dng@gmail.com</a>
                                    <span class="block text-xs text-acon-cyan font-semibold">www.acondn.vn</span>
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- Embedded Google Maps for 145-147 Trung Lương 14, Hòa Xuân, Đà Nẵng -->
                    <div class="rounded-3xl overflow-hidden shadow-lg border-4 border-white h-64 sm:h-72 relative">
                        <iframe 
                            title="Bản đồ trụ sở Công ty Cổ phần Đầu tư Xây dựng ACON - 145-147 Trung Lương 14, Hòa Xuân, Đà Nẵng"
                            src="https://www.google.com/maps?q=145+Trung+L%C6%B0%C6%A1ng+14,+H%C3%B2a+Xu%C3%A2n,+C%E1%BA%A9m+L%E1%BB%87,+%C4%90%C3%A0+N%E1%BA%B5ng&output=embed"
                            class="w-full h-full border-0"
                            loading="lazy"
                            referrerpolicy="no-referrer-when-downgrade">
                        </iframe>
                    </div>
                </div>

                <!-- Right Column: Consultation / Tender / Application Form -->
                <div class="lg:col-span-6 reveal-right">
                    <div class="bg-white rounded-3xl p-8 sm:p-10 shadow-xl border border-slate-200/80">
                        <span class="inline-block px-3 py-1 rounded-full bg-acon-blue/10 text-acon-blue text-xs font-bold uppercase tracking-wider mb-3">
                            Đăng ký tư vấn & Hợp tác
                        </span>
                        <h3 class="font-display font-extrabold text-2xl text-acon-navy mb-2">
                            GỬI YÊU CẦU BÁO GIÁ / HỒ SƠ ĐẤU THẦU
                        </h3>
                        <p class="text-xs sm:text-sm text-slate-500 mb-6">
                            Phòng Đấu thầu & Kỹ thuật ACON sẽ phản hồi Quý khách trong vòng 24 giờ làm việc.
                        </p>

                        <form id="contact-form" onsubmit="handleContactSubmit(event)" class="space-y-4">
                            <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
                                <div>
                                    <label class="block text-xs font-bold uppercase text-slate-700 mb-1.5">Họ và tên / Tên đơn vị *</label>
                                    <input type="text" id="cf-name" required placeholder="Nhập họ tên hoặc Chủ đầu tư..." class="w-full px-4 py-3 rounded-xl bg-slate-50 border border-slate-200 focus:border-acon-blue focus:bg-white focus:outline-none text-sm" />
                                </div>
                                <div>
                                    <label class="block text-xs font-bold uppercase text-slate-700 mb-1.5">Số điện thoại liên hệ *</label>
                                    <input type="tel" id="cf-phone" required placeholder="Ví dụ: 0916.104.099" class="w-full px-4 py-3 rounded-xl bg-slate-50 border border-slate-200 focus:border-acon-blue focus:bg-white focus:outline-none text-sm" />
                                </div>
                            </div>

                            <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
                                <div>
                                    <label class="block text-xs font-bold uppercase text-slate-700 mb-1.5">Email</label>
                                    <input type="email" id="cf-email" placeholder="example@domain.com" class="w-full px-4 py-3 rounded-xl bg-slate-50 border border-slate-200 focus:border-acon-blue focus:bg-white focus:outline-none text-sm" />
                                </div>
                                <div>
                                    <label class="block text-xs font-bold uppercase text-slate-700 mb-1.5">Nhu cầu hợp tác *</label>
                                    <select id="cf-service" class="w-full px-4 py-3 rounded-xl bg-slate-50 border border-slate-200 focus:border-acon-blue focus:bg-white focus:outline-none text-sm">
                                        <option value="Tổng thầu Thiết kế & Thi công (D&B)">Tổng thầu Thiết kế & Thi công (D&B)</option>
                                        <option value="Thi công công trình Dân dụng / Khách sạn / Biệt thự">Thi công Dân dụng / Khách sạn / Biệt thự</option>
                                        <option value="Thi công Nhà xưởng & Công nghiệp">Thi công Nhà xưởng & Công nghiệp</option>
                                        <option value="Tư vấn Quản lý dự án & Giám sát">Tư vấn Quản lý dự án & Giám sát</option>
                                        <option value="Ứng tuyển nhân sự (QS / Chỉ huy trưởng / Kỹ sư)">Ứng tuyển nhân sự (QS / Kỹ sư / Kế toán)</option>
                                    </select>
                                </div>
                            </div>

                            <div>
                                <label class="block text-xs font-bold uppercase text-slate-700 mb-1.5">Nội dung chi tiết (Quy mô, địa điểm dự án...)</label>
                                <textarea id="cf-message" rows="4" placeholder="Mô tả sơ bộ nhu cầu thiết kế, thi công hoặc vị trí ứng tuyển..." class="w-full px-4 py-3 rounded-xl bg-slate-50 border border-slate-200 focus:border-acon-blue focus:bg-white focus:outline-none text-sm"></textarea>
                            </div>

                            <button type="submit" class="btn-newtecons w-full bg-acon-navy hover:bg-acon-blue text-white font-display font-bold text-sm uppercase tracking-wider py-4 rounded-xl shadow-lg transition-all flex items-center justify-center gap-2">
                                <i class="fa-solid fa-paper-plane"></i>
                                <span>Gửi thông tin đến ACON (acondn.vn)</span>
                            </button>
                        </form>

                        <!-- Notification Box -->
                        <div id="contact-success" class="hidden mt-4 p-4 rounded-2xl bg-emerald-50 border border-emerald-200 text-emerald-800 text-xs sm:text-sm">
                            <div class="flex items-center gap-2 font-bold">
                                <i class="fa-solid fa-circle-check text-emerald-600 text-lg"></i>
                                <span>Đã ghi nhận yêu cầu thành công!</span>
                            </div>
                            <p class="mt-1">Cảm ơn Quý khách đã liên hệ <strong>CÔNG TY CỔ PHẦN ĐẦU TƯ XÂY DỰNG ACON</strong>. Bộ phận phụ trách sẽ liên hệ lại qua số điện thoại Quý khách vừa cung cấp hoặc Quý khách có thể gọi trực tiếp Hotline <strong>0916.104.099</strong>.</p>
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- ==========================================
         NEWTECONS-STYLE CORPORATE FOOTER
    =========================================== -->
    <footer class="bg-acon-dark text-white pt-16 pb-10 border-t border-white/10 bg-blueprint-dark">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-12 gap-10 pb-12 border-b border-white/10">
                
                <!-- Col 1: Brand Info (5 cols) -->
                <div class="lg:col-span-5 space-y-4">
                    <div class="flex items-center gap-3">
                        <div class="w-12 h-12 rounded-xl bg-white flex items-center justify-center p-1.5">
                            <span class="font-display font-black text-acon-navy text-lg"><span class="text-acon-red">Λ</span>CON</span>
                        </div>
                        <div>
                            <h3 class="font-display font-extrabold text-base sm:text-lg text-white">CÔNG TY CỔ PHẦN ĐẦU TƯ XÂY DỰNG ACON</h3>
                            <p class="text-xs text-acon-cyan font-semibold">ACON INVESTMENT CONSTRUCTION JOINT STOCK COMPANY</p>
                        </div>
                    </div>
                    <p class="text-xs sm:text-sm text-white/70 leading-relaxed">
                        Biểu tượng của Niềm tin, Chất lượng và Sự bền vững trong lĩnh vực Thiết kế, Quản lý dự án, Giám sát và Thi công xây dựng công trình Dân dụng – Công nghiệp tại Đà Nẵng và Miền Trung.
                    </p>
                    <div class="flex items-center gap-3 pt-2">
                        <a href="https://www.facebook.com/aconvn.construction" target="_blank" rel="noopener noreferrer" class="w-10 h-10 rounded-xl bg-white/10 hover:bg-[#1877F2] flex items-center justify-center text-white transition-all" title="Fanpage ACON Construction">
                            <i class="fa-brands fa-facebook-f"></i>
                        </a>
                        <a href="tel:0916104099" class="w-10 h-10 rounded-xl bg-white/10 hover:bg-acon-red flex items-center justify-center text-white transition-all" title="Gọi 0916.104.099">
                            <i class="fa-solid fa-phone"></i>
                        </a>
                        <a href="mailto:acon.dng@gmail.com" class="w-10 h-10 rounded-xl bg-white/10 hover:bg-acon-cyan flex items-center justify-center text-white transition-all" title="Email acon.dng@gmail.com">
                            <i class="fa-solid fa-envelope"></i>
                        </a>
                    </div>
                </div>

                <!-- Col 2: Quick Links (3 cols) -->
                <div class="lg:col-span-3 space-y-3">
                    <h4 class="font-display font-bold text-xs uppercase tracking-widest text-acon-cyan">Danh mục website</h4>
                    <ul class="space-y-2.5 text-xs sm:text-sm text-white/75">
                        <li><a href="#sec-02" class="hover:text-acon-cyan transition-colors">Giới thiệu & Lịch sử hình thành</a></li>
                        <li><a href="#sec-03" class="hover:text-acon-cyan transition-colors">Tổng thầu Thiết kế & Thi công (D&B)</a></li>
                        <li><a href="#sec-04" class="hover:text-acon-cyan transition-colors">Chứng chỉ năng lực HĐXD (00076275)</a></li>
                        <li><a href="#sec-05" class="hover:text-acon-cyan transition-colors">Dự án tiêu biểu</a></li>
                        <li><a href="#sec-06" class="hover:text-acon-cyan transition-colors">Tin tức Fanpage & Tuyển dụng</a></li>
                    </ul>
                </div>

                <!-- Col 3: Direct Contact Details (4 cols) -->
                <div class="lg:col-span-4 space-y-3">
                    <h4 class="font-display font-bold text-xs uppercase tracking-widest text-acon-cyan">Thông tin liên hệ</h4>
                    <ul class="space-y-2.5 text-xs sm:text-sm text-white/80">
                        <li><strong class="text-white">Địa chỉ:</strong> 145-147 Trung Lương 14, P. Hòa Xuân, Q. Cẩm Lệ, TP. Đà Nẵng</li>
                        <li><strong class="text-white">Hotline:</strong> <a href="tel:0916104099" class="text-acon-cyan font-bold">0916.104.099</a> | ĐT: 02363.789.769</li>
                        <li><strong class="text-white">Email:</strong> acon.dng@gmail.com</li>
                        <li><strong class="text-white">Website:</strong> <a href="#sec-01" class="text-acon-cyan">https://acondn.vn</a></li>
                        <li><strong class="text-white">Fanpage:</strong> <a href="https://www.facebook.com/aconvn.construction" target="_blank" rel="noopener noreferrer" class="underline hover:text-acon-cyan">fb.com/aconvn.construction</a></li>
                    </ul>
                </div>

            </div>

            <div class="pt-8 flex flex-col sm:flex-row items-center justify-between gap-4 text-xs text-white/50">
                <p>© 2026 CÔNG TY CỔ PHẦN ĐẦU TƯ XÂY DỰNG ACON (acondn.vn). All rights reserved.</p>
                <p>MST: 0401676571 • Mã chứng chỉ năng lực HĐXD: 00076275 • Đà Nẵng, Việt Nam</p>
            </div>
        </div>
    </footer>

    <!-- ==========================================
         MODAL 1: CHI TIẾT DỰ ÁN (PROJECT DETAIL MODAL)
    =========================================== -->
    <div id="project-modal" class="fixed inset-0 z-50 bg-acon-dark/90 backdrop-blur-md hidden items-center justify-center p-4 overflow-y-auto">
        <div class="bg-white rounded-3xl max-w-4xl w-full overflow-hidden shadow-2xl border border-slate-200 my-8">
            <div class="relative h-72 sm:h-96 bg-acon-navy">
                <img id="pm-img" src="" alt="" class="w-full h-full object-cover" />
                <div class="absolute inset-0 bg-gradient-to-t from-acon-dark/90 via-transparent to-black/30"></div>
                <button onclick="closeProjectModal()" class="absolute top-4 right-4 w-10 h-10 rounded-full bg-black/50 hover:bg-acon-red text-white flex items-center justify-center transition-all">
                    <i class="fa-solid fa-xmark"></i>
                </button>
                <div class="absolute bottom-6 left-6 right-6 text-white">
                    <span id="pm-category" class="px-3 py-1 rounded-full bg-acon-cyan text-xs font-bold uppercase tracking-wider"></span>
                    <h3 id="pm-title" class="font-display font-black text-2xl sm:text-3xl mt-2"></h3>
                </div>
            </div>
            <div class="p-6 sm:p-8">
                <div class="grid grid-cols-2 sm:grid-cols-4 gap-4 pb-6 border-b border-slate-200 text-xs">
                    <div class="bg-slate-50 p-3.5 rounded-2xl">
                        <span class="text-slate-400 uppercase font-bold block">Địa điểm</span>
                        <strong id="pm-location" class="text-acon-navy text-sm mt-0.5 block"></strong>
                    </div>
                    <div class="bg-slate-50 p-3.5 rounded-2xl">
                        <span class="text-slate-400 uppercase font-bold block">Vai trò ACON</span>
                        <strong id="pm-role" class="text-acon-blue text-sm mt-0.5 block"></strong>
                    </div>
                    <div class="bg-slate-50 p-3.5 rounded-2xl">
                        <span class="text-slate-400 uppercase font-bold block">Quy mô</span>
                        <strong id="pm-scale" class="text-acon-navy text-sm mt-0.5 block"></strong>
                    </div>
                    <div class="bg-slate-50 p-3.5 rounded-2xl">
                        <span class="text-slate-400 uppercase font-bold block">Năm thực hiện</span>
                        <strong id="pm-year" class="text-acon-navy text-sm mt-0.5 block"></strong>
                    </div>
                </div>
                <p id="pm-desc" class="text-slate-600 text-sm sm:text-base leading-relaxed mt-6"></p>
                <div class="mt-8 flex flex-wrap justify-between items-center gap-4 pt-4 border-t border-slate-100">
                    <a href="https://www.facebook.com/aconvn.construction" target="_blank" rel="noopener noreferrer" class="text-xs font-bold text-[#1877F2] hover:underline flex items-center gap-1.5">
                        <i class="fa-brands fa-facebook"></i> Xem thêm hình ảnh thi công trên Fanpage ACON Construction
                    </a>
                    <button onclick="closeProjectModal()" class="px-6 py-2.5 rounded-xl bg-acon-navy text-white font-display font-bold text-xs uppercase">Đóng cửa sổ</button>
                </div>
            </div>
        </div>
    </div>

    <!-- ==========================================
         MODAL 2: HỒ SƠ NĂNG LỰC & BẢNG CHỨNG CHỈ 00076275
    =========================================== -->
    <div id="profile-modal" class="fixed inset-0 z-50 bg-acon-dark/90 backdrop-blur-md hidden items-center justify-center p-4 overflow-y-auto">
        <div class="bg-white rounded-3xl max-w-4xl w-full overflow-hidden shadow-2xl border border-slate-200 my-8">
            <div class="bg-acon-navy text-white p-6 sm:p-8 flex items-center justify-between">
                <div>
                    <span class="text-xs font-bold text-acon-cyan uppercase tracking-widest">HỒ SƠ PHÁP LÝ & NĂNG LỰC</span>
                    <h3 class="font-display font-black text-xl sm:text-2xl mt-1">CÔNG TY CỔ PHẦN ĐẦU TƯ XÂY DỰNG ACON</h3>
                </div>
                <button onclick="closeProfileModal()" class="w-10 h-10 rounded-full bg-white/10 hover:bg-acon-red text-white flex items-center justify-center">
                    <i class="fa-solid fa-xmark"></i>
                </button>
            </div>
            <div class="p-6 sm:p-8 max-h-[75vh] overflow-y-auto space-y-6 text-xs sm:text-sm">
                <div class="grid grid-cols-1 sm:grid-cols-2 gap-4 bg-slate-50 p-5 rounded-2xl border border-slate-200">
                    <div><strong>Tên doanh nghiệp:</strong> CÔNG TY CỔ PHẦN ĐẦU TƯ XÂY DỰNG ACON</div>
                    <div><strong>Tên quốc tế:</strong> ACON INVESTMENT CONSTRUCTION.,JSC</div>
                    <div><strong>Người đại diện pháp luật:</strong> Ông Huỳnh Bá Quý (Giám đốc)</div>
                    <div><strong>Mã số thuế:</strong> 0401676571 (Cấp ngày 14/05/2015)</div>
                    <div><strong>Mã chứng chỉ năng lực HĐXD:</strong> <span class="text-acon-red font-bold">00076275</span></div>
                    <div><strong>Văn phòng giao dịch:</strong> 145-147 Trung Lương 14, Hòa Xuân, Đà Nẵng</div>
                </div>

                <h4 class="font-display font-bold text-acon-navy text-base uppercase">Bảng tổng hợp phạm vi hoạt động xây dựng được cấp phép (Số CC: HCM-00076275):</h4>
                <div class="overflow-x-auto">
                    <table class="w-full text-left border-collapse border border-slate-200 rounded-xl overflow-hidden">
                        <thead class="bg-acon-navy text-white text-xs uppercase">
                            <tr>
                                <th class="p-3 border border-slate-200">STT</th>
                                <th class="p-3 border border-slate-200">Lĩnh vực hoạt động</th>
                                <th class="p-3 border border-slate-200">Loại công trình</th>
                                <th class="p-3 border border-slate-200">Hạng</th>
                                <th class="p-3 border border-slate-200">Hiệu lực đến</th>
                            </tr>
                        </thead>
                        <tbody class="divide-y divide-slate-200 text-xs">
                            <tr class="bg-red-50/60 font-semibold">
                                <td class="p-3">1</td>
                                <td class="p-3">Thi công xây dựng công trình</td>
                                <td class="p-3">Công trình Dân dụng</td>
                                <td class="p-3 text-acon-red font-bold">Hạng II</td>
                                <td class="p-3">27/09/2033</td>
                            </tr>
                            <tr>
                                <td class="p-3">2</td>
                                <td class="p-3">Thi công xây dựng công trình</td>
                                <td class="p-3">Công trình Nhà công nghiệp</td>
                                <td class="p-3 font-bold text-acon-blue">Hạng III</td>
                                <td class="p-3">27/09/2033</td>
                            </tr>
                            <tr>
                                <td class="p-3">3</td>
                                <td class="p-3">Thiết kế, thẩm tra thiết kế xây dựng</td>
                                <td class="p-3">Dân dụng & Nhà công nghiệp</td>
                                <td class="p-3 font-bold text-acon-blue">Hạng III</td>
                                <td class="p-3">27/09/2033</td>
                            </tr>
                            <tr>
                                <td class="p-3">4</td>
                                <td class="p-3">Tư vấn quản lý dự án đầu tư xây dựng</td>
                                <td class="p-3">Dân dụng & Công nghiệp</td>
                                <td class="p-3 font-bold text-acon-blue">Hạng III</td>
                                <td class="p-3">27/09/2033</td>
                            </tr>
                            <tr>
                                <td class="p-3">5</td>
                                <td class="p-3">Thi công lắp đặt thiết bị vào công trình</td>
                                <td class="p-3">Dân dụng & Nhà công nghiệp</td>
                                <td class="p-3 font-bold text-acon-blue">Hạng III</td>
                                <td class="p-3">27/09/2033</td>
                            </tr>
                            <tr>
                                <td class="p-3">6</td>
                                <td class="p-3">Tư vấn giám sát công tác xây dựng</td>
                                <td class="p-3">Dân dụng & Công nghiệp</td>
                                <td class="p-3 font-bold text-acon-blue">Hạng III</td>
                                <td class="p-3">27/09/2033</td>
                            </tr>
                        </tbody>
                    </table>
                </div>
            </div>
        </div>
    </div>

    <!-- ==========================================
         MODAL 3: ĐỒNG BỘ LOGO & THÊM DỰ ÁN TỪ FANPAGE
    =========================================== -->
    <div id="logo-modal" class="fixed inset-0 z-50 bg-acon-dark/90 backdrop-blur-md hidden items-center justify-center p-4 overflow-y-auto">
        <div class="bg-white rounded-3xl max-w-2xl w-full overflow-hidden shadow-2xl border border-slate-200 my-8">
            <div class="bg-acon-navy text-white p-6 flex items-center justify-between">
                <div>
                    <span class="text-xs font-bold text-acon-cyan uppercase">Quản trị nội dung Fanpage</span>
                    <h3 class="font-display font-bold text-lg mt-0.5">Cập nhật Logo & Hình ảnh dự án từ Fanpage ACON</h3>
                </div>
                <button onclick="closeLogoModal()" class="w-9 h-9 rounded-full bg-white/10 hover:bg-acon-red text-white flex items-center justify-center">
                    <i class="fa-solid fa-xmark"></i>
                </button>
            </div>
            <div class="p-6 space-y-6 text-xs sm:text-sm">
                <!-- Part 1: Upload / Link Logo from Fanpage -->
                <div class="bg-slate-50 p-5 rounded-2xl border border-slate-200 space-y-3">
                    <h4 class="font-display font-bold text-acon-navy text-sm uppercase">1. Thay đổi Logo từ máy tính hoặc URL ảnh Fanpage</h4>
                    <p class="text-xs text-slate-500">Bạn có thể tải trực tiếp file ảnh Logo tải về từ trang <a href="https://www.facebook.com/aconvn.construction" target="_blank" class="text-acon-blue underline">facebook.com/aconvn.construction</a> hoặc dán đường dẫn ảnh vào đây:</p>
                    <div class="flex flex-col sm:flex-row gap-3">
                        <input type="file" id="logo-file-input" accept="image/*" onchange="handleLogoUpload(event)" class="text-xs file:mr-3 file:py-2 file:px-4 file:rounded-xl file:border-0 file:text-xs file:font-bold file:bg-acon-blue file:text-white hover:file:bg-acon-navy" />
                        <button onclick="resetDefaultLogo()" class="px-4 py-2 rounded-xl bg-slate-200 hover:bg-slate-300 text-slate-700 font-semibold text-xs">Khôi phục Logo Vector ΛCON</button>
                    </div>
                </div>

                <!-- Part 2: Add New Project from Fanpage -->
                <form onsubmit="handleAddProject(event)" class="bg-slate-50 p-5 rounded-2xl border border-slate-200 space-y-3">
                    <h4 class="font-display font-bold text-acon-navy text-sm uppercase">2. Đăng thêm dự án mới từ Fanpage lên Website</h4>
                    <div class="grid grid-cols-1 sm:grid-cols-2 gap-3">
                        <input type="text" id="np-title" required placeholder="Tên dự án (VD: Khách sạn Mỹ Khê...)" class="px-3.5 py-2.5 rounded-xl bg-white border border-slate-200 text-xs" />
                        <select id="np-cat" class="px-3.5 py-2.5 rounded-xl bg-white border border-slate-200 text-xs">
                            <option value="commercial">Khách sạn & Văn phòng</option>
                            <option value="residential">Biệt thự & Dân dụng</option>
                            <option value="industrial">Nhà xưởng & Công nghiệp</option>
                        </select>
                    </div>
                    <div class="grid grid-cols-1 sm:grid-cols-2 gap-3">
                        <input type="text" id="np-loc" required placeholder="Địa điểm (VD: Sơn Trà, Đà Nẵng)" class="px-3.5 py-2.5 rounded-xl bg-white border border-slate-200 text-xs" />
                        <input type="url" id="np-img" required placeholder="Dán link ảnh dự án từ Fanpage..." class="px-3.5 py-2.5 rounded-xl bg-white border border-slate-200 text-xs" />
                    </div>
                    <textarea id="np-desc" rows="2" placeholder="Mô tả gói thầu thi công..." class="w-full px-3.5 py-2.5 rounded-xl bg-white border border-slate-200 text-xs"></textarea>
                    <button type="submit" class="w-full py-3 rounded-xl bg-acon-cyan hover:bg-sky-500 text-white font-display font-bold text-xs uppercase tracking-wider">
                        <i class="fa-solid fa-cloud-arrow-up mr-1.5"></i>Đưa dự án lên trang chủ acondn.vn
                    </button>
                </form>
            </div>
        </div>
    </div>

    <!-- ==========================================
         MODAL 4: CHI TIẾT TIN TỨC & TUYỂN DỤNG
    =========================================== -->
    <div id="news-modal" class="fixed inset-0 z-50 bg-acon-dark/90 backdrop-blur-md hidden items-center justify-center p-4 overflow-y-auto">
        <div class="bg-white rounded-3xl max-w-2xl w-full overflow-hidden shadow-2xl border border-slate-200 my-8">
            <div class="bg-acon-navy text-white p-6 flex items-center justify-between">
                <span id="nm-badge" class="px-3 py-1 rounded-full bg-acon-cyan text-xs font-bold uppercase">Tin tức ACON</span>
                <button onclick="closeNewsModal()" class="w-9 h-9 rounded-full bg-white/10 hover:bg-acon-red text-white flex items-center justify-center">
                    <i class="fa-solid fa-xmark"></i>
                </button>
            </div>
            <div class="p-6 sm:p-8 space-y-4">
                <h3 id="nm-title" class="font-display font-black text-xl sm:text-2xl text-acon-navy"></h3>
                <p id="nm-date" class="text-xs font-bold text-acon-blue"></p>
                <div id="nm-body" class="text-slate-600 text-sm sm:text-base leading-relaxed space-y-3"></div>
                <div class="pt-6 border-t border-slate-100 flex justify-between items-center">
                    <a href="https://www.facebook.com/aconvn.construction" target="_blank" rel="noopener noreferrer" class="text-xs font-bold text-[#1877F2] hover:underline">
                        <i class="fa-brands fa-facebook mr-1"></i>Xem bài gốc trên Fanpage
                    </a>
                    <button onclick="closeNewsModal()" class="px-5 py-2 rounded-xl bg-slate-100 hover:bg-slate-200 text-slate-700 font-bold text-xs">Đóng</button>
                </div>
            </div>
        </div>
    </div>

    <!-- ==========================================
         JAVASCRIPT LOGIC & NEWTECONS INTERACTIVE EFFECTS
    =========================================== -->
    <script>
        // 1. Dữ liệu Dự án tiêu biểu của CÔNG TY CỔ PHẦN ĐẦU TƯ XÂY DỰNG ACON
        let aconProjects = [
            {
                id: 1,
                title: "TỔ HỢP KHÁCH SẠN & CĂN HỘ DỊCH VỤ VEN BIỂN MỸ KHÊ",
                category: "commercial",
                categoryName: "Khách sạn & Thương mại",
                location: "Quận Sơn Trà, TP. Đà Nẵng",
                role: "Tổng thầu Thiết kế & Thi công (D&B)",
                scale: "12 tầng nổi + 1 tầng hầm, 4.800 m² sàn",
                year: "2025 - 2026",
                image: "https://images.unsplash.com/photo-1545324418-cc1a3fa10c00?auto=format&fit=crop&w=900&q=80",
                desc: "Dự án khách sạn và căn hộ lưu trú cao cấp tại khu vực biển Sơn Trà, Đà Nẵng. ACON đảm nhận vai trò Tổng thầu thi công phần ngầm, kết cấu bê tông cốt thép, hoàn thiện kiến trúc mặt dựng kính và hệ thống Cơ điện (M&E) đạt chuẩn khách sạn 4 sao."
            },
            {
                id: 2,
                title: "TÒA NHÀ VĂN PHÒNG & TRỤ SỞ ĐIỀU HÀNH HÒA XUÂN",
                category: "commercial",
                categoryName: "Văn phòng & Thương mại",
                location: "Trung Lương 14, P. Hòa Xuân, Đà Nẵng",
                role: "Thiết kế, Thi công & Hoàn thiện Nội thất",
                scale: "Tòa nhà 5 tầng hiện đại, không gian mở",
                year: "2024 - 2026",
                image: "https://images.unsplash.com/photo-1486406146926-c627a92ad1ab?auto=format&fit=crop&w=900&q=80",
                desc: "Công trình văn phòng hiện đại tại khu đô thị sinh thái Hòa Xuân, Cẩm Lệ, Đà Nẵng. Thiết kế mặt đứng kiến trúc xanh kết hợp hệ lam chắn nắng và không gian làm việc tiêu chuẩn cao."
            },
            {
                id: 3,
                title: "BIỆT THỰ NGHỈ DƯỠNG SINH THÁI NAM HÒA XUÂN & EURO VILLAGE",
                category: "residential",
                categoryName: "Biệt thự & Dân dụng cao cấp",
                location: "KĐT Hòa Xuân & Sơn Trà, Đà Nẵng",
                role: "Tổng thầu Thi công trọn gói & Nội thất",
                scale: "Biệt thự 3 tầng + Hồ bơi sân vườn, 650 m²",
                year: "2025",
                image: "https://images.unsplash.com/photo-1600596542815-ffad4c1539a9?auto=format&fit=crop&w=900&q=80",
                desc: "Chuỗi các công trình biệt thự hiện đại ven sông tại khu đô thị Hòa Xuân và Euro Village Đà Nẵng do ACON Construction trực tiếp thi công kết cấu và hoàn thiện trọn gói với độ tinh xảo cao."
            },
            {
                id: 4,
                title: "NHÀ MÁY SẢN XUẤT & TRUNG TÂM KHO VẬN KCN HÒA KHÁNH",
                category: "industrial",
                categoryName: "Nhà xưởng & Công nghiệp",
                location: "KCN Hòa Khánh, Liên Chiểu, Đà Nẵng",
                role: "Thi công Nhà công nghiệp & Hạ tầng",
                scale: "12.500 m² nhà xưởng kết cấu thép & văn phòng",
                year: "2024 - 2025",
                image: "https://images.unsplash.com/photo-1581092160607-ee22621dd758?auto=format&fit=crop&w=900&q=80",
                desc: "Thi công xây dựng công trình nhà xưởng công nghiệp, nền sàn bê tông chịu lực cao, lắp dựng kết cấu thép khẩu độ lớn, hệ thống PCCC và hạ tầng kỹ thuật đồng bộ."
            },
            {
                id: 5,
                title: "TÒA NHÀ THƯƠNG MẠI DỊCH VỤ & SHOWROOM HẢI CHÂU",
                category: "commercial",
                categoryName: "Khách sạn & Thương mại",
                location: "Quận Hải Châu, TP. Đà Nẵng",
                role: "Tổng thầu Thi công & Lắp đặt thiết bị",
                scale: "7 tầng nổi + 1 bán hầm, 2.400 m² sàn",
                year: "2025",
                image: "https://images.unsplash.com/photo-1554469384-e58fac16e23a?auto=format&fit=crop&w=900&q=80",
                desc: "Công trình phức hợp showroom trưng bày và văn phòng cho thuê tại trung tâm quận Hải Châu, ứng dụng giải pháp sàn vượt nhịp và mặt dựng nhôm kính hiện đại."
            },
            {
                id: 6,
                title: "KHU NHÀ PHỐ THƯƠNG MẠI (SHOPHOUSE) & VILLA PHỐ BIỂN",
                category: "residential",
                categoryName: "Biệt thự & Dân dụng cao cấp",
                location: "Quận Ngũ Hành Sơn, TP. Đà Nẵng",
                role: "Tư vấn QLDA, Giám sát & Thi công",
                scale: "Tổ hợp 14 căn Shophouse & Villa liền kề",
                year: "2024 - 2026",
                image: "https://images.unsplash.com/photo-1600585154340-be6161a56a0c?auto=format&fit=crop&w=900&q=80",
                desc: "Dự án khu nhà phố thương mại kết hợp nghỉ dưỡng đạt chuẩn chất lượng Hạng II, đảm bảo tiến độ bàn giao đồng loạt và thẩm mỹ kiến trúc đồng bộ."
            }
        ];

        // 2. Render danh sách dự án
        function renderProjects(filter = 'all') {
            const grid = document.getElementById('projects-grid');
            const filtered = filter === 'all' ? aconProjects : aconProjects.filter(p => p.category === filter);

            grid.innerHTML = filtered.map((proj, idx) => `
                <article onclick="openProjectModal(${proj.id})" class="project-card group relative rounded-3xl overflow-hidden shadow-lg cursor-pointer h-[390px] bg-acon-navy border border-slate-200/60">
                    <img src="${proj.image}" 
                         onerror="this.src='https://placehold.co/800x600/002B5B/FFFFFF?text=ACON+PROJECT'"
                         alt="${proj.title}" 
                         class="w-full h-full object-cover" />
                    <div class="project-overlay absolute inset-0 p-6 sm:p-7 flex flex-col justify-between text-white">
                        <div class="flex items-center justify-between">
                            <span class="px-3 py-1 rounded-full bg-acon-cyan/90 text-white text-[11px] font-bold uppercase tracking-wider shadow">
                                ${proj.categoryName}
                            </span>
                            <span class="w-9 h-9 rounded-full bg-white/15 backdrop-blur-md flex items-center justify-center group-hover:bg-acon-cyan transition-colors">
                                <i class="fa-solid fa-arrow-up-right-from-square text-xs"></i>
                            </span>
                        </div>
                        <div>
                            <p class="text-xs text-acon-cyan font-semibold mb-1 flex items-center gap-1.5">
                                <i class="fa-solid fa-location-dot"></i> ${proj.location} • ${proj.year}
                            </p>
                            <h3 class="font-display font-extrabold text-lg sm:text-xl leading-snug group-hover:text-sky-200 transition-colors">
                                ${proj.title}
                            </h3>
                            <div class="mt-3 pt-3 border-t border-white/15 flex items-center justify-between text-xs text-white/80">
                                <span><strong>Gói thầu:</strong> ${proj.role}</span>
                            </div>
                        </div>
                    </div>
                </article>
            `).join('');
        }

        function filterProjects(cat) {
            document.querySelectorAll('.proj-filter-btn').forEach(btn => {
                if (btn.dataset.filter === cat) {
                    btn.className = "proj-filter-btn active px-4 py-2.5 rounded-xl font-display font-bold text-xs uppercase tracking-wider bg-acon-navy text-white shadow-md transition-all";
                } else {
                    btn.className = "proj-filter-btn px-4 py-2.5 rounded-xl font-display font-bold text-xs uppercase tracking-wider bg-white text-slate-700 hover:bg-acon-blue hover:text-white transition-all border border-slate-200";
                }
            });
            renderProjects(cat);
        }

        // 3. Modal Chi tiết dự án
        function openProjectModal(id) {
            const proj = aconProjects.find(p => p.id === id);
            if (!proj) return;
            document.getElementById('pm-img').src = proj.image;
            document.getElementById('pm-category').textContent = proj.categoryName;
            document.getElementById('pm-title').textContent = proj.title;
            document.getElementById('pm-location').textContent = proj.location;
            document.getElementById('pm-role').textContent = proj.role;
            document.getElementById('pm-scale').textContent = proj.scale;
            document.getElementById('pm-year').textContent = proj.year;
            document.getElementById('pm-desc').textContent = proj.desc;

            const modal = document.getElementById('project-modal');
            modal.classList.remove('hidden');
            modal.classList.add('flex');
        }

        function closeProjectModal() {
            const modal = document.getElementById('project-modal');
            modal.classList.add('hidden');
            modal.classList.remove('flex');
        }

        // 4. Hero Slider Logic (Newtecons Style)
        const heroData = [
            {
                title: `CÔNG TY CỔ PHẦN <br/><span class="text-transparent bg-clip-text bg-gradient-to-r from-acon-cyan via-sky-300 to-white">ĐẦU TƯ XÂY DỰNG ACON</span>`,
                subtitle: `Sự tin tưởng của Chủ đầu tư là chuẩn mực cho giá trị của ACON Construction. Chúng tôi tự hào là Tổng thầu Thiết kế & Thi công (Design & Build) các công trình Dân dụng, Thương mại, Khách sạn và Công nghiệp uy tín hàng đầu tại Đà Nẵng & khu vực Miền Trung.`
            },
            {
                title: `KIẾN TẠO CÔNG TRÌNH <br/><span class="text-transparent bg-clip-text bg-gradient-to-r from-amber-300 via-acon-cyan to-white">VỮNG BỀN THEO THỜI GIAN</span>`,
                subtitle: `Sở hữu Chứng chỉ năng lực Hoạt động Xây dựng Hạng II (Mã số 00076275), ACON cam kết chuẩn mực Kỹ - Mỹ thuật vượt trội, an toàn tuyệt đối và tối ưu tiến độ cho mọi dự án.`
            },
            {
                title: `ĐỘI NGŨ KỸ SƯ TÂM HUYẾT <br/><span class="text-transparent bg-clip-text bg-gradient-to-r from-acon-cyan via-sky-300 to-white">TRỤ SỞ HÒA XUÂN, ĐÀ NẴNG</span>`,
                subtitle: `Văn phòng điều hành tại 145-147 Trung Lương 14, P. Hòa Xuân, Đà Nẵng quy tụ đội ngũ Chỉ huy trưởng, Kỹ sư QS, Kiến trúc sư giàu kinh nghiệm thực chiến trên khắp Miền Trung.`
            }
        ];

        let currentHeroSlide = 0;
        function setHeroSlide(index) {
            currentHeroSlide = index;
            const slides = document.querySelectorAll('.hero-slide');
            slides.forEach((s, idx) => {
                s.style.opacity = idx === index ? '1' : '0';
            });

            document.getElementById('hero-title').innerHTML = heroData[index].title;
            document.getElementById('hero-subtitle').textContent = heroData[index].subtitle;

            [0, 1, 2].forEach(i => {
                const bar = document.getElementById(`hero-bar-${i}`);
                if (bar) bar.style.width = i === index ? '100%' : '0%';
            });
        }

        setInterval(() => {
            setHeroSlide((currentHeroSlide + 1) % 3);
        }, 6500);

        // 5. About Tabs Switcher
        function switchAboutTab(tab) {
            const historyPanel = document.getElementById('tab-panel-history');
            const valuesPanel = document.getElementById('tab-panel-values');
            const btnHistory = document.getElementById('tab-btn-history');
            const btnValues = document.getElementById('tab-btn-values');

            if (tab === 'history') {
                historyPanel.classList.remove('hidden');
                valuesPanel.classList.add('hidden');
                btnHistory.className = "about-tab-btn group text-left p-5 rounded-2xl bg-acon-navy text-white shadow-lg transition-all";
                btnValues.className = "about-tab-btn group text-left p-5 rounded-2xl bg-slate-100 hover:bg-acon-navy hover:text-white text-acon-navy transition-all";
            } else {
                historyPanel.classList.add('hidden');
                valuesPanel.classList.remove('hidden');
                btnValues.className = "about-tab-btn group text-left p-5 rounded-2xl bg-acon-navy text-white shadow-lg transition-all";
                btnHistory.className = "about-tab-btn group text-left p-5 rounded-2xl bg-slate-100 hover:bg-acon-navy hover:text-white text-acon-navy transition-all";
            }
        }

        // 6. Fullscreen Mega Menu Toggle
        function toggleMegaMenu() {
            const menu = document.getElementById('mega-menu');
            if (menu.classList.contains('hidden')) {
                menu.classList.remove('hidden');
                setTimeout(() => menu.classList.remove('opacity-0'), 20);
            } else {
                menu.classList.add('opacity-0');
                setTimeout(() => menu.classList.add('hidden'), 300);
            }
        }

        // 7. Modals (Profile, Logo/Fanpage Sync, News)
        function openProfileModal() {
            const m = document.getElementById('profile-modal');
            m.classList.remove('hidden');
            m.classList.add('flex');
        }
        function closeProfileModal() {
            const m = document.getElementById('profile-modal');
            m.classList.add('hidden');
            m.classList.remove('flex');
        }

        function openLogoModal() {
            const m = document.getElementById('logo-modal');
            m.classList.remove('hidden');
            m.classList.add('flex');
        }
        function closeLogoModal() {
            const m = document.getElementById('logo-modal');
            m.classList.add('hidden');
            m.classList.remove('flex');
        }

        function handleLogoUpload(event) {
            const file = event.target.files[0];
            if (!file) return;
            const reader = new FileReader();
            reader.onload = function(e) {
                const img = document.getElementById('custom-logo-img');
                const svg = document.getElementById('default-logo-svg');
                img.src = e.target.result;
                img.classList.remove('hidden');
                svg.classList.add('hidden');
                closeLogoModal();
            };
            reader.readAsDataURL(file);
        }

        function resetDefaultLogo() {
            document.getElementById('custom-logo-img').classList.add('hidden');
            document.getElementById('default-logo-svg').classList.remove('hidden');
        }

        function handleAddProject(e) {
            e.preventDefault();
            const title = document.getElementById('np-title').value;
            const category = document.getElementById('np-cat').value;
            const location = document.getElementById('np-loc').value;
            const image = document.getElementById('np-img').value;
            const desc = document.getElementById('np-desc').value || "Dự án tiêu biểu được cập nhật từ Fanpage chính thức của CÔNG TY CỔ PHẦN ĐẦU TƯ XÂY DỰNG ACON.";

            const catMap = {
                commercial: "Khách sạn & Văn phòng",
                residential: "Biệt thự & Dân dụng",
                industrial: "Nhà xưởng & Công nghiệp"
            };

            aconProjects.unshift({
                id: Date.now(),
                title: title.toUpperCase(),
                category,
                categoryName: catMap[category],
                location,
                role: "Tổng thầu Thiết kế & Thi công",
                scale: "Theo hồ sơ thiết kế kỹ thuật",
                year: "2026",
                image,
                desc
            });

            renderProjects('all');
            closeLogoModal();
            document.getElementById('sec-05').scrollIntoView({ behavior: 'smooth' });
        }

        // 8. News & Recruitment Modal Data
        const newsArticles = [
            {
                badge: "Tin công trường Fanpage",
                title: "ACON CONSTRUCTION ĐẨY MẠNH TIẾN ĐỘ THI CÔNG & NGHIỆM THU CÁC DỰ ÁN DÂN DỤNG – THƯƠNG MẠI TẠI ĐÀ NẴNG",
                date: "15 Tháng 10, 2026 • Nguồn: fb.com/aconvn.construction",
                body: `
                    <p>Tại các dự án trọng điểm trên địa bàn TP. Đà Nẵng, đội ngũ Ban chỉ huy công trường <strong>CÔNG TY CỔ PHẦN ĐẦU TƯ XÂY DỰNG ACON</strong> đang tập trung tối đa nguồn lực nhân sự và thiết bị để hoàn thành các cột mốc kết cấu & hoàn thiện theo đúng tiến độ cam kết.</p>
                    <p>Mỗi hạng mục từ công tác cốt thép, cốp pha, đổ bê tông thương phẩm đến lắp đặt hệ thống cơ điện (MEP) đều được kiểm tra nghiệm thu nội bộ nghiêm ngặt theo tiêu chuẩn kỹ thuật trước khi bàn giao.</p>
                `
            },
            {
                badge: "Tuyển dụng Nhân sự Đà Nẵng",
                title: "THÔNG BÁO TUYỂN DỤNG: KỸ SƯ QS, CHỈ HUY TRƯỞNG CÔNG TRÌNH, KỸ SƯ HIỆN TRƯỜNG & KẾ TOÁN XÂY DỰNG",
                date: "Đang nhận hồ sơ • Địa điểm: 145-147 Trung Lương 14, Hòa Xuân, Đà Nẵng",
                body: `
                    <p>Nhằm đáp ứng nhu cầu mở rộng quy mô các dự án trong năm 2026, <strong>CÔNG TY CỔ PHẦN ĐẦU TƯ XÂY DỰNG ACON (ACON Construction)</strong> thông báo tuyển dụng các vị trí:</p>
                    <ul class="list-disc pl-5 space-y-1 font-medium text-acon-navy">
                        <li>02 Chuyên viên / Kỹ sư QS (Bóc tách khối lượng, lập dự toán, thanh quyết toán)</li>
                        <li>02 Chỉ huy trưởng Công trình Dân dụng & Công nghiệp</li>
                        <li>03 Kỹ sư Giám sát Hiện trường / Kỹ sư Kết cấu - Hoàn thiện</li>
                        <li>01 Kế toán Xây dựng tổng hợp</li>
                    </ul>
                    <p class="mt-2"><strong>Quyền lợi:</strong> Mức lương thỏa thuận hấp dẫn theo năng lực, đầy đủ chế độ BHXH, thưởng theo tiến độ dự án và môi trường làm việc chuyên nghiệp.</p>
                    <p><strong>Liên hệ nộp hồ sơ:</strong> Văn phòng 145-147 Trung Lương 14, P. Hòa Xuân, TP. Đà Nẵng | Email: <strong>acon.dng@gmail.com</strong> | Hotline: <strong>0916.104.099</strong> (hoặc 02363.789.769).</p>
                `
            },
            {
                badge: "Hoạt động doanh nghiệp",
                title: "CHUẨN HÓA QUY TRÌNH QUẢN LÝ CHẤT LƯỢNG & AN TOÀN VỆ SINH LAO ĐỘNG TRÊN TOÀN HỆ THỐNG CÔNG TRƯỜNG ACON",
                date: "28 Tháng 08, 2026",
                body: `
                    <p>An toàn lao động (HSE) và Chất lượng thi công (QA/QC) luôn là ưu tiên số 1 tại mọi công trường của ACON Construction. Công ty thường xuyên tổ chức các buổi huấn luyện định kỳ và kiểm tra thực tế hệ thống giàn giáo, lưới bao che và thiết bị thi công.</p>
                `
            },
            {
                badge: "Dấu ấn phát triển",
                title: "KỶ NIỆM 11 NĂM HÌNH THÀNH VÀ PHÁT TRIỂN CÔNG TY CỔ PHẦN ĐẦU TƯ XÂY DỰNG ACON (14/05/2015 – 14/05/2026)",
                date: "14 Tháng 05, 2026",
                body: `
                    <p>Trải qua 11 năm xây dựng và trưởng thành kể từ ngày 14/05/2015, tập thể Ban lãnh đạo và CBNV Công ty Cổ phần Đầu tư Xây dựng ACON tự hào đã kiến tạo nên hàng trăm công trình giá trị, khẳng định thương hiệu nhà thầu uy tín tại Đà Nẵng và Miền Trung.</p>
                `
            }
        ];

        function openNewsModal(idx) {
            const item = newsArticles[idx];
            if (!item) return;
            document.getElementById('nm-badge').textContent = item.badge;
            document.getElementById('nm-title').textContent = item.title;
            document.getElementById('nm-date').textContent = item.date;
            document.getElementById('nm-body').innerHTML = item.body;
            const m = document.getElementById('news-modal');
            m.classList.remove('hidden');
            m.classList.add('flex');
        }

        function closeNewsModal() {
            const m = document.getElementById('news-modal');
            m.classList.add('hidden');
            m.classList.remove('flex');
        }

        // 9. Contact Form Handler
        function handleContactSubmit(e) {
            e.preventDefault();
            document.getElementById('contact-success').classList.remove('hidden');
            e.target.reset();
        }

        // 10. Language Switcher (VN / EN)
        function switchLang(lang) {
            const vnBtn = document.getElementById('lang-vn');
            const enBtn = document.getElementById('lang-en');
            if (lang === 'EN') {
                enBtn.className = 'text-acon-cyan font-bold';
                vnBtn.className = 'text-white/60 hover:text-white';
                document.getElementById('hero-title').innerHTML = `ACON INVESTMENT <br/><span class="text-transparent bg-clip-text bg-gradient-to-r from-acon-cyan via-sky-300 to-white">CONSTRUCTION JSC</span>`;
                document.getElementById('hero-subtitle').textContent = `Build On Trust — Your trusted Design & Build General Contractor for Civil, Commercial, Hospitality, and Industrial projects in Da Nang & Central Vietnam.`;
            } else {
                vnBtn.className = 'text-acon-cyan font-bold';
                enBtn.className = 'text-white/60 hover:text-white';
                setHeroSlide(0);
            }
        }

        // 11. Scroll Reveal, Counter Animation & Right-Side Section Pagination (01 - 07)
        let countersStarted = false;
        function startCounters() {
            if (countersStarted) return;
            countersStarted = true;
            document.querySelectorAll('.counter-value').forEach(el => {
                const target = parseInt(el.dataset.target, 10);
                let count = 0;
                const step = Math.max(1, Math.ceil(target / 45));
                const timer = setInterval(() => {
                    count += step;
                    if (count >= target) {
                        el.textContent = target;
                        clearInterval(timer);
                    } else {
                        el.textContent = count;
                    }
                }, 30);
            });
        }

        function handleScrollEffects() {
            // Reveal elements on scroll
            document.querySelectorAll('.reveal-up, .reveal-left, .reveal-right').forEach(el => {
                const rect = el.getBoundingClientRect();
                if (rect.top < window.innerHeight - 60) {
                    el.classList.add('active');
                }
            });

            // Trigger counters when Section 04 enters viewport
            const counterGrid = document.getElementById('counters-grid');
            if (counterGrid && counterGrid.getBoundingClientRect().top < window.innerHeight - 80) {
                startCounters();
            }

            // Update Right-Side Pagination (01 - 07)
            const sections = ['sec-01', 'sec-02', 'sec-03', 'sec-04', 'sec-05', 'sec-06', 'sec-07'];
            let currentSec = 'sec-01';
            sections.forEach(secId => {
                const el = document.getElementById(secId);
                if (el && el.getBoundingClientRect().top <= window.innerHeight * 0.45) {
                    currentSec = secId;
                }
            });

            document.querySelectorAll('.side-dot-nav .nav-item').forEach(item => {
                if (item.dataset.section === currentSec) {
                    item.classList.add('active');
                } else {
                    item.classList.remove('active');
                }
            });
        }

        window.addEventListener('scroll', handleScrollEffects);
        window.addEventListener('DOMContentLoaded', () => {
            renderProjects('all');
            handleScrollEffects();
        });
    </script>
</body>
</html>
