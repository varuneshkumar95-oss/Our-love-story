# Our-love-story
Sorry bby ❤️
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#090909">

<title>Our Little Love Story ❤️</title>

<!-- Google Fonts -->
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@400;500;600;700&family=Montserrat:wght@300;400;500;600&display=swap" rel="stylesheet">

<style>
/* =========================================================
   EDIT THESE COLORS IF YOU WANT
========================================================= */

:root {
    --bg: #080808;
    --soft-bg: #111010;
    --text: #fff8f8;
    --muted: #c7b8bb;
    --pink: #ff6f91;
    --rose: #ff9aae;
    --glass: rgba(255,255,255,0.08);
    --border: rgba(255,255,255,0.14);
}

/* =========================================================
   BASIC RESET
========================================================= */

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    background: var(--bg);
    color: var(--text);
    font-family: "Montserrat", sans-serif;
    overflow-x: hidden;
}

button {
    font-family: inherit;
}

section {
    position: relative;
}

/* =========================================================
   LOADING / OPEN SCREEN
========================================================= */

#opening {
    position: fixed;
    inset: 0;
    z-index: 9999;
    background:
        radial-gradient(circle at 50% 40%, rgba(255,80,120,.20), transparent 35%),
        #050505;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    padding: 25px;
    transition: opacity 1s ease, visibility 1s ease;
}

#opening.hide {
    opacity: 0;
    visibility: hidden;
    pointer-events: none;
}

.opening-content {
    max-width: 500px;
    animation: fadeUp 1.5s ease;
}

.small-text {
    color: var(--muted);
    letter-spacing: 4px;
    text-transform: uppercase;
    font-size: 11px;
    margin-bottom: 22px;
}

.opening-content h1 {
    font-family: "Cormorant Garamond", serif;
    font-size: clamp(50px, 14vw, 95px);
    font-weight: 500;
    line-height: .9;
    margin-bottom: 25px;
}

.opening-content h1 span {
    color: var(--rose);
    font-style: italic;
}

.opening-content p {
    color: var(--muted);
    font-size: 14px;
    line-height: 1.8;
    margin-bottom: 35px;
}

.open-btn {
    border: 1px solid rgba(255,255,255,.3);
    background: rgba(255,255,255,.07);
    color: white;
    padding: 15px 30px;
    border-radius: 50px;
    cursor: pointer;
    transition: .4s;
    backdrop-filter: blur(10px);
}

.open-btn:hover {
    background: var(--pink);
    border-color: var(--pink);
    transform: translateY(-3px);
}

/* =========================================================
   HERO
========================================================= */

