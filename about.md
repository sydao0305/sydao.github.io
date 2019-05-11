---
title: Team
layout: default
---

<style>
    .hero-section,
    .features-section,
    .quote-section,
    .blog-section {
        padding: 30px 0;
        border-radius: 2px;
    }

    .features-section * {
        box-sizing: border-box;
    }


    .features-section .feature-row {
        display: flex;
        justify-content: space-evenly;
        flex-wrap: wrap;
    }

    .features-section .feature-row .feature-card {
        background-color: #fff;
        /*width: 238.65px;*/
        width: calc(33.333% - 8px);
        margin-top: 16px;
        border-radius: 2px;
        box-shadow: 0 2px 2px 0 rgba(0, 0, 0, .14), 0 3px 1px -2px rgba(0, 0, 0, .2), 0 1px 5px 0 rgba(0, 0, 0, .12);
    }

    .features-section .feature-row .feature-card .image {
        background-color: rgb(43, 180, 201);
        background-size: cover;
        background-position: center;
        min-height: 4px;
    }

    .features-section .feature-row .feature-card .image.contain {
        background-size: contain
    }

    .features-section .feature-row .feature-card .text {
        padding: 32px 16px;
    }

    .features-section h5 {
        color: #111;
        font-size: 21px;
    }

    .features-section p {
        color: #828282;
        font-size: 90%;
        padding-top: 12px;
        margin-bottom: 0;
    }

    .features-section .feature-row .feature-card.portrait .image {
        height: 240px;
        background-color: #333;
        position: relative;
    }

    .features-section .feature-row .feature-card.portrait .image h5 {
        color: #f8f8f8;
        background-color: rgb(43, 180, 201);
        display: inline-block;
        padding: 0 8px;
        position: absolute;
        bottom: -24px;
    }

    .features-section .feature-row .feature-card.portrait .text {
        padding: 8px 16px 20px;
    }

    .features-section .feature-row .feature-card .button {
        padding: 16px 16px 32px;
    }

    @media only screen and (max-width: 700px) {
        .features-section .feature-row .feature-card {
            width: 48%;
        }
    }

    @media only screen and (max-width: 460px) {
        .features-section .feature-row .feature-card {
            width: 100%;
        }

        .features-section .feature-row .feature-card.portrait .image {
            background-size: cover;
            height: 320px;
        }
    }

    h2.section-title {
        font-weight: 300;
        text-transform: uppercase;
        text-align: center;
        color: #828282;
    }
</style>

<section class="features-section">
    <h2 class="section-title">Development Team</h2>
    <div class="features-wrapper">
        <div class="feature-row">
            <div class="feature-card portrait">
                <div class="image" style="background-image:url(/assets/img/thi.jpg)">
                    <h5>Thi</h5>
                </div>
                <div class="text">
                    <p>Architecture</p>
                </div>
            </div>
            <div class="feature-card portrait">
                <div class="image contain" style="background-image:url(/assets/img/huy.png)">
                    <h5>Huy</h5>
                </div>
                <div class="text">
                    <p>dApp & Libs</p>
                </div>
            </div>
            <div class="feature-card portrait">
                <div class="image contain" style="background-image:url(/assets/img/luong.png)">
                    <h5>Luong</h5>
                </div>
                <div class="text">
                    <p>Wallet</p>
                </div>
            </div>
        </div>
        <div class="feature-row">
            <div class="feature-card portrait">
                <div class="image" style="background-image:url('/assets/img/duc.jpg')">
                    <h5>Duc</h5>
                </div>
                <div class="text">
                    <p>Wasm & Rust</p>
                </div>
            </div>
            <div class="feature-card portrait">
                <div class="image" style="background-image:url(/assets/img/tin.jpg);background-position: top">
                    <h5>Tin</h5>
                </div>
                <div class="text">
                    <p>React</p>
                </div>
            </div>
            <div class="feature-card portrait">
                <div class="image" style="background-image:url(/assets/img/viet.jpg);background-position: top">
                    <h5>Viet</h5>
                </div>
                <div class="text">
                    <p>Can't describe him</p>
                </div>
            </div>
        </div>
        <div class="feature-row">
            <div class="feature-card portrait">
                <div class="image contain" style="background-image:url('/assets/img/duong.jpg')">
                    <h5>Duong</h5>
                </div>
                <div class="text">
                    <p>Transpiler & Tools</p>
                </div>
            </div>
            <div class="feature-card portrait">
                <div class="image" style="background-image:url(/assets/img/giang.jpg)">
                    <h5>Giang</h5>
                </div>
                <div class="text">
                    <p>UX</p>
                </div>
            </div>
            <div class="feature-card portrait">
                <div class="image" style="background-image:url(/assets/img/you.png)">
                    <h5>Join us</h5>
                </div>
                <div class="text">
                    <p>React Native</p>
                </div>
            </div>
        </div>
    </div>
</section>
