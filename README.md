# eid-ilfter
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>عيد سعيد يا ميار ❤️</title>
    <link href="https://fonts.googleapis.com/css2?family=Tajawal:wght@400;700&family=Amiri:ital,wght@0,700;1,700&display=swap" rel="stylesheet">
    <style>
        :root {
            --gold: #D4AF37;
            --dark-gold: #b8860b;
            --soft-white: #fffcf5;
            --heart-red: #ff4d6d;
        }

        body {
            margin: 0;
            /* تم تغيير نوع الخط هنا إلى Tajawal */
            font-family: 'Tajawal', sans-serif;
            /* تم تغيير لون الخلفية لدرجة رومانسية ناعمة */
            background: linear-gradient(135deg, #fff5f5 0%, #f3e5f5 100%);
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            overflow-x: hidden;
        }

        /* تأثير النجوم في الخلفية */
        .stars {
            position: fixed;
            top: 0; left: 0; width: 100%; height: 100%;
            pointer-events: none;
            background: radial-gradient(circle, rgba(212, 175, 55, 0.1) 1px, transparent 1px);
            background-size: 30px 30px;
            z-index: 0;
        }

        .container {
            width: 90%;
            max-width: 450px;
            background: white;
            border-radius: 25px;
            box-shadow: 0 15px 35px rgba(0,0,0,0.1);
            padding: 30px;
            text-align: center;
            position: relative;
            z-index: 1;
            min-height: 500px;
            display: flex;
            flex-direction: column;
            justify-content: center;
            border: 2px solid var(--gold);
        }

        .screen { display: none; animation: fadeIn 0.8s ease-in-out; }
        .active { display: block; }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }

        h1, h2 { font-family: 'Amiri', serif; color: var(--gold); }
        p { line-height: 1.8; color: #444; font-size: 1.1rem; }

        input {
            width: 80%; padding: 12px; border-radius: 25px;
            border: 1px solid var(--gold); outline: none; margin: 15px 0;
            text-align: center; font-size: 1.1rem;
            /* التأكد من استخدام الخط الجديد داخل الـ input */
            font-family: 'Tajawal', sans-serif;
        }

        .btn {
            background: var(--gold); color: white; border: none;
            padding: 12px 30px; border-radius: 25px; cursor: pointer;
            font-size: 1.1rem; transition: 0.3s; margin-top: 15px;
            /* التأكد من استخدام الخط الجديد داخل الزر */
            font-family: 'Tajawal', sans-serif;
            font-weight: bold;
        }
        .btn:hover { background: var(--dark-gold); transform: scale(1.05); }

        /* العداد */
        .timer-box { display: grid; grid-template-columns: repeat(2, 1fr); gap: 10px; margin: 20px 0; }
        .time-unit { background: var(--soft-white); padding: 10px; border-radius: 10px; border: 1px solid var(--gold); }
        .time-unit span { display: block; font-weight: bold; font-size: 1.2rem; color: var(--dark-gold); }

        /* الخط الزمني */
        .timeline { text-align: right; margin: 20px 0; border-right: 2px solid var(--gold); padding-right: 15px; }
        .event { margin-bottom: 20px; position: relative; }
        .event::after { content: '✨'; position: absolute; right: -25px; top: 0; background: white; }
        .event-date { font-weight: bold; color: var(--dark-gold); font-size: 0.9rem; }

        /* فيديو وصور */
        .media-container { margin-top: 20px; }
        .media-container iframe { width: 100%; border-radius: 15px; margin-bottom: 15px; }
        .photo-grid { display: flex; gap: 10px; overflow-x: auto; padding-bottom: 10px; }
        .photo-grid img { width: 150px; height: 150px; object-fit: cover; border-radius: 10px; border: 2px solid var(--gold); }

        .crescent { font-size: 5rem; color: var(--gold); cursor: pointer; animation: pulse 2s infinite; }
        @keyframes pulse { 0% { transform: scale(1); } 50% { transform: scale(1.1); } 100% { transform: scale(1); } }
    </style>
</head>
<body>

<div class="stars"></div>

<div class="container">
    
    <div class="screen active" id="screen1">
        <h1>عيد سعيد ✨</h1>
        <p>اكتبي الباسورد يا أغلى حد في دنيتي</p>
        <input type="password" id="pass" placeholder="Password">
        <button class="btn" onclick="checkPass()">فتح الرسالة</button>
    </div>

    <div class="screen" id="screen2">
        <div class="crescent" onclick="nextScreen(3)">🌙</div>
        <p>دوسـي على الهلال عشان تشوفي عديتك..</p>
    </div>

    <div class="screen" id="screen3">
        <h2>رسالة من القلب ❤️</h2>
        <div style="text-align: right; font-size: 0.95rem;">
            <p>
                انا بعملك الويب سايت دي وعارف انك مستنيها مني وع يقين اني هبعتهالك خلاص بقي برمجتي اتعرفت 😔😂<br><br>
                بس عمتا بكون مبسوط وانا ببسطك بحاجه زي دي واول حاجه انا سبحان الله انه خليكي تتغيري فجاه كد وتبقي كويسه ودي حاجه بسطاني اوي والعيد م هدخله م معاكي لا بعكس هيكون معاكي وانا مبسوط اني داخله معاكي ينور عيني وان شاء الله م اول وم اخر عيد واحنا مع بعض وان شاء الله هيجي العيد الي هتبقي فيه في بيتي... 
                <br><b>(اضغطي Next لتكملة الرسالة)</b>
            </p>
        </div>
        <button class="btn" onclick="nextScreen(4)">Next</button>
    </div>

    <div class="screen" id="screen4">
        <div style="text-align: right; font-size: 0.95rem;">
            <p>
                ان شاء الله علشان شوفت منك خطوه انك عايزه تصلحي كل حاجه بينا عمري خلاص ما هتخلي عنك وانتي رجعلتي ليا امل انك تكوني مراتي لان الصراحه م هكدب عليكي كنت فقدته.<br><br>
                بس حاليا املي رجع فيكي تاني وشايف بنتي الي حبيتها والي ربيتها رجعت وان شاء الله هتكون احسن من الاول ويرب يميار مهما يحصل مشاكل بينا تتحل وسيطنا ومحدش يشتمت فينا في يوم ولا سنين عمرنا تضيع ع الارض ويكتبلي معاكي كل خير وتكوني من نصيبي وام عيالي ي اجمل ام رهف 🫶🏻🫀<br><br>
                بحبك وبعشقك والله ي بنتي وحبيبتي وكل ما ليا 🫂🫶🏻🌍
            </p>
        </div>
        <button class="btn" onclick="nextScreen(5)">ذكرياتنا 🎞️</button>
    </div>

    <div class="screen" id="screen5">
        <h2>أغنيتنا وذكرياتنا ✨</h2>
        <div class="media-container">
            <iframe src="https://www.youtube.com/embed/_JtUGKTx2BA" frameborder="0" allowfullscreen></iframe>
            <div class="photo-grid">
    <img src="https://i.postimg.cc/Px0wvkGk/photo1.jpg" alt="Memory 1">
    <img src="https://i.postimg.cc/MTgQf8k6/photo2.jpg" alt="Memory 2">
    <img src="https://i.postimg.cc/50DCQMc9/photo3.jpg" alt="Memory 3">
          </div>
        </div>
        <button class="btn" onclick="nextScreen(6)">إحنا مع بعض من قد إيه؟</button>
    </div>

    <div class="screen" id="screen6">
        <h2>Love Timer ❤️</h2>
        <div class="timer-box">
            <div class="time-unit"><span id="days">0</span> يوم</div>
            <div class="time-unit"><span id="hours">0</span> ساعة</div>
            <div class="time-unit"><span id="minutes">0</span> دقيقة</div>
            <div class="time-unit"><span id="seconds">0</span> ثانية</div>
        </div>
        <button class="btn" onclick="nextScreen(7)">قصتنا 📖</button>
    </div>

    <div class="screen" id="screen7">
        <h2>Our Story 📖</h2>
        <div class="timeline">
            <div class="event">
                <div class="event-date">١ / ١ / ٢٠٢٤</div>
                <div>أول مرة نتعرف ببعض وبحبنا 😂😂🫀</div>
            </div>
            <div class="event">
                <div class="event-date">٣٠ / ١١ / ٢٠٢٣</div>
                <div>اليوم الي جيتي عندي فيه البطاط وفضلنا اليوم كله مع بعض 😍🫀</div>
            </div>
            <div class="event">
                <div class="event-date">٦ / ٢ / ٢٠٢٤</div>
                <div>أول مرة أمسك فيها إيدك 🫶🏻🌍</div>
            </div>
        </div>
        <button class="btn" onclick="nextScreen(8)">أهم كلمة..</button>
    </div>

    <div class="screen" id="screen8">
        <h2>إلى الأبد.. ❤️</h2>
        <p style="font-style: italic;">
            "كل يوم معاكي كان هديه من ربنا ليا وهفضل طول عمري بحب وجودك في حياتي وهفضل علطول حبي ليكي في مكانه لوحده في قلبي وفي الاخر نهايه علاقتنا تكون في بيتي ان شاء الله ي نور عيني بحبك اوي ي ميار 🫶🏻🫂"
        </p>
        <div style="font-size: 3rem;">🫂❤️💍</div>
    </div>

</div>

<script>
    function nextScreen(screenId) {
        document.querySelectorAll('.screen').forEach(s => s.classList.remove('active'));
        document.getElementById('screen' + screenId).classList.add('active');
        if(screenId === 6) startTimer();
    }

    function checkPass() {
        const p = document.getElementById('pass').value;
        if(p === "112023") { // الباسوردتاريخ ارتبطنا
            nextScreen(2);
        } else {
            alert("اول مره نتعترف بي حبينا لبعض ");
        }
    }

    function startTimer() {
        const startDate = new Date("2022-10-13T00:00:00").getTime();
        setInterval(() => {
            const now = new Date().getTime();
            const diff = now - startDate;

            document.getElementById("days").innerText = Math.floor(diff / (1000 * 60 * 60 * 24));
            document.getElementById("hours").innerText = Math.floor((diff % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
            document.getElementById("minutes").innerText = Math.floor((diff % (1000 * 60 * 60)) / (1000 * 60));
            document.getElementById("seconds").innerText = Math.floor((diff % (1000 * 60)) / 1000);
        }, 1000);
    }
</script>

</body>
</html>