.hero {
    min-height: 100svh;
    display: flex;
    align-items: flex-end;
    padding: 35px 22px;
    background:
        linear-gradient(to top, #080808 3%, transparent 55%),
        linear-gradient(to bottom, rgba(0,0,0,.15), rgba(0,0,0,.45)),
        url("https://images.unsplash.com/photo-1518199266791-5375a83190b7?auto=format&fit=crop&w=1400&q=85")
        center/cover no-repeat;
}

.hero-content {
    width: 100%;
    max-width: 650px;
    margin: auto auto 15px;
}

.hero-tag {
    color: #ffd8df;
    letter-spacing: 4px;
    font-size: 10px;
    text-transform: uppercase;
    margin-bottom: 14px;
}

.hero h1 {
    font-family: "Cormorant Garamond", serif;
    font-size: clamp(60px, 17vw, 130px);
    line-height: .82;
    font-weight: 500;
}

.hero h1 em {
    display: block;
    color: var(--rose);
}

.hero-subtitle {
    margin-top: 25px;
    color: #e8dfe1;
    font-size: 13px;
    line-height: 1.8;
    max-width: 390px;
}

.scroll {
    margin-top: 35px;
    font-size: 10px;
    letter-spacing: 3px;
    color: #bbaeb1;
}

/* =========================================================
   GENERAL SECTIONS
========================================================= */

.section {
    padding: 100px 22px;
    max-width: 900px;
    margin: auto;
}

.section-label {
    color: var(--pink);
    font-size: 10px;
    letter-spacing: 4px;
    text-transform: uppercase;
    margin-bottom: 15px;
}

.section-title {
    font-family: "Cormorant Garamond", serif;
    font-size: clamp(45px, 11vw, 80px);
    line-height: .95;
    font-weight: 500;
    margin-bottom: 30px;
}

.section-text {
    color: var(--muted);
    line-height: 1.9;
    font-size: 14px;
}

/* =========================================================
   LOVE COUNTER
========================================================= */

.counter-section {
    text-align: center;
    background:
        radial-gradient(circle at center, rgba(255,90,120,.12), transparent 45%);
}

.counter-grid {
    display: grid;
    grid-template-columns: repeat(2,1fr);
    gap: 10px;
    margin-top: 40px;
}

.counter-box {
    padding: 25px 10px;
    border: 1px solid var(--border);
    border-radius: 20px;
    background: var(--glass);
    backdrop-filter: blur(15px);
}

.counter-number {
    font-family: "Cormorant Garamond", serif;
    font-size: 45px;
    color: white;
}

.counter-label {
    color: var(--muted);
    font-size: 9px;
    letter-spacing: 2px;
    text-transform: uppercase;
}

/* =========================================================
   STORY TIMELINE
========================================================= */

.timeline {
    margin-top: 50px;
    border-left: 1px solid rgba(255,255,255,.15);
    padding-left: 25px;
}

.timeline-item {
    margin-bottom: 55px;
    position: relative;
}

.timeline-item::before {
    content: "♡";
    position: absolute;
    left: -39px;
    top: 0;
    color: var(--pink);
    background: var(--bg);
    padding: 4px;
}

.timeline-date {
    font-size: 10px;
    letter-spacing: 3px;
    color: var(--pink);
    text-transform: uppercase;
    margin-bottom: 10px;
}

.timeline-item h3 {
    font-family: "Cormorant Garamond", serif;
    font-size: 34px;
    font-weight: 500;
    margin-bottom: 8px;
}

.timeline-item p {
    color: var(--muted);
    font-size: 13px;
    line-height: 1.8;
}

/* =========================================================
   REASONS
========================================================= */

.reasons {
    display: grid;
    gap: 12px;
    margin-top: 40px;
}

.reason {
    padding: 25px;
    border-radius: 22px;
    background: linear-gradient(
        135deg,
        rgba(255,255,255,.08),
        rgba(255,255,255,.025)
    );
    border: 1px solid var(--border);
    transition: .4s;
}

.reason:hover {
    transform: translateY(-5px);
    border-color: rgba(255,110,145,.4);
}

.reason-number {
    color: var(--pink);
    font-size: 11px;
    letter-spacing: 2px;
    margin-bottom: 15px;
}

.reason h3 {
    font-family: "Cormorant Garamond", serif;
    font-size: 29px;
    font-weight: 500;
    margin-bottom: 7px;
}

.reason p {
    color: var(--muted);
    font-size: 12px;
    line-height: 1.7;
}

/* =========================================================
   PHOTO GALLERY
========================================================= */

.gallery {
    display: grid;
    grid-template-columns: repeat(2,1fr);
    gap: 8px;
    margin-top: 40px;
}

.gallery img {
    width: 100%;
    height: 250px;
    object-fit: cover;
    border-radius: 5px;
    cursor: pointer;
    transition: .5s;
}

.gallery img:nth-child(1) {
    grid-row: span 2;
    height: 508px;
}

.gallery img:hover {
    transform: scale(.98);
    filter: brightness(.8);
}

/* =========================================================
   LOVE LETTER
========================================================= */

.letter-box {
    margin-top: 40px;
    padding: 35px 25px;
    border: 1px solid var(--border);
    border-radius: 25px;
    background:
        linear-gradient(
            135deg,
            rgba(255,110,145,.08),
            rgba(255,255,255,.03)
        );
}

.letter-box p {
    font-family: "Cormorant Garamond", serif;
    font-size: 24px;
    line-height: 1.6;
    color: #f5e9eb;
}

/* =========================================================
   SECRET BUTTON
========================================================= */

.secret-area {
    text-align: center;
}

.secret-btn {
    background: transparent;
    color: white;
    border: 1px solid rgba(255,255,255,.25);
    padding: 15px 25px;
    border-radius: 50px;
    cursor: pointer;
    margin-top: 30px;
    transition: .4s;
}

.secret-btn:hover {
    background: var(--pink);
    border-color: var(--pink);
}

.secret-message {
    display: none;
    margin-top: 30px;
    animation: fadeUp 1s ease;
}

.secret-message.show {
    display: block;
}

.secret-message h2 {
    font-family: "Cormorant Garamond", serif;
    font-size: 55px;
    font-weight: 500;
    color: var(--rose);
}

.secret-message p {
    color: var(--muted);
    margin-top: 15px;
    line-height: 1.8;
}

/* =========================================================
   FOOTER
========================================================= */

footer {
    text-align: center;
    padding: 80px 20px 45px;
    color: #756b6e;
    font-size: 10px;
    letter-spacing: 2px;
}

footer span {
    color: var(--pink);
}

/* =========================================================
   HEART PARTICLES
========================================================= */

.heart {
    position: fixed;
    bottom: -30px;
    pointer-events: none;
    color: rgba(255,130,155,.7);
    animation: floatHeart linear forwards;
    z-index: 5;
}

@keyframes floatHeart {
    from {
        transform: translateY(0) rotate(0);
        opacity: 0;
    }

    15% {
        opacity: 1;
    }

    to {
        transform: translateY(-110vh) rotate(360deg);
        opacity: 0;
    }
}

@keyframes fadeUp {
    from {
        opacity: 0;
        transform: translateY(25px);
    }

    to {
        opacity: 1;
        transform: translateY(0);
    }
}

/* =========================================================
   IMAGE LIGHTBOX
========================================================= */

#lightbox {
    position: fixed;
    inset: 0;
    background: rgba(0,0,0,.95);
    display: none;
    align-items: center;
    justify-content: center;
    z-index: 10000;
    padding: 20px;
}

