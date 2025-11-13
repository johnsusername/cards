# cards
<!DOCTYPE html>
<html lang="en">
<head>
    <style>
        #card-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 25px;
            max-width: 1200px;
            margin: 0 auto;
            padding-top: 20px;
        }
        .card {
            background-color: #ffffff;
            border-radius: 15px;
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
            overflow: hidden; /* Crucial to contain the hidden answer */
            position: relative;
            height: 200px; /* Fixed height for consistent look */
            cursor: pointer;
            border: 3px solid #007bff;
        }
        .card-front {
            padding: 20px;
            position: absolute;
            width: 100%;
            height: 100%;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            color: #007bff;
            font-size: 1.2em;
            font-weight: bold;
            background-color: #e6f0ff;
            transition: transform 0.6s ease-in-out, opacity 0.6s ease-in-out;
            z-index: 2;
        }
        .card-back {
            padding: 20px;
            position: absolute;
            width: 100%;
            height: 100%;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            color: #ffffff;
            background-color: #28a745;
            font-size: 1em;
            transform: translateY(100%) scale(0.8);
            opacity: 0;
            z-index: 1;
            transition: transform 0.6s ease-in-out, opacity 0.6s ease-in-out;
        }
        .card:hover .card-front {
            transform: translateY(-100%) scale(0.8);
            opacity: 0;
        }
        .card:hover .card-back {
            transform: translateY(0) scale(1);
            opacity: 1;
        }
        .card:hover {
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.2);
            transform: scale(1.02);
            transition: transform 0.3s ease;
        }
    </style>
</head>
<body>
    <div id="card-grid">
        <div class="card">
            <div class="card-front">What is the core structural language of web content?</div>
            <div class="card-back">HTML (HyperText Markup Language). It defines the structure of the page.</div>
        </div>
        <div class="card">
            <div class="card-front">What is used to control the presentation and styling of web pages?</div>
            <div class="card-back">CSS (Cascading Style Sheets). It handles colors, fonts, layout, and more.</div>
        </div>
        <div class="card">
            <div class="card-front">What language adds interactivity and dynamic behavior to a website?</div>
            <div class="card-back">JavaScript. It allows for complex features and updating content in real-time.</div>
        </div>
        <div class="card">
            <div class="card-front">What language adds interactivity and dynamic behavior to a website?</div>
            <div class="card-back">JavaScript. It allows for complex features and updating content in real-time.</div>
        </div>
        <div class="card">
            <div class="card-front">what is the term used when you win an acummulation prize amount</div>
            <div class="card-back">jack pot!!!</div>
        </div>
        <div class="card">
            <div class="card-front">What language adds interactivity and dynamic behavior to a website?</div>
            <div class="card-back">JavaScript. It allows for complex features and updating content in real-time.</div>
        </div>
        <div class="card">
            <div class="card-front">What language adds interactivity and dynamic behavior to a website?</div>
            <div class="card-back">JavaScript. It allows for complex features and updating content in real-time.</div>
        </div>
    </div>
</body>
</html>
