---
title: "Test"
order: 7
in_menu: true
---
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Citations - Pourquoi faire un mini-site ?</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, sans-serif;
            background-color: #f5f7fa;
            padding: 40px 20px;
            line-height: 1.6;
        }

        .container {
            max-width: 800px;
            margin: 0 auto;
        }

        .intro {
            text-align: center;
            margin-bottom: 50px;
        }

        .intro h1 {
            color: #2d3436;
            font-size: 32px;
            margin-bottom: 10px;
        }

        .intro p {
            color: #636e72;
            font-size: 18px;
        }

        .quotes-container {
            display: flex;
            flex-direction: column;
            gap: 25px;
        }

        .quote {
            padding: 25px 30px;
            border-radius: 20px;
            color: white;
            position: relative;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.08);
        }

        .quote:before {
            content: "“";
            position: absolute;
            top: 10px;
            left: 20px;
            font-size: 70px;
            font-family: Georgia, serif;
            opacity: 0.7;
        }

        .quote p {
            font-size: 20px;
            margin-left: 15px;
            position: relative;
            z-index: 1;
        }

        .quote-1 {
            background-color: #3498db;
        }

        .quote-2 {
            background-color: #2ecc71;
        }

        .quote-3 {
            background-color: #e84393;
        }

        /* Responsive */
        @media (max-width: 768px) {
            .intro h1 {
                font-size: 28px;
            }
            
            .quote p {
                font-size: 18px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="intro">
            <h1>Pourquoi faire un mini-site ?</h1>
            <p>Quelques exemples de questions que vous pourriez répondre</p>
        </div>
        
        <div class="quotes-container">
            <div class="quote quote-1">
                <p>Dis, tu connais un outil pour faire des visios qui respecte la vie privée ?</p>
            </div>
            
            <div class="quote quote-2">
                <p>Dis, je cherche un logiciel pour retoucher mes photos, t'as quoi à me recommander ?</p>
            </div>
            
            <div class="quote quote-3">
                <p>Dis, je veux arrêter d'utiliser mon vieux mail, il y en a qui sont plus éthiques ?</p>
            </div>
        </div>
    </div>
</body>
</html> 