#lightbox img {
    max-width: 100%;
    max-height: 90vh;
    border-radius: 8px;
}

#closeLightbox {
    position: absolute;
    top: 20px;
    right: 25px;
    font-size: 35px;
    color: white;
    cursor: pointer;
}

/* =========================================================
   DESKTOP
========================================================= */

@media (min-width: 700px) {

    .counter-grid {
        grid-template-columns: repeat(4,1fr);
    }

    .reasons {
        grid-template-columns: repeat(2,1fr);
    }

    .gallery {
        grid-template-columns: repeat(3,1fr);
    }

    .gallery img,
    .gallery img:nth-child(1) {
        height: 350px;
        grid-row: auto;
    }

    .gallery img:nth-child(1) {
        grid-row: span 2;
        height: 708px;
    }
}
</style>
</head>

<body>

<!-- =========================================================
     OPENING SCREEN
========================================================= -->

<div id="opening">

    <div class="opening-content">

        <div class="small-text">
            A little something for you
        </div>

        <h1>
            Hey <span id="openingName">Beautiful</span>
        </h1>

        <p>
            Some things are too special to fit inside
            an ordinary message.
        </p>

        <button class="open-btn" onclick="openWebsite()">
            Open My Heart ❤️
        </button>

    </div>

</div>


<!-- =========================================================
     HERO
========================================================= -->

<section class="hero">

    <div class="hero-content">

        <div class="hero-tag">
            Our little story
        </div>

        <h1>
            You.
            <em>Me.</em>
            Always.
        </h1>

        <p class="hero-subtitle">
            In a world full of people,
            somehow I found my favorite one.
        </p>

        <div class="scroll">
            ↓ SCROLL TO OUR STORY
        </div>

    </div>

</section>


<!-- =========================================================
     COUNTER
========================================================= -->

<section class="section counter-section">

    <div class="section-label">
        Since the day we met
    </div>

    <h2 class="section-title">
        Time with you
    </h2>

    <p class="section-text">
        And somehow, every day still feels like
        the beginning.
    </p>

    <div class="counter-grid">

        <div class="counter-box">
            <div class="counter-number" id="years">0</div>
            <div class="counter-label">Years</div>
        </div>

        <div class="counter-box">
            <div class="counter-number" id="months">0</div>
            <div class="counter-label">Months</div>
        </div>

        <div class="counter-box">
            <div class="counter-number" id="days">0</div>
            <div class="counter-label">Days</div>
        </div>

        <div class="counter-box">
            <div class="counter-number" id="hours">0</div>
            <div class="counter-label">Hours</div>
        </div>

    </div>

</section>


<!-- =========================================================
     OUR STORY
========================================================= -->

