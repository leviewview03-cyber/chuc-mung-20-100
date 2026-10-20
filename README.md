<audio id="bgMusic" loop preload="auto">
    <source src="https://www.youtube.com/watch?v=heMYSOZoT3c&list=RDheMYSOZoT3c&start_radio=1" type="audio/mpeg">
</audio>
<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gửi Quỳnh - 20/10 ✨</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Dancing+Script:wght@600;700&family=Quicksand:wght@400;500;600;700&family=Great+Vibes&display=swap" rel="stylesheet">
    <!-- FontAwesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Canvas Confetti -->
    <script src="https://cdn.jsdelivr.net/npm/canvas-confetti@1.6.0/dist/confetti.browser.min.js"></script>
    
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        roseGold: '#e0a96d',
                        deepRose: '#881337',
                        magicPink: '#ff4d6d',
                        pastelPurple: '#2e1065'
                    },
                    fontFamily: {
                        cursive: ['"Dancing Script"', 'cursive'],
                        luxury: ['"Great Vibes"', 'cursive'],
                        sans: ['"Quicksand"', 'sans-serif']
                    }
                }
            }
        }
    </script>

    <style>
        body {
            font-family: 'Quicksand', sans-serif;
            background: radial-gradient(circle at center, #2e1065 0%, #0f172a 100%);
            overflow-x: hidden;
            min-height: 100vh;
            color: #f8fafc;
        }

        /* Glassmorphism styling */
        .glass-card {
            background: rgba(35, 15, 55, 0.75);
            backdrop-filter: blur(20px);
            -webkit-backdrop-filter: blur(20px);
            border: 1px solid rgba(255, 182, 193, 0.25);
            box-shadow: 0 20px 50px rgba(0, 0, 0, 0.5), 0 0 30px rgba(255, 77, 109, 0.2);
        }

        .glass-modal {
            background: rgba(25, 10, 40, 0.95);
            backdrop-filter: blur(25px);
            border: 1px solid rgba(255, 182, 193, 0.4);
            box-shadow: 0 0 50px rgba(255, 77, 109, 0.4);
        }

        /* Glow effects */
        .glow-text-gold {
            text-shadow: 0 0 10px rgba(224, 169, 109, 0.6), 0 0 20px rgba(255, 215, 0, 0.4);
        }

        /* Gift Animation */
        @keyframes pulse-gift {
            0%, 100% { transform: scale(1); box-shadow: 0 0 25px rgba(255, 77, 109, 0.4); }
            50% { transform: scale(1.06); box-shadow: 0 0 45px rgba(255, 77, 109, 0.8); }
        }

        .animate-gift {
            animation: pulse-gift 2.2s infinite ease-in-out;
        }

        /* Typewriter Cursor */
        .typewriter-cursor::after {
            content: '|';
            animation: blink 0.8s infinite;
            color: #ff4d6d;
            font-weight: bold;
        }

        @keyframes blink {
            0%, 100% { opacity: 1; }
            50% { opacity: 0; }
        }

        /* Custom Scrollbar */
        ::-webkit-scrollbar {
            width: 5px;
        }
        ::-webkit-scrollbar-track {
            background: rgba(15, 23, 42, 0.6);
        }
        ::-webkit-scrollbar-thumb {
            background: rgba(255, 77, 109, 0.6);
            border-radius: 10px;
        }
    </style>
</head>
<body class="relative flex items-center justify-center p-4 sm:p-6 select-none overflow-x-hidden min-h-screen">

    <!-- Canvas for Floating Petals and Stars -->
    <canvas id="canvas" class="fixed inset-0 pointer-events-none z-10"></canvas>

    <!--
        ===================================================================
        🎵 FILE NHẠC NỀN MP3:
        Nhạc sẽ TỰ ĐỘNG PHÁT ngay khoảnh khắc Quỳnh nhấn nút "Mở Quà" ở trang đầu!
        Muốn đổi bài hát khác: Bạn đổi tên file ở `src="nhac-nen.mp3"` là xong.
        ===================================================================
    -->
    <audio id="bgMusic" loop preload="auto">
        <source src="nhac-nen.mp3" type="audio/mpeg">
        <source src="https://assets.mixkit.co/music/preview/mixkit-sweet-love-121.mp3" type="audio/mpeg">
    </audio>

    <!-- MAIN CONTAINER -->
    <main class="relative z-20 w-full max-w-lg mx-auto my-auto">

        <!-- ================= STAGE 1: MÀN HÌNH HỘP QUÀ ================= -->
        <section id="stage1" class="glass-card rounded-3xl p-6 sm:p-10 text-center transition-all duration-700 transform scale-100">
            <div class="relative inline-block mb-6">
                <div class="w-28 h-28 sm:w-32 sm:h-32 rounded-full bg-gradient-to-tr from-rose-900 via-purple-700 to-pink-500 flex items-center justify-center mx-auto animate-gift cursor-pointer shadow-2xl" onclick="openGift()">
                    <span class="text-5xl sm:text-6xl transform hover:scale-110 transition-transform">🎁</span>
                </div>
                <span class="absolute -bottom-2 left-1/2 -translate-x-1/2 px-3 py-0.5 bg-purple-950 border border-pink-500/50 rounded-full text-[10px] text-pink-300 uppercase tracking-widest whitespace-nowrap">
                    20 . 10 Special Message
                </span>
            </div>

            <h1 class="text-3xl sm:text-4xl font-bold font-luxury text-amber-200 glow-text-gold mb-2">
                Gửi Quỳnh ✨
            </h1>
            <p class="text-rose-200/80 text-sm sm:text-base mb-8 max-w-md mx-auto leading-relaxed">
                Một chút tâm sự nho nhỏ tui gửi tặng Quỳnh nhân ngày 20/10...
            </p>

            <button onclick="openGift()" class="w-full sm:w-auto px-8 py-3.5 bg-gradient-to-r from-rose-600 via-pink-600 to-purple-600 hover:from-rose-500 hover:to-purple-500 text-white font-bold rounded-2xl shadow-lg shadow-pink-900/50 hover:shadow-pink-600/50 transition-all duration-300 transform active:scale-95 flex items-center justify-center gap-3 mx-auto">
                <i class="fa-solid fa-envelope-open-text text-amber-300"></i>
                <span>Chạm Để Mở Thư 💕</span>
            </button>
        </section>

        <!-- ================= STAGE 2: BỨC THƯ ĐÁNH MÁY CHÍNH ================= -->
        <section id="stage2" class="hidden glass-card rounded-3xl p-6 sm:p-9 text-center transition-all duration-700 opacity-0 translate-y-8">
            <div class="mb-4">
                <span class="px-3 py-1 bg-purple-950 border border-pink-500/50 text-pink-300 text-xs font-semibold rounded-full uppercase tracking-widest">
                    20 . 10 . 2026 💌
                </span>
                <h2 class="text-3xl sm:text-4xl font-bold font-cursive text-amber-200 mt-2 glow-text-gold">
                    Gửi Quỳnh 💖
                </h2>
                <div class="w-20 h-0.5 bg-gradient-to-r from-transparent via-pink-500 to-transparent mx-auto mt-2"></div>
            </div>

            <!-- Letter Box with Typewriter Effect -->
            <div class="bg-black/40 p-5 sm:p-6 rounded-2xl border border-pink-500/30 text-left text-rose-100 text-sm sm:text-base leading-relaxed mb-6 shadow-inner min-h-[260px] max-h-[380px] overflow-y-auto">
                <p id="typewriterText" class="font-sans leading-7 sm:leading-8 text-pink-100 text-justify whitespace-pre-line"></p>
            </div>

            <!-- Final Interactive Button -->
            <div id="finalActionArea" class="hidden transition-all duration-500 opacity-0 transform scale-90">
                <button onclick="sendLoveToQuynh()" class="w-full py-3.5 px-6 bg-gradient-to-r from-pink-600 via-rose-500 to-amber-500 hover:from-pink-500 hover:to-amber-400 text-white font-bold rounded-2xl shadow-xl shadow-rose-900/60 hover:shadow-pink-500/50 transform active:scale-95 transition-all duration-300 flex items-center justify-center gap-3 text-sm sm:text-base">
                    <i class="fa-solid fa-heart text-amber-200 animate-pulse"></i>
                    <span>Tui Nhận Lời Chúc Này Nha! ✨</span>
                </button>
            </div>
        </section>

    </main>

    <!-- MODAL POPUP -->
    <div id="modalSuccess" class="fixed inset-0 bg-black/80 backdrop-blur-lg z-50 hidden items-center justify-center p-4">
        <div class="glass-modal rounded-3xl p-6 sm:p-8 max-w-sm w-full text-center border border-pink-400 transform scale-95 transition-all">
            <div class="text-5xl mb-3 animate-bounce">🥰✨</div>
            <h3 class="text-2xl font-bold font-cursive text-amber-200 mb-2">Cảm Ơn Quỳnh Rất Nhiều!</h3>
            <p class="text-sm text-pink-100 leading-relaxed mb-6">
                Chúc Quỳnh một ngày 20/10 thật nhiều niềm vui, luôn xinh đẹp và bình an nhé! 🌸
            </p>
            <button onclick="closeSuccessModal()" class="w-full py-3 bg-gradient-to-r from-pink-600 to-purple-600 text-white font-bold rounded-xl hover:from-pink-500 hover:to-purple-500 transition-all">
                Đóng Thư ✨
            </button>
        </div>
    </div>

    <!-- SCRIPT LOGIC -->
    <script>
        // Particle Background System (Petals & Stars)
        const canvas = document.getElementById('canvas');
        const ctx = canvas.getContext('2d');
        let width = canvas.width = window.innerWidth;
        let height = canvas.height = window.innerHeight;

        window.addEventListener('resize', () => {
            width = canvas.width = window.innerWidth;
            height = canvas.height = window.innerHeight;
        });

        class Particle {
            constructor() {
                this.reset();
            }

            reset() {
                this.x = Math.random() * width;
                this.y = -20;
                this.size = Math.random() * 10 + 6;
                this.speedY = Math.random() * 1.2 + 0.5;
                this.speedX = Math.random() * 0.8 - 0.4;
                this.rotation = Math.random() * 360;
                this.rotSpeed = Math.random() * 1.5 - 0.7;
                this.type = Math.random() > 0.4 ? 'petal' : 'sparkle';
                this.opacity = Math.random() * 0.7 + 0.3;
            }

            update() {
                this.y += this.speedY;
                this.x += Math.sin(this.y * 0.01) + this.speedX;
                this.rotation += this.rotSpeed;

                if (this.y > height + 20) {
                    this.reset();
                }
            }

            draw() {
                ctx.save();
                ctx.translate(this.x, this.y);
                ctx.rotate((this.rotation * Math.PI) / 180);
                ctx.globalAlpha = this.opacity;

                if (this.type === 'petal') {
                    ctx.fillStyle = '#ff4d6d';
                    ctx.beginPath();
                    ctx.moveTo(0, 0);
                    ctx.bezierCurveTo(-this.size / 2, -this.size / 2, -this.size, this.size / 3, 0, this.size);
                    ctx.bezierCurveTo(this.size, this.size / 3, this.size / 2, -this.size / 2, 0, 0);
                    ctx.fill();
                } else {
                    ctx.fillStyle = '#ffd700';
                    ctx.beginPath();
                    ctx.arc(0, 0, this.size / 3, 0, Math.PI * 2);
                    ctx.fill();
                }

                ctx.restore();
            }
        }

        const particles = Array.from({ length: 45 }, () => new Particle());

        function animateParticles() {
            ctx.clearRect(0, 0, width, height);
            particles.forEach(p => {
                p.update();
                p.draw();
            });
            requestAnimationFrame(animateParticles);
        }

        animateParticles();

        // Refined, natural Southern Vietnamese message
        const letterMessage = `Nay 20/10, ngày dành riêng cho phụ nữ, xin lỗi Quỳnh vì dạo này tui bận quá nên chưa kịp chuẩn bị món quà chỉn chu hơn cho bà. Dạo gần đây tụi mình cũng không trò chuyện hay gặp nhau nhiều.

Tình cảm tui dành cho Quỳnh mấy tháng qua, tui không biết bà cảm nhận thế nào hay có suy nghĩ gì không... Nhưng tui vẫn luôn mong người con gái tui để ý sẽ luôn vui vẻ, hạnh phúc và khỏe mạnh. 

Nhớ phải nghe lời tui dặn nè: ăn uống đầy đủ đúng giờ, đừng gồng gánh công việc nhiều quá nữa nha, kiệt sức rồi lại phải nhập viện nữa đó...

Gửi chút tình cảm của tui nhân ngày 20/10 đến Quỳnh, mong Quỳnh thông cảm cho sự chưa hoàn hảo lần này của tui nha. Tui nhất định sẽ bù cho bà vào những lần sau nếu có cơ hội...!`;

        // Direct Open Gift + Auto Play Music Action
        function openGift() {
            // Auto play music on interaction
            const bgMusic = document.getElementById('bgMusic');
            bgMusic.play().catch(e => console.log("Audio play blocked", e));

            const stage1 = document.getElementById('stage1');
            const stage2 = document.getElementById('stage2');

            stage1.classList.add('opacity-0', 'scale-90');
            setTimeout(() => {
                stage1.classList.add('hidden');
                stage2.classList.remove('hidden');
                setTimeout(() => {
                    stage2.classList.remove('opacity-0', 'translate-y-8');
                    stage2.classList.add('opacity-100', 'translate-y-0');
                    startTypewriter();
                }, 50);
            }, 400);
        }

        function startTypewriter() {
            const target = document.getElementById('typewriterText');
            target.classList.add('typewriter-cursor');
            let i = 0;
            target.innerText = '';

            function typeNextChar() {
                if (i < letterMessage.length) {
                    target.innerText += letterMessage.charAt(i);
                    i++;
                    setTimeout(typeNextChar, 30);
                } else {
                    target.classList.remove('typewriter-cursor');
                    showFinalActionButton();
                }
            }

            typeNextChar();
        }

        function showFinalActionButton() {
            const area = document.getElementById('finalActionArea');
            area.classList.remove('hidden');
            setTimeout(() => {
                area.classList.remove('opacity-0', 'scale-90');
                area.classList.add('opacity-100', 'scale-100');
            }, 100);
        }

        function sendLoveToQuynh() {
            // Confetti Fireworks
            confetti({
                particleCount: 120,
                spread: 80,
                origin: { y: 0.6 }
            });

            setTimeout(() => {
                confetti({
                    particleCount: 60,
                    angle: 60,
                    spread: 50,
                    origin: { x: 0 }
                });
                confetti({
                    particleCount: 60,
                    angle: 120,
                    spread: 50,
                    origin: { x: 1 }
                });
            }, 200);

            document.getElementById('modalSuccess').classList.remove('hidden');
            document.getElementById('modalSuccess').classList.add('flex');
        }

        function closeSuccessModal() {
            document.getElementById('modalSuccess').classList.add('hidden');
            document.getElementById('modalSuccess').classList.remove('flex');
        }
    </script>
</body>
</html>
