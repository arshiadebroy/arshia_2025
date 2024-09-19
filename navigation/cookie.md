---
layout: page
title: Cookie Clicker
description: Cookie Clicker game
permalink: /cookieclicker/
---

{% include nav/home.html %}

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cookie Clicker</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="container">
        <h1>Cookie Clicker</h1>
        <div id="cookie" onclick="makeCookie()">
            🍪
        </div>
        <h2 id="cookieCount">Cookies: 0</h2>
        <button onclick="buyUpgrade()">Upgrade (Cost: 10 cookies)</button>
        <h3 id="upgradeCount">Upgrades: 0</h3>
    </div>
    <script src="script.js"></script>
</body>
</html>