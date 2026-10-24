<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Anamika Roy - Portfolio</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        body {
            background-color: #050505;
            color: #ffffff;
            font-family: 'Inter', sans-serif;
            background-image: 
                linear-gradient(45deg, rgba(255,255,255,0.02) 1px, transparent 1px),
                linear-gradient(-45deg, rgba(255,255,255,0.02) 1px, transparent 1px);
            background-size: 60px 60px;
            background-position: center center;
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 3rem 1rem;
        }

        .glass-card {
            position: relative;
            background: linear-gradient(135deg, rgba(255, 255, 255, 0.08) 0%, rgba(255, 255, 255, 0.01) 100%);
            backdrop-filter: blur(16px);
            -webkit-backdrop-filter: blur(16px);
            border: 1px solid rgba(255, 255, 255, 0.15);
            box-shadow: 
                0 4px 30px rgba(0, 0, 0, 0.5),
                inset 0 1px 0 rgba(255, 255, 255, 0.2);
            border-radius: 40px;
            overflow: hidden;
            z-index: 10;
        }

        /* Diagonal shine effect */
        .glass-card::before {
            content: '';
            position: absolute;
            top: 0; left: -100%;
            width: 50%; height: 100%;
            background: linear-gradient(to right, rgba(255,255,255,0) 0%, rgba(255,255,255,0.1) 50%, rgba(255,255,255,0) 100%);
            transform: skewX(-45deg);
            animation: shine 6s infinite;
        }

        @keyframes shine {
            0% { left: -100%; }
            20% { left: 200%; }
            100% { left: 200%; }
        }

        /* Subtle edge highlights */
        .sparkle {
            position: absolute;
            width: 4px; height: 4px;
            border-radius: 50%;
            background: white;
            box-shadow: 0 0 10px 2px rgba(255, 255, 255, 0.8);
        }
        
        .s1 { top: -2px; left: 20%; }
        .s2 { bottom: -2px; right: 30%; }

        a {
            transition: opacity 0.2s;
        }
        a:hover {
            opacity: 0.8;
        }
    </style>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600&display=swap" rel="stylesheet">
</head>
<body class="antialiased selection:bg-purple-500 selection:text-white">

    <div class="max-w-3xl w-full flex flex-col gap-8 relative z-10">
        
        <!-- Header Card -->
        <div class="glass-card p-10 text-center flex flex-col items-center">
            <div class="sparkle s1"></div>
            
            <p class="text-xs tracking-[0.3em] text-gray-400 mb-4">D E S I G N &nbsp; / &nbsp; C O D E &nbsp; / &nbsp; M O T I O N</p>
            
            <h1 class="text-4xl md:text-5xl font-semibold mb-6 tracking-tight">Anamika Roy</h1>
            
            <img src="https://readme-typing-svg.demolab.com?font=Inter&weight=400&size=18&duration=2800&pause=1800&color=A78BFA&center=true&vCenter=true&width=480&height=40&lines=Creative+technologist.;Interfaces+with+intention.;Details+that+make+a+difference." class="max-w-full mb-6" alt="Typing SVG" />
            
            <p class="text-gray-300 text-lg mb-8 leading-relaxed max-w-lg">
                I bring design and engineering together <br class="hidden md:block">
                to make the web feel a little more thoughtful.
            </p>
            
            <div class="flex gap-4 justify-center">
                <a href="mailto:anamikaroy1120@gmail.com"><img src="https://img.shields.io/badge/Email_%E2%86%97-18181B?style=for-the-badge&logo=gmail&logoColor=C4B5FD" alt="Email" class="rounded-md" /></a>
                <a href="https://instagram.com/___ana_211"><img src="https://img.shields.io/badge/Instagram_%E2%86%97-18181B?style=for-the-badge&logo=instagram&logoColor=C4B5FD" alt="Instagram" class="rounded-md" /></a>
                <a href="https://github.com/anamikaroy1120?tab=repositories"><img src="https://img.shields.io/badge/My_work_%E2%86%97-18181B?style=for-the-badge&logo=github&logoColor=C4B5FD" alt="Explore my work" class="rounded-md" /></a>
            </div>
        </div>

        <!-- Split Skills Card -->
        <div class="glass-card p-10">
            <div class="sparkle s2"></div>
            <div class="grid md:grid-cols-2 gap-10 md:gap-4 divide-y md:divide-y-0 md:divide-x divide-white/10">
                
                <div class="md:pr-8 pt-4 md:pt-0">
                    <h3 class="text-xl font-semibold text-purple-300 mb-3">The visual side</h3>
                    <p class="text-gray-400 text-sm leading-relaxed mb-4">
                        Responsive layouts. Clear hierarchy.<br>
                        Subtle motion that serves a purpose.
                    </p>
                    <p class="font-medium text-sm text-gray-200">React · Tailwind CSS · Three.js</p>
                </div>
                
                <div class="md:pl-8 pt-8 md:pt-0">
                    <h3 class="text-xl font-semibold text-purple-300 mb-3">The engineering side</h3>
                    <p class="text-gray-400 text-sm leading-relaxed mb-4">
                        Reusable components. Connected systems.<br>
                        Care in how everything fits together.
                    </p>
                    <p class="font-medium text-sm text-gray-200">TypeScript · Laravel · MySQL</p>
                </div>

            </div>
        </div>

        <!-- Toolkit & Footer Card -->
        <div class="glass-card p-10 text-center flex flex-col items-center">
            
            <p class="text-xs tracking-[0.2em] text-gray-400 mb-8">MY EVERYDAY TOOLKIT</p>
            
            <img src="https://skillicons.dev/icons?i=ts,js,react,redux,tailwind&theme=dark" class="mb-4 max-w-full" alt="Frontend Tools" />
            <img src="https://skillicons.dev/icons?i=threejs,vite,laravel,mysql,github&theme=dark" class="mb-10 max-w-full" alt="Backend & Other Tools" />
            
            <div class="w-24 h-px bg-white/20 mb-10"></div>
            
            <p class="text-lg text-gray-200 mb-6 font-light">Good ideas start with a conversation.</p>
            
            <a href="mailto:anamikaroy1120@gmail.com" class="inline-block px-8 py-3 mb-10 bg-white/5 border border-white/20 rounded-full hover:bg-white/10 transition-colors text-purple-300 font-medium tracking-wide shadow-[0_0_15px_rgba(167,139,250,0.2)]">
                Let’s talk ↗
            </a>
            
            <p class="text-[10px] tracking-[0.2em] text-gray-500">ANAMIKA ROY &nbsp; · &nbsp; CREATIVE TECHNOLOGIST</p>
        </div>

    </div>

</body>
</html>