<section class="section">

    <div class="section-label">
        Chapter One
    </div>

    <h2 class="section-title">
        Our Story
    </h2>

    <div class="timeline">

        <div class="timeline-item">

            <div class="timeline-date">
                The beginning
            </div>

            <h3>
                The day we met
            </h3>

            <p>
                I didn't know it at the time,
                but that ordinary day was about
                to become one of my favorite memories.
            </p>

        </div>


        <div class="timeline-item">

            <div class="timeline-date">
                Chapter Two
            </div>

            <h3>
                Our first conversation
            </h3>

            <p>
                One conversation turned into another,
                and somewhere between those moments,
                you became someone I wanted around.
            </p>

        </div>


        <div class="timeline-item">

            <div class="timeline-date">
                Chapter Three
            </div>

            <h3>
                The memories
            </h3>

            <p>
                The laughs, the stupid jokes,
                the late-night conversations,
                and every little moment in between.
            </p>

        </div>


        <div class="timeline-item">

            <div class="timeline-date">
                Today
            </div>

            <h3>
                Still choosing you.
            </h3>

            <p>
                And if I could go back and live
                everything again, I would still
                choose the same story.
            </p>

        </div>

    </div>

</section>


<!-- =========================================================
     REASONS
========================================================= -->

<section class="section">

    <div class="section-label">
        A few reasons
    </div>

    <h2 class="section-title">
        Why you?
    </h2>

    <div class="reasons">

        <div class="reason">

            <div class="reason-number">01</div>

            <h3>
                Your smile
            </h3>

            <p>
                Somehow it can turn even an ordinary
                moment into something beautiful.
            </p>

        </div>


        <div class="reason">

            <div class="reason-number">02</div>

            <h3>
                Your heart
            </h3>

            <p>
                The way you care, love and understand
                people is something I never want to lose.
            </p>

        </div>


        <div class="reason">

            <div class="reason-number">03</div>

            <h3>
                Your presence
            </h3>

            <p>
                I don't always need a plan.
                Sometimes having you around is enough.
            </p>

        </div>


        <div class="reason">

            <div class="reason-number">04</div>

            <h3>
                Simply you.
            </h3>

            <p>
                No complicated reason.
                You're just my favorite person.
            </p>

        </div>

    </div>

</section>


<!-- =========================================================
     PHOTO GALLERY
========================================================= -->

<section class="section">

    <div class="section-label">
        Our memories
    </div>

    <h2 class="section-title">
        Little moments.
    </h2>

    <p class="section-text">
        Replace these photos with your own favorite memories.
    </p>


    <div class="gallery">

        <!-- PHOTO 1 -->
        <img
            src="https://images.unsplash.com/photo-1516589178581-6cd7833ae3b2?auto=format&fit=crop&w=900&q=85"
            alt="Our memory"
        >

        <!-- PHOTO 2 -->
        <img
            src="https://images.unsplash.com/photo-1522673607200-164d1b6ce486?auto=format&fit=crop&w=900&q=85"
            alt="Our memory"
        >

        <!-- PHOTO 3 -->
        <img
            src="https://images.unsplash.com/photo-1518568814500-bf0f8d125f46?auto=format&fit=crop&w=900&q=85"
            alt="Our memory"
        >

        <!-- PHOTO 4 -->
        <img
            src="https://images.unsplash.com/photo-1494774157365-9e04c6720e47?auto=format&fit=crop&w=900&q=85"
            alt="Our memory"
        >

        <!-- PHOTO 5 -->
        <img
            src="https://images.unsplash.com/photo-1529333166437-7750a6dd5a70?auto=format&fit=crop&w=900&q=85"
            alt="Our memory"
        >

    </div>

</section>


<!-- =========================================================
     LOVE LETTER
========================================================= -->

<section class="section">

    <div class="section-label">
        From my heart
    </div>

    <h2 class="section-title">
        A letter for you.
    </h2>

    <div class="letter-box">

        <p>
            My love,
            <br><br>

            I don't know if words will ever be enough
            to explain what you mean to me.

            <br><br>

            But if there is one thing I want you to know,
            it is this:

            <br><br>

            I am grateful for every laugh,
            every conversation, every memory,
            and every little moment that brought us here.

            <br><br>

            You are one of the most beautiful chapters
            of my life.

            <br><br>

            And I hope this story keeps going...
            one day, one memory and one smile at a time.

            <br><br>

            Always yours. ❤️
        </p>

    </div>

</section>


<!-- =========================================================
     SECRET MESSAGE
========================================================= -->

<section class="section secret-area">

    <div class="section-label">
        One last thing
    </div>

    <h2 class="section-title">
        I have a secret.
    </h2>

    <button
        class="secret-btn"
        onclick="showSecret()"
    >
        Tap to reveal ❤️
    </button>
