<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>King Cafe</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f2f2f2;
            margin: 0;
            padding: 0;
        }

        header {
            background-color: #333;
            color: white;
            padding: 20px;
            text-align: center;
        }

        nav {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            background-color: #444;
        }

        nav button {
            background-color: #444;
            color: white;
            border: none;
            padding: 15px 20px;
            cursor: pointer;
            font-size: 16px;
            flex: 1 1 auto;
            min-width: 120px;
        }

        nav button:hover,
        nav button.active {
            background-color: #666;
        }

        .section {
            display: none;
            padding: 20px;
            color: white;
            background-size: contain;
            background-position: center;
            background-repeat: no-repeat;
        }

        .active {
            display: block;
        }

        /* Section Colors + Hookah Icon */
        .section1 {
            background-color: #ff6f61;
            background-image: url('https://upload.wikimedia.org/wikipedia/commons/thumb/e/e3/Hookah_icon.svg/512px-Hookah_icon.svg.png');
            background-size: 150px;
            background-repeat: no-repeat;
            background-position: right bottom;
            opacity: 0.95;
        }

        .section2 { background-color: #6a5acd; }
        .section3 { background-color: #20b2aa; }
        .section4 { background-color: #ffb347; }
        .section5 { background-color: #3cb371; }
        .section6 { background-color: #ffa07a; }
        .section7 { background-color: #708090; }

        ul {
            list-style: none;
            padding: 0;
        }

        ul li {
            margin: 10px 0;
            font-size: 18px;
        }

        @media (max-width: 600px) {
            nav {
                flex-direction: column;
            }

            nav button {
                font-size: 18px;
                padding: 15px;
            }

            ul li {
                font-size: 16px;
            }

            .section {
                padding: 15px;
            }

            header {
                font-size: 20px;
                padding: 15px;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>King Cafe</h1>
    </header>

    <nav>
        <button onclick="showSection(0)" class="active">نێرگەلەکان</button>
        <button onclick="showSection(1)">خواردن</button>
        <button onclick="showSection(2)">Section 3</button>
        <button onclick="showSection(3)">Section 4</button>
        <button onclick="showSection(4)">Section 5</button>
        <button onclick="showSection(5)">Section 6</button>
        <button onclick="showSection(6)">Section 7</button>
    </nav>

    <div id="sections">
        <div class="section section1 active">
            <h2>تامەکان</h2>
            <ul>
                <li>King 1</li>
                <li>King 2</li>
                <li>King 3</li>
                <li>King 4</li>
                <li>King 5</li>
                <li>King 6</li>
                <li>King 7</li>
                <li>King 8</li>
                <li>King 9</li>
                <li>King 10</li>
                <li>King 11</li>
                <li>Dw Sew</li>
                <li>بنیشت</li>
                <li>بغدادی</li>
                <li>کاسترۆ</li>
                <li>لیمۆ</li>
            </ul>
        </div>

        <div class="section section2">
            <h2>خواردن</h2>
            <ul>
                <li>٤٠٠٠،٦٠٠٠،٨٠٠٠،١٠٠٠٠پیزا</li>
                <li>King 2</li>
                <li>King 3</li>
                <li>King 4</li>
                <li>King 5</li>
                <li>King 6</li>
                <li>King 7</li>
                <li>King 8</li>
                <li>King 9</li>
                <li>King 10</li>
                <li>King 11</li>
                <li>Dw Sew</li>
                <li>بنیشت</li>
                <li>بغدادی</li>
                <li>کاسترۆ</li>
                <li>لیمۆ</li>
            </ul>
        </div>

        <div class="section section3">
            <h2>Section 3</h2>
            <ul>
                <li>1</li>
                <li>2</li>
                <li>3</li>
                <li>4</li>
                <li>5</li>
                <li>6</li>
                <li>7</li>
                <li>8</li>
                <li>9</li>
            </ul>
        </div>

        <div class="section section4">
            <h2>Section 4</h2>
            <ul>
                <li>1</li>
                <li>2</li>
                <li>3</li>
                <li>4</li>
                <li>5</li>
                <li>6</li>
                <li>7</li>
                <li>8</li>
                <li>9</li>
            </ul>
        </div>

        <div class="section section5">
            <h2>Section 5</h2>
            <ul>
                <li>1</li>
                <li>2</li>
                <li>3</li>
                <li>4</li>
                <li>5</li>
                <li>6</li>
                <li>7</li>
                <li>8</li>
                <li>9</li>
            </ul>
        </div>

        <div class="section section6">
            <h2>Section 6</h2>
            <ul>
                <li>1</li>
                <li>2</li>
                <li>3</li>
                <li>4</li>
                <li>5</li>
                <li>6</li>
                <li>7</li>
                <li>8</li>
                <li>9</li>
            </ul>
        </div>

        <div class="section section7">
            <h2>Section 7</h2>
            <ul>
                <li>1</li>
                <li>2</li>
                <li>3</li>
                <li>4</li>
                <li>5</li>
                <li>6</li>
                <li>7</li>
                <li>8</li>
                <li>9</li>
            </ul>
        </div>
    </div>

    <script>
        function showSection(index) {
            const sections = document.querySelectorAll('.section');
            const buttons = document.querySelectorAll('nav button');

            sections.forEach((section, i) => {
                section.classList.toggle('active', i === index);
            });

            buttons.forEach((btn, i) => {
                btn.classList.toggle('active', i === index);
            });
        }
    </script>
</body>
</html>
