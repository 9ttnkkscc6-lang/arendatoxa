<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Arenda Toxa</title>

<style>
* {
    box-sizing: border-box;
}

body {
    margin: 0;
    font-family: Arial, sans-serif;
    background: #09090d;
    color: white;
}

.app {
    max-width: 500px;
    margin: auto;
    padding: 18px;
    padding-bottom: 90px;
}

.header {
    text-align: center;
    padding: 20px 0;
}

.logo {
    font-size: 30px;
    font-weight: 800;
}

.logo span {
    color: #8b5cf6;
}

.subtitle {
    color: #999;
    margin-top: 5px;
}

.card {
    background: #15151d;
    border-radius: 22px;
    padding: 20px;
    margin-top: 16px;
    border: 1px solid #242431;
}

.hero {
    text-align: center;
    padding: 30px 20px;
    background: linear-gradient(145deg, #201b2b, #111116);
}

.scooter {
    font-size: 75px;
}

h1, h2, h3 {
    margin-top: 0;
}

.button {
    width: 100%;
    border: none;
    border-radius: 15px;
    padding: 16px;
    margin-top: 12px;
    background: #8b5cf6;
    color: white;
    font-size: 17px;
    font-weight: bold;
    cursor: pointer;
}

.button:active {
    transform: scale(0.98);
}

.button.secondary {
    background: #272732;
}

.button.danger {
    background: #d93636;
}

.scooter-item {
    display: flex;
    align-items: center;
    justify-content: space-between;
    background: #20202a;
    padding: 15px;
    border-radius: 15px;
    margin-top: 10px;
}

.scooter-info {
    display: flex;
    align-items: center;
    gap: 12px;
}

.scooter-icon {
    font-size: 35px;
}

.status {
    color: #55d66f;
    font-size: 13px;
    margin-top: 4px;
}

.tariff {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background: #20202a;
    padding: 15px;
    border-radius: 14px;
    margin-top: 10px;
}

.price {
    font-weight: bold;
    color: #b794ff;
}

.hidden {
    display: none;
}

select {
    width: 100%;
    padding: 15px;
    border-radius: 14px;
    border: 1px solid #353542;
    background: #20202a;
    color: white;
    font-size: 16px;
    margin-top: 10px;
}

.timer {
    text-align: center;
    font-size: 48px;
    font-weight: bold;
    color: #b794ff;
    margin: 20px 0;
}

.bottom {
    position: fixed;
    bottom: 0;
    left: 0;
    right: 0;
    background: #111117;
    border-top: 1px solid #292934;
    padding: 12px;
    text-align: center;
}

.bottom button {
    background: none;
    border: none;
    color: #aaa;
    font-size: 13px;
    margin: 0 14px;
}

.bottom button.active {
    color: #b794ff;
}

.notice {
    color: #aaa;
    font-size: 13px;
    line-height: 1.5;
}
</style>
</head>

<body>

<div class="app">

    <!-- ГЛАВНАЯ -->

    <div id="home">

        <div class="header">
            <div class="logo">🛴 <span>Arenda</span> Toxa</div>
            <div class="subtitle">Аренда электросамокатов</div>
        </div>

        <div class="card hero">

            <div class="scooter">🛴</div>

            <h1>Арендуй самокат</h1>

            <p style="color:#aaa;">
                Быстро • Просто • Удобно
            </p>

            <button class="button" onclick="showRent()">
                🛴 АРЕНДОВАТЬ
            </button>

        </div>

        <div class="card">

            <h2>🛴 Свободные самокаты</h2>

            <div class="scooter-item">

                <div class="scooter-info">
                    <div class="scooter-icon">🛴</div>

                    <div>
                        <b>TOXA #001</b>
                        <div class="status">● Свободен</div>
                    </div>
                </div>

            </div>

            <div class="scooter-item">

                <div class="scooter-info">
                    <div class="scooter-icon">🛴</div>

                    <div>
                        <b>TOXA #002</b>
                        <div class="status">● Свободен</div>
                    </div>
                </div>

            </div>

            <div class="scooter-item">

                <div class="scooter-info">
                    <div class="scooter-icon">🛴</div>

                    <div>
                        <b>TOXA #003</b>
                        <div style="color:#ffb347;font-size:13px;">
                            ● В аренде
                        </div>
                    </div>
                </div>

            </div>

        </div>

        <div class="card">

            <h2>💰 Тарифы</h2>

            <div class="tariff">
                <span>30 минут</span>
                <span class="price">300 ₽</span>
            </div>

            <div class="tariff">
                <span>60 минут</span>
                <span class="price">500 ₽</span>
            </div>

            <div class="tariff">
                <span>120 минут</span>
                <span class="price">800 ₽</span>
            </div>

            <div class="tariff">
                <span>180 минут</span>
                <span class="price">1000 ₽</span>
            </div>

        </div>

        <div class="card">

            <h2>📜 Условия</h2>

            <div class="notice">
                • Используйте самокат аккуратно<br>
                • Соблюдайте ПДД и местные правила<br>
                • Используйте защитный шлем<br>
                • Соблюдайте возрастные требования,
                установленные местными правилами и условиями аренды<br>
                • Возвращайте самокат в согласованное место
            </div>

        </div>

    </div>


    <!-- АРЕНДА -->

    <div id="rent" class="hidden">

        <div class="header">

            <div class="logo">🛴 Выбор аренды</div>

            <div class="subtitle">
                Arenda Toxa
            </div>

        </div>

        <div class="card">

            <h2>1️⃣ Выберите самокат</h2>

            <select id="scooterSelect">

                <option value="TOXA #001">
                    🛴 TOXA #001 — свободен
                </option>

                <option value="TOXA #002">
                    🛴 TOXA #002 — свободен
                </option>

            </select>

        </div>

        <div class="card">

            <h2>2️⃣ Время аренды</h2>

            <select id="timeSelect">

                <option value="30">30 минут — 300 ₽</option>

                <option value="60">60 минут — 500 ₽</option>

                <option value="120">120 минут — 800 ₽</option>

                <option value="180">180 минут — 1000 ₽</option>

            </select>

        </div>

        <div class="card">

            <h2>3️⃣ Подтверждение</h2>

            <p id="summary" style="color:#aaa;">
                TOXA #001 • 30 минут • 300 ₽
            </p>

            <button class="button" onclick="startRental()">
                ✅ Начать аренду
            </button>

            <button class="button secondary" onclick="showHome()">
                ← Назад
            </button>

        </div>

    </div>


    <!-- АКТИВНАЯ АРЕНДА -->

    <div id="active" class="hidden">

        <div class="header">

            <div class="logo">🛴 Аренда активна</div>

        </div>

        <div class="card" style="text-align:center;">

            <div style="font-size:65px;">🛴</div>

            <h2 id="activeScooter">
                TOXA #001
            </h2>

            <div class="timer" id="timer">
                30:00
            </div>

            <p style="color:#aaa;">
                Время аренды
            </p>

            <button class="button danger" onclick="finishRental()">
                ⛔ Завершить аренду
            </button>

        </div>

        <div class="card">

            <h3>📍 Возврат</h3>

            <p class="notice">
                После завершения аренды оставьте самокат
                в согласованном месте возврата.
            </p>

        </div>

    </div>


    <!-- ПОДДЕРЖКА -->

    <div id="support" class="hidden">

        <div class="header">

            <div class="logo">📞 Поддержка</div>

        </div>

        <div class="card">

            <h2>Нужна помощь?</h2>

            <p class="notice">
                Если возникла проблема с арендой,
                обратитесь в Telegram.
            </p>

            <a
                href="https://t.me/Arendatoxa_bot"
                style="text-decoration:none;"
            >

                <button class="button">
                    💬 Написать в Telegram
                </button>

            </a>

        </div>

    </div>

</div>


<!-- НИЖНЕЕ МЕНЮ -->

<div class="bottom">

    <button onclick="showHome()">
        🏠<br>Главная
    </button>

    <button onclick="showRent()">
        🛴<br>Аренда
    </button>

    <button onclick="showSupport()">
        📞<br>Поддержка
    </button>

</div>


<script>

/* Telegram Mini App */

if (window.Telegram && Telegram.WebApp) {

    Telegram.WebApp.ready();

    Telegram.WebApp.expand();

}


/* Экраны */

function hideAll() {

    document.getElementById("home")
        .classList.add("hidden");

    document.getElementById("rent")
        .classList.add("hidden");

    document.getElementById("active")
        .classList.add("hidden");

    document.getElementById("support")
        .classList.add("hidden");

}


function showHome() {

    hideAll();

    document.getElementById("home")
        .classList.remove("hidden");

}


function showRent() {

    hideAll();

    document.getElementById("rent")
        .classList.remove("hidden");

    updateSummary();

}


function showSupport() {

    hideAll();

    document.getElementById("support")
        .classList.remove("hidden");

}


/* Обновление заказа */

document.getElementById("scooterSelect")
    .addEventListener("change", updateSummary);

document.getElementById("timeSelect")
    .addEventListener("change", updateSummary);


function getPrice(time) {

    if (time == 30) return 300;

    if (time == 60) return 500;

    if (time == 120) return 800;

    if (time == 180) return 1000;

}


function updateSummary() {

    let scooter =
        document.getElementById("scooterSelect").value;

    let time =
        document.getElementById("timeSelect").value;

    let price =
        getPrice(time);

    document.getElementById("summary").innerText =
        scooter + " • " +
        time + " минут • " +
        price + " ₽";

}


/* Таймер */

let timerInterval;

let remainingSeconds = 0;


function startRental() {

    let scooter =
        document.getElementById("scooterSelect").value;

    let time =
        parseInt(
            document.getElementById("timeSelect").value
        );

    remainingSeconds = time * 60;

    document.getElementById("activeScooter")
        .innerText = scooter;

    hideAll();

    document.getElementById("active")
        .classList.remove("hidden");

    updateTimer();

    clearInterval(timerInterval);

    timerInterval =
        setInterval(function() {

            remainingSeconds--;

            updateTimer();

            if (remainingSeconds <= 0) {

                clearInterval(timerInterval);

                alert("⏰ Время аренды закончилось!");

            }

        }, 1000);

}


function updateTimer() {

    let minutes =
        Math.floor(remainingSeconds / 60);

    let seconds =
        remainingSeconds % 60;

    document.getElementById("timer")
        .innerText =
        String(minutes).padStart(2, "0")
        + ":" +
        String(seconds).padStart(2, "0");

}


function finishRental() {

    clearInterval(timerInterval);

    alert("Аренда завершена ✅");

    showHome();

}

</script>

</body>
</html>