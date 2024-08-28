---
layout: home
title: "Reverse Engineering Android and Windows Malware"
description: "Reverse Engineering and Malware Analysis Blog"
author:
  name: "Urban Vidergar"
  avatar: "https://www.infosek.net/images1/Urban%20Vidergar.jpg"
  bio: "Malware Reverse Engineer"
  location: "Ljubljana, Slovenia"
  links:
    email: "mailto:farghly.mahmod66@gmail.com"
    twitter: "https://twitter.com/"
    linkedin: "https://www.linkedin.com/"
    github: "https://github.com/urban5"
author_profile: true
---

---

<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>test Page</title>
    <link rel="stylesheet" href="assets/css/main.css">
    <link rel="stylesheet" href="assets/css/custom.css">
    <link href="https://fonts.googleapis.com/css2?family=Open+Sans:wght@400;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css">
    <style>
        body {
            background-color: #2C2F33;
            color: #fff;
            font-family: 'Open Sans', sans-serif;
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 20px;
        }

        .container {
            max-width: 700px;
            width: 100%;
            margin-bottom: 20px;
        }

        .post-blog-card {
            display: flex;
            align-items: stretch;
            transition: transform 0.3s, box-shadow 0.3s;
            overflow: hidden;
            position: relative;
            border-radius: 8px;
            background: #ffffff;
            margin-bottom: 25px;
            text-decoration: none;
            color: black;
            border-bottom: 4px solid #007bff;
            box-shadow: none;
            height: 280px;
        }

        .post-blog-card:hover {
            transform: scale(1.05);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.15), 0 10px 20px rgba(0, 123, 255, 0.7);
            background-color: rgba(255, 255, 255, 0.85);
        }

        .windows-logo, .android-logo {
            position: absolute;
            top: 10px;
            right: 10px;
            width: 30px;
            height: 30px;
            z-index: 2;
        }

        .post-image-container {
            flex-shrink: 0;
            width: 220px;
            height: auto;
            overflow: hidden;
            position: relative;
        }

        .post-image-container::before {
            content: '';
            position: absolute;
            top: 0;
            right: 0;
            width: 100%;
            height: 100%;
            background: inherit;
            clip-path: polygon(0 0, 100% 0, 0% 100%, 0 100%);
            z-index: 1;
        }

        .post-image {
            width: 100%;
            height: 100%;
            object-fit: cover;
            position: relative;
            z-index: 0;
        }

        .post-description {
            padding: 1rem;
            flex: 1;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            position: relative;
        }

        .post-meta, .post-ribbon {
            position: relative;
        }

        .post-ribbon4 {
            position: absolute;
            top: 0;
            right: 0;
            background: DodgerBlue;
            color: white;
            padding: 0.3rem 0.6rem;
            font-size: 0.9rem;
            transform: rotate(45deg);
            transform-origin: 100% 0;
        }

        .post-description h1 {
            font-family: 'Open Sans', sans-serif;
            color: #333;
            font-weight: bold;
            font-size: 1.4rem;
            margin-bottom: 8px;
            border-bottom: 2px solid #007bff;
            padding-bottom: 0.3rem;
            margin-right: 40px; /* Ensure space for the logo */
        }

        .post-description p {
            color: #666;
            font-size: 0.9rem;
            margin-right: 40px; /* Ensure space for the logo */
        }

        .post-date, .post-time {
            color: #999;
            font-size: 0.8rem;
            white-space: nowrap;
        }

        .post-footer {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding-top: 0.5rem;
        }

        .post-footer .post-date {
            text-align: center;
            flex: 1;
        }

        .post-footer .post-time {
            text-align: right;
            flex: 1;
        }

        .post-footer i {
            margin-right: 5px;
        }

        .post-blog-card-android {
            border-bottom: 4px solid #3ddc84;
        }

        .post-blog-card-android:hover {
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.15), 0 10px 20px rgba(61, 220, 132, 0.7);
        }

        .post-description-android h1 {
            border-bottom: 2px solid #3ddc84;
            margin-right: 40px; /* Ensure space for the logo */
        }

        .post-description-android p {
            margin-right: 40px; /* Ensure space for the logo */
        }

        .post-ribbon4-android {
            background: #3ddc84;
        }

        @media (max-width: 768px) {
            .post-blog-card {
                flex-direction: column;
                height: auto;
            }

            .post-image-container {
                width: 100%;
                height: 150px;
            }

            .post-image {
                width: 100%;
                height: 100%;
            }

            .post-description {
                padding: 0.5rem;
            }

            .post-footer {
                flex-direction: column;
                align-items: flex-start;
            }

            .post-footer .post-date, .post-footer .post-time {
                text-align: left;
                flex: unset;
            }
        }
    </style>
</head>
<body>

    <div class="container">
        <div class="post-blog-card">
            <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/5f/Windows_logo_-_2012.svg/200px-Windows_logo_-_2012.svg.png" alt="Windows Logo" class="windows-logo" />
            <div class="post-meta">
                <div class="post-ribbon">
                    <span class="post-ribbon4"></span>
                </div>
            </div>
            <div class="post-image-container">
                <img src="https://i.imgur.com/HeKi1VH.png" alt="NoEscape Ransomware" class="post-image" />
            </div>
            <div class="post-description">
                <h1>Windows Malware API Resolving</h1>
                <p>Article currently in the process of writing.</p>
                <div class="post-footer">
                    <p class="post-date page__meta"><i class="fas fa-calendar-alt"></i> 10 May 2024</p>
                    <p class="post-time page__meta"><i class="fas fa-clock"></i> 26 minute read</p>
                </div>
            </div>
        </div>

        <div class="post-blog-card post-blog-card-android" onclick="window.location.href='/malware_analysis/2024-07-25-first-malware-analysis-post/'">

            <img src="https://cdn.freebiesupply.com/logos/large/2x/android-logo-png-transparent.png" alt="Android Logo" class="android-logo" />
            <div class="post-meta">
                <div class="post-ribbon">
                    <span class="post-ribbon4 post-ribbon4-android"></span>
                </div>
            </div>
            <div class="post-image-container">
                <img src="https://imgur.com/6b3DT3W.jpg" alt="Android Malware" class="post-image" />
            </div>
            <div class="post-description post-description-android">
                <h1>Attacking Android Malware with Frida</h1>
                <p>Frida for Malware Reverse Engineering</p>
                <div class="post-footer">
                    <p class="post-date page__meta"><i class="fas fa-calendar-alt"></i> 26 July 2024</p>
                    <p class="post-time page__meta"><i class="fas fa-clock"></i> 10 minute read</p>
                </div>
            </div>
        </div>
    </div>
</body>
</html>
