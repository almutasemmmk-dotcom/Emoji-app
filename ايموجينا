<!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>أضخم مكتبة رموز Unicode ✨🪄</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Tajawal:wght@400;700&display=swap');
        
        /* تأثير الخلفية السحرية */
        body {
            font-family: 'Tajawal', sans-serif;
            background: radial-gradient(circle at center, #1a0033 0%, #0d0d26 50%, #000000 100%);
            color: #fff;
            padding: 20px;
            margin: 0;
            overflow: hidden; /* لمنع شريط التمرير */
            position: relative;
        }

        /* تأثيرات النجوم والجسيمات في الخلفية */
        body::before {
            content: '';
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: url("data:image/svg+xml,%3Csvg width='100%25' height='100%25' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='n' x='0' y='0'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.6' numOctaves='3' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23n)' opacity='0.05'/%3E%3C/svg%3E");
            animation: move-noise 20s infinite linear;
            z-index: -1;
            opacity: 0.2;
        }

        @keyframes move-noise {
            0% { transform: translate(0, 0); }
            100% { transform: translate(100px, 100px); }
        }

        h1 {
            text-align: center;
            color: #ff69b4;
            font-size: 2.8rem;
            margin-bottom: 20px;
            text-shadow: 0 0 15px #ff69b4, 0 0 25px #ff69b4;
            letter-spacing: 2px;
            animation: pulse-glow 3s infinite alternate;
        }

        @keyframes pulse-glow {
            0% { text-shadow: 0 0 15px #ff69b4, 0 0 25px #ff69b4; }
            100% { text-shadow: 0 0 25px #ff69b4, 0 0 40px #ff69b4; }
        }

        #search {
            display: block;
            width: 100%;
            padding: 18px;
            margin-bottom: 20px;
            border-radius: 16px;
            border: 2px solid #5a008a;
            font-size: 20px;
            outline: none;
            background: rgba(34, 1, 51, 0.5);
            color: #e0e0e0;
            box-shadow: 0 0 20px rgba(90, 0, 138, 0.5);
            transition: all 0.4s ease-in-out;
        }

        #search:focus {
            background: rgba(45, 2, 68, 0.7);
            border-color: #ff69b4;
            box-shadow: 0 0 30px #ff69b4, 0 0 50px #ff69b4;
        }

        .symbols-container {
            background: rgba(17, 1, 26, 0.7);
            padding: 25px;
            border-radius: 20px;
            border: 1px solid rgba(255, 255, 255, 0.1);
            max-height: 70vh;
            overflow-y: auto;
            backdrop-filter: blur(5px);
            -webkit-backdrop-filter: blur(5px);
            box-shadow: inset 0 0 50px rgba(255, 255, 255, 0.05), 0 0 40px rgba(0, 0, 0, 0.4);
        }
        
        .symbol-grid {
            display: flex;
            flex-wrap: wrap;
            gap: 12px;
        }

        .section-title {
            text-align: center;
            color: #ffed8d;
            font-size: 1.8rem;
            margin-top: 30px;
            margin-bottom: 10px;
            text-shadow: 0 0 10px #ffed8d;
            letter-spacing: 1px;
            animation: section-glow 2s infinite alternate;
        }

        @keyframes section-glow {
            0% { text-shadow: 0 0 5px #ffed8d; }
            100% { text-shadow: 0 0 15px #ffed8d; }
        }

        .symbol-item {
            cursor: pointer;
            padding: 8px 12px;
            border-radius: 12px;
            background: rgba(34, 1, 51, 0.6);
            border: 1px solid rgba(255, 255, 255, 0.1);
            transition: all 0.4s ease-in-out;
            font-size: 28px;
            user-select: none;
            position: relative;
            text-shadow: 0 0 8px rgba(255, 255, 255, 0.8);
            box-shadow: 0 0 10px rgba(255, 105, 180, 0.4);
            transform: translateZ(0);
        }

        /* تأثيرات خاصة بالرموز */
        .symbol-item.regular-symbol:hover {
            background: rgba(255, 105, 180, 0.3);
            transform: scale(1.3) rotate(5deg) translateZ(50px);
            text-shadow: 0 0 15px #ff69b4, 0 0 25px #ff69b4, 0 0 40px #ff69b4;
            box-shadow: 0 0 15px #ff69b4, 0 0 25px #ff69b4, 0 0 40px #ff69b4;
            z-index: 10;
        }

        /* تأثيرات خاصة بالإيموجي */
        .symbol-item.emoji-symbol:hover {
            transform: scale(1.1) rotate(0deg) translateZ(0px);
            box-shadow: 0 0 10px rgba(255, 105, 180, 0.4);
            animation: none;
        }
        
        .toast {
            position: fixed;
            bottom: 30px;
            left: 50%;
            transform: translateX(-50%);
            background-color: #ff69b4;
            color: #fff;
            padding: 12px 25px;
            border-radius: 12px;
            opacity: 0;
            transition: opacity 0.5s ease-in-out, transform 0.5s ease-in-out;
            z-index: 100;
            font-weight: bold;
            box-shadow: 0 4px 20px rgba(255, 105, 180, 0.4);
        }

        /* تأثير وهج عند الضغط */
        .symbol-item.flash {
            animation: click-flash 0.3s ease-out forwards;
        }

        @keyframes click-flash {
            0% {
                transform: scale(1);
                box-shadow: 0 0 15px #ffed8d, 0 0 30px #ffed8d, 0 0 60px #ffed8d;
            }
            100% {
                transform: scale(1.1);
                box-shadow: 0 0 5px rgba(255, 105, 180, 0.4);
            }
        }
    </style>
</head>
<body class="bg-gray-900">
    <h1 class="text-pink-400 font-bold text-center">أضخم مكتبة رموز Unicode ✨🪄</h1>
    <input type="text" id="search" placeholder="ابحث عن أي رمز..." class="w-full px-4 py-3 mb-4">
    
    <div class="symbols-container" id="mainContainer">
        <h2 class="section-title">الرموز التعبيرية (إيموجي) ✨</h2>
        <div class="symbol-grid" id="emojisContainer"></div>
        <h2 class="section-title">رموز أخرى 🗃️</h2>
        <div class="symbol-grid" id="symbolsContainer"></div>
    </div>
    
    <div id="toast" class="toast">تم نسخ الرمز!</div>

    <script>
    // نطاقات رموز تعبيرية (تم تعديلها لتكون أكثر دقة)
    const emojiRanges = [
        [0x1F600, 0x1F64F],    // Emoticons
        [0x1F300, 0x1F5FF],    // Miscellaneous Symbols and Pictographs
        [0x1F680, 0x1F6FF],    // Transport and Map Symbols
        [0x1F900, 0x1F9FF],    // Supplemental Symbols and Pictographs
        [0x1FA00, 0x1FA6F],    // Chess Symbols
        [0x1FA70, 0x1FAFF],    // Symbols and Pictographs Extended-A
        [0x2600, 0x27BF],      // Miscellaneous Symbols and Dingbats
    ];

    // نطاقات رموز عامة (تم تعديلها لتشمل النطاقات المخصصة في السابق)
    const symbolRanges = [
        [0x0020, 0x007E],      // Basic ASCII
        [0x00A0, 0x00FF],      // Latin-1 Supplement
        [0x0100, 0x017F],      // Latin Extended-A
        [0x0180, 0x024F],      // Latin Extended-B
        [0x0250, 0x02AF],      // IPA Extensions
        [0x0370, 0x03FF],      // Greek and Coptic
        [0x0400, 0x04FF],      // Cyrillic
        [0x0500, 0x052F],      // Cyrillic Supplement
        [0x0530, 0x058F],      // Armenian
        [0x0600, 0x06FF],      // Arabic
        [0x0900, 0x097F],      // Devanagari
        [0x1B00, 0x1B7F],      // Batak
        [0x2000, 0x206F],      // General Punctuation
        [0x2070, 0x209F],      // Superscripts and Subscripts
        [0x20A0, 0x20CF],      // Currency Symbols
        [0x2100, 0x214F],      // Letterlike Symbols
        [0x2150, 0x218F],      // Number Forms
        [0x2500, 0x257F],      // Box Drawing
        [0x2580, 0x259F],      // Block Elements
        [0x25A0, 0x25FF],      // Geometric Shapes
        [0x2900, 0x297F],      // Supplemental Arrows-A
        [0x2A00, 0x2AFF],      // Supplemental Mathematical Operators
        [0x2B00, 0x2BFF],      // Miscellaneous Symbols and Arrows
        [0x3000, 0x303F],      // CJK Symbols and Punctuation
        [0x3200, 0x32FF],      // Enclosed CJK Letters and Months
        [0x4E00, 0x9FFF],      // CJK Unified Ideographs
        [0xFB00, 0xFB4F],      // Alphabetic Presentation Forms
        [0xFF00, 0xFFEF],      // Halfwidth and Fullwidth Forms
        [0x10000, 0x1007F],    // Linear B Syllabary
        [0x12000, 0x123FF],    // Cuneiform
        [0x1D400, 0x1D7FF],    // Mathematical Alphanumeric Symbols
    ];

    // إضافة رموز زخارف ونصوص خاصة
    const specialSymbols = [
        "˚ʚ♡ɞ˚", "𓅓", "｡ﾟﾟ･｡･ﾟﾟ｡", "🍙", "💖", "💘", "💓", "💞", "💔",
        "❥", "❦", "❧", "✨", "🎀", "🦉", "🦌", "🐼", "🐍", "🌹", "💗", "💝",
        "ᡣ𐭩", "𐙚₊˚⊹♡", "ᝰ.ᥫ᭡。", "🪞🕊️", "☁️", "⚘", "🍭", "🧸",
        "˚₊ · ͟͟͞͞➳❥", "⸜❤︎⸝‍", "⁺₊✧❤︎✧₊⁺", "꧁༺♡mylife♡༻꧂",
        "٩(♡ε♡ )۶", "ʕ ´•̥̥̥ ᴥ•̥̥̥`ʔ", "︵‿︵‿୨♡୧‿︵‿︵",
        "🎧💿", "🪐", "🌌", "🌟", "💫", "🕊️", "🗝️", "⚡", "🔥", "❄️"
    ];

    // دالة لعرض رسالة النسخ
    function showToast() {
        const toast = document.getElementById('toast');
        toast.style.opacity = '1';
        setTimeout(() => {
            toast.style.opacity = '0';
        }, 2000);
    }

    // دالة للتحقق مما إذا كان الرمز رمزًا تعبيريًا (إيموجي)
    function isEmoji(char) {
        const codePoint = char.codePointAt(0);
        return emojiRanges.some(range => codePoint >= range[0] && codePoint <= range[1]) || specialSymbols.includes(char);
    }

    // دالة لتحميل جميع الرموز
    function loadAllSymbols() {
        const emojisContainer = document.getElementById("emojisContainer");
        const symbolsContainer = document.getElementById("symbolsContainer");
        const allSymbols = [];

        // جمع جميع الرموز
        [...emojiRanges, ...symbolRanges].forEach(range => {
            const [start, end] = range;
            for (let i = start; i <= end; i++) {
                try {
                    allSymbols.push(String.fromCodePoint(i));
                } catch (e) {
                    continue;
                }
            }
        });
        
        // إضافة الرموز الخاصة
        allSymbols.push(...specialSymbols);

        // فرز الرموز إلى إيموجي ورموز أخرى
        allSymbols.forEach(sym => {
            const span = document.createElement("span");
            span.textContent = sym;
            span.onclick = () => {
                const tempInput = document.createElement("textarea");
                tempInput.value = sym;
                document.body.appendChild(tempInput);
                tempInput.select();
                try {
                    const successful = document.execCommand('copy');
                    if (successful) {
                        showToast();
                        // تطبيق تأثير الوهج
                        span.classList.add('flash');
                        setTimeout(() => {
                            span.classList.remove('flash');
                        }, 300);
                    } else {
                        console.error("فشل في نسخ الرمز باستخدام execCommand");
                    }
                } catch (err) {
                    console.error("فشل في نسخ الرمز:", err);
                } finally {
                    document.body.removeChild(tempInput);
                }
            };
            if (isEmoji(sym)) {
                span.className = "symbol-item emoji-symbol";
                emojisContainer.appendChild(span);
            } else {
                span.className = "symbol-item regular-symbol";
                symbolsContainer.appendChild(span);
            }
        });
    }

    // تحميل الرموز عند فتح الصفحة
    window.onload = loadAllSymbols;

    // البحث المباشر
    document.getElementById("search").addEventListener("input", e=>{
        const val = e.target.value;
        const allSymbolItems = document.querySelectorAll(".symbol-item");
        allSymbolItems.forEach(span=>{
            span.style.display = span.textContent.includes(val)?"inline-block":"none";
        });
    });
    </script>
</body>
</html>
