---
title: "QCM nombres complexes"
order: 8
in_menu: true
---
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>QCM - Propriétés des nombres complexes</title>
    <style>
        * {
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            margin: 0;
            padding: 20px;
            background-color: #f5f9ff;
            color: #333;
            line-height: 1.6;
        }
        
        .container {
            max-width: 800px;
            margin: 0 auto;
            background-color: white;
            border-radius: 12px;
            box-shadow: 0 5px 15px rgba(0, 0, 100, 0.1);
            padding: 30px;
            margin-bottom: 30px;
        }
        
        header {
            text-align: center;
            margin-bottom: 30px;
            padding-bottom: 20px;
            border-bottom: 2px solid #4a6fa5;
        }
        
        h1 {
            color: #2c3e6e;
            margin-bottom: 10px;
        }
        
        .subtitle {
            color: #5a7cbf;
            font-size: 1.1em;
        }
        
        .intro {
            background-color: #edf3ff;
            padding: 15px 20px;
            border-radius: 8px;
            margin-bottom: 25px;
            border-left: 4px solid #4a6fa5;
        }
        
        .question {
            margin-bottom: 25px;
            padding: 20px;
            border-radius: 8px;
            background-color: #f9fbff;
            border: 1px solid #e0e8ff;
            transition: all 0.3s ease;
        }
        
        .question:hover {
            box-shadow: 0 3px 8px rgba(0, 0, 100, 0.08);
        }
        
        .question-title {
            font-weight: 600;
            color: #2c3e6e;
            margin-bottom: 15px;
            font-size: 1.1em;
        }
        
        .options {
            margin-left: 10px;
        }
        
        .option {
            margin-bottom: 10px;
            padding: 10px;
            border-radius: 6px;
            cursor: pointer;
            transition: background-color 0.2s;
        }
        
        .option:hover {
            background-color: #f0f5ff;
        }
        
        .option input {
            margin-right: 10px;
            cursor: pointer;
        }
        
        .option label {
            cursor: pointer;
            display: flex;
            align-items: center;
        }
        
        .formula {
            font-family: 'Cambria Math', 'Times New Roman', serif;
            font-size: 1.1em;
            background-color: #f8faff;
            padding: 5px 10px;
            border-radius: 4px;
            display: inline-block;
            margin: 2px 0;
        }
        
        .correct {
            background-color: #e8f7ef !important;
            border-left: 4px solid #2ecc71;
        }
        
        .incorrect {
            background-color: #fdeded !important;
            border-left: 4px solid #e74c3c;
        }
        
        .result {
            display: none;
            padding: 10px;
            margin-top: 10px;
            border-radius: 6px;
            font-weight: 500;
        }
        
        .correct .result {
            display: block;
            color: #27ae60;
        }
        
        .incorrect .result {
            display: block;
            color: #c0392b;
        }
        
        .buttons {
            display: flex;
            justify-content: center;
            gap: 15px;
            margin-top: 30px;
        }
        
        button {
            padding: 12px 24px;
            border: none;
            border-radius: 6px;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s;
            font-size: 1em;
        }
        
        #submit-btn {
            background-color: #4a6fa5;
            color: white;
        }
        
        #submit-btn:hover {
            background-color: #3a5a8a;
        }
        
        #reset-btn {
            background-color: #e0e8ff;
            color: #4a6fa5;
        }
        
        #reset-btn:hover {
            background-color: #d0d8f0;
        }
        
        .score-container {
            text-align: center;
            margin-top: 30px;
            padding: 20px;
            background-color: #edf3ff;
            border-radius: 8px;
            display: none;
        }
        
        .score {
            font-size: 2em;
            font-weight: bold;
            color: #2c3e6e;
            margin: 10px 0;
        }
        
        .feedback {
            font-size: 1.1em;
            margin-top: 10px;
        }
        
        .good-feedback {
            color: #27ae60;
        }
        
        .medium-feedback {
            color: #f39c12;
        }
        
        .poor-feedback {
            color: #e74c3c;
        }
        
        @media (max-width: 600px) {
            .container {
                padding: 15px;
            }
            
            .buttons {
                flex-direction: column;
            }
            
            button {
                width: 100%;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1>QCM - Propriétés des nombres complexes</h1>
            <p class="subtitle">Conjugué, module et argument</p>
        </header>
        
        <div class="intro">
            <p>Ce questionnaire à choix multiples porte sur les propriétés des nombres complexes vues dans le chapitre IV. Pour chaque question, choisissez la bonne réponse parmi les propositions. Vous pouvez vérifier vos réponses à la fin du test.</p>
            <p>Rappel : \( \overline{z} \) désigne le conjugué de \( z \), \( |z| \) son module et \( \arg(z) \) son argument.</p>
        </div>
        
        <form id="quiz-form">
            <!-- Question 1 -->
            <div class="question" id="q1">
                <div class="question-title">Question 1 : Quelle est la propriété correcte pour le conjugué d'une somme ?</div>
                <div class="options">
                    <div class="option">
                        <label>
                            <input type="radio" name="q1" value="a">
                            <span class="formula">\(\overline{z_1 + z_2} = \overline{z_1} + \overline{z_2}\)</span>
                        </label>
                    </div>
                    <div class="option">
                        <label>
                            <input type="radio" name="q1" value="b">
                            <span class="formula">\(\overline{z_1 + z_2} = \overline{z_1} - \overline{z_2}\)</span>
                        </label>
                    </div>
                    <div class="option">
                        <label>
                            <input type="radio" name="q1" value="c">
                            <span class="formula">\(\overline{z_1 + z_2} = \overline{z_1} \times \overline{z_2}\)</span>
                        </label>
                    </div>
                </div>
                <div class="result"></div>
            </div>
            
            <!-- Question 2 -->
            <div class="question" id="q2">
                <div class="question-title">Question 2 : Quelle est la propriété correcte pour le conjugué d'un produit ?</div>
                <div class="options">
                    <div class="option">
                        <label>
                            <input type="radio" name="q2" value="a">
                            <span class="formula">\(\overline{z_1 \times z_2} = \overline{z_1} + \overline{z_2}\)</span>
                        </label>
                    </div>
                    <div class="option">
                        <label>
                            <input type="radio" name="q2" value="b">
                            <span class="formula">\(\overline{z_1 \times z_2} = \overline{z_1} \times \overline{z_2}\)</span>
                        </label>
                    </div>
                    <div class="option">
                        <label>
                            <input type="radio" name="q2" value="c">
                            <span class="formula">\(\overline{z_1 \times z_2} = \frac{\overline{z_1}}{\overline{z_2}}\)</span>
                        </label>
                    </div>
                </div>
                <div class="result"></div>
            </div>
            
            <!-- Question 3 -->
            <div class="question" id="q3">
                <div class="question-title">Question 3 : Quelle est la propriété correcte pour le module d'un produit ?</div>
                <div class="options">
                    <div class="option">
                        <label>
                            <input type="radio" name="q3" value="a">
                            <span class="formula">\(|z_1 \times z_2| = |z_1| + |z_2|\)</span>
                        </label>
                    </div>
                    <div class="option">
                        <label>
                            <input type="radio" name="q3" value="b">
                            <span class="formula">\(|z_1 \times z_2| = |z_1| \times |z_2|\)</span>
                        </label>
                    </div>
                    <div class="option">
                        <label>
                            <input type="radio" name="q3" value="c">
                            <span class="formula">\(|z_1 \times z_2| = |z_1| - |z_2|\)</span>
                        </label>
                    </div>
                </div>
                <div class="result"></div>
            </div>
            
            <!-- Question 4 -->
            <div class="question" id="q4">
                <div class="question-title">Question 4 : Quelle inégalité est vérifiée pour le module d'une somme ?</div>
                <div class="options">
                    <div class="option">
                        <label>
                            <input type="radio" name="q4" value="a">
                            <span class="formula">\(|z_1 + z_2| \leq |z_1| + |z_2|\)</span>
                        </label>
                    </div>
                    <div class="option">
                        <label>
                            <input type="radio" name="q4" value="b">
                            <span class="formula">\(|z_1 + z_2| \geq |z_1| + |z_2|\)</span>
                        </label>
                    </div>
                    <div class="option">
                        <label>
                            <input type="radio" name="q4" value="c">
                            <span class="formula">\(|z_1 + z_2| = |z_1| + |z_2|\)</span>
                        </label>
                    </div>
                </div>
                <div class="result"></div>
            </div>
            
            <!-- Question 5 -->
            <div class="question" id="q5">
                <div class="question-title">Question 5 : Quelle est la relation entre les arguments d'un produit ?</div>
                <div class="options">
                    <div class="option">
                        <label>
                            <input type="radio" name="q5" value="a">
                            <span class="formula">\(\arg(z_1 \times z_2) \equiv \arg(z_1) + \arg(z_2) \ [2\pi]\)</span>
                        </label>
                    </div>
                    <div class="option">
                        <label>
                            <input type="radio" name="q5" value="b">
                            <span class="formula">\(\arg(z_1 \times z_2) \equiv \arg(z_1) - \arg(z_2) \ [2\pi]\)</span>
                        </label>
                    </div>
                    <div class="option">
                        <label>
                            <input type="radio" name="q5" value="c">
                            <span class="formula">\(\arg(z_1 \times z_2) \equiv \arg(z_1) \times \arg(z_2) \ [2\pi]\)</span>
                        </label>
                    </div>
                </div>
                <div class="result"></div>
            </div>
            
            <!-- Question 6 -->
            <div class="question" id="q6">
                <div class="question-title">Question 6 : Quelle est la propriété correcte pour l'argument d'un quotient ?</div>
                <div class="options">
                    <div class="option">
                        <label>
                            <input type="radio" name="q6" value="a">
                            <span class="formula">\(\arg\left(\frac{z_1}{z_2}\right) \equiv \arg(z_1) + \arg(z_2) \ [2\pi]\)</span>
                        </label>
                    </div>
                    <div class="option">
                        <label>
                            <input type="radio" name="q6" value="b">
                            <span class="formula">\(\arg\left(\frac{z_1}{z_2}\right) \equiv \arg(z_1) - \arg(z_2) \ [2\pi]\)</span>
                        </label>
                    </div>
                    <div class="option">
                        <label>
                            <input type="radio" name="q6" value="c">
                            <span class="formula">\(\arg\left(\frac{z_1}{z_2}\right) \equiv \frac{\arg(z_1)}{\arg(z_2)} \ [2\pi]\)</span>
                        </label>
                    </div>
                </div>
                <div class="result"></div>
            </div>
            
            <!-- Question 7 -->
            <div class="question" id="q7">
                <div class="question-title">Question 7 : Comment s'exprime la puissance d'un nombre complexe en forme polaire ?</div>
                <div class="options">
                    <div class="option">
                        <label>
                            <input type="radio" name="q7" value="a">
                            <span class="formula">\([r, \alpha]^n = [r^n, n\alpha]\)</span>
                        </label>
                    </div>
                    <div class="option">
                        <label>
                            <input type="radio" name="q7" value="b">
                            <span class="formula">\([r, \alpha]^n = [r, n\alpha]\)</span>
                        </label>
                    </div>
                    <div class="option">
                        <label>
                            <input type="radio" name="q7" value="c">
                            <span class="formula">\([r, \alpha]^n = [n r, \alpha]\)</span>
                        </label>
                    </div>
                </div>
                <div class="result"></div>
            </div>
            
            <!-- Question 8 -->
            <div class="question" id="q8">
                <div class="question-title">Question 8 : Quelle est la propriété correcte pour le conjugué d'une puissance ?</div>
                <div class="options">
                    <div class="option">
                        <label>
                            <input type="radio" name="q8" value="a">
                            <span class="formula">\(\overline{z^n} = (\overline{z})^n\)</span>
                        </label>
                    </div>
                    <div class="option">
                        <label>
                            <input type="radio" name="q8" value="b">
                            <span class="formula">\(\overline{z^n} = \overline{z} \times n\)</span>
                        </label>
                    </div>
                    <div class="option">
                        <label>
                            <input type="radio" name="q8" value="c">
                            <span class="formula">\(\overline{z^n} = n \overline{z}\)</span>
                        </label>
                    </div>
                </div>
                <div class="result"></div>
            </div>
            
            <div class="buttons">
                <button type="button" id="submit-btn">Soumettre les réponses</button>
                <button type="button" id="reset-btn">Réinitialiser</button>
            </div>
        </form>
        
        <div class="score-container" id="score-container">
            <h3>Résultat du QCM</h3>
            <div class="score" id="score">0/8</div>
            <div class="feedback" id="feedback"></div>
        </div>
    </div>

    <!-- MathJax pour l'affichage des formules mathématiques -->
    <script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
    <script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
    
    <script>
        // Réponses correctes
        const correctAnswers = {
            q1: "a",
            q2: "b", 
            q3: "b",
            q4: "a",
            q5: "a",
            q6: "b",
            q7: "a",
            q8: "a"
        };
        
        // Explications des réponses
        const explanations = {
            q1: "Le conjugué d'une somme est égal à la somme des conjugués.",
            q2: "Le conjugué d'un produit est égal au produit des conjugués.",
            q3: "Le module d'un produit est égal au produit des modules.",
            q4: "C'est l'inégalité triangulaire pour les nombres complexes.",
            q5: "L'argument d'un produit est égal à la somme des arguments modulo \(2\pi\).",
            q6: "L'argument d'un quotient est égal à la différence des arguments modulo \(2\pi\).",
            q7: "En forme polaire, la puissance n-ième élève le module à la puissance n et multiplie l'argument par n.",
            q8: "Le conjugué d'une puissance est égal à la puissance du conjugué."
        };
        
        // Initialisation
        document.addEventListener('DOMContentLoaded', function() {
            // Soumission du formulaire
            document.getElementById('submit-btn').addEventListener('click', submitQuiz);
            
            // Réinitialisation
            document.getElementById('reset-btn').addEventListener('click', resetQuiz);
            
            // Initialiser MathJax
            if (window.MathJax) {
                MathJax.typesetPromise();
            }
        });
        
        function submitQuiz() {
            let score = 0;
            const totalQuestions = Object.keys(correctAnswers).length;
            
            // Parcourir toutes les questions
            for (let i = 1; i <= totalQuestions; i++) {
                const questionId = `q${i}`;
                const questionElement = document.getElementById(questionId);
                const selectedOption = document.querySelector(`input[name="${questionId}"]:checked`);
                
                // Réinitialiser les classes
                questionElement.classList.remove('correct', 'incorrect');
                
                // Vérifier si une réponse a été sélectionnée
                if (selectedOption) {
                    const userAnswer = selectedOption.value;
                    const correctAnswer = correctAnswers[questionId];
                    
                    // Vérifier si la réponse est correcte
                    if (userAnswer === correctAnswer) {
                        score++;
                        questionElement.classList.add('correct');
                        questionElement.querySelector('.result').textContent = `Correct! ${explanations[questionId]}`;
                    } else {
                        questionElement.classList.add('incorrect');
                        
                        // Trouver la bonne réponse
                        let correctOptionText = '';
                        const options = questionElement.querySelectorAll('.option');
                        options.forEach(option => {
                            const input = option.querySelector('input');
                            if (input.value === correctAnswer) {
                                const formula = option.querySelector('.formula').textContent;
                                correctOptionText = formula;
                            }
                        });
                        
                        questionElement.querySelector('.result').textContent = `Incorrect. La bonne réponse est : ${correctOptionText}. ${explanations[questionId]}`;
                    }
                } else {
                    // Aucune réponse sélectionnée
                    questionElement.classList.add('incorrect');
                    
                    // Trouver la bonne réponse
                    let correctOptionText = '';
                    const options = questionElement.querySelectorAll('.option');
                    options.forEach(option => {
                        const input = option.querySelector('input');
                        if (input.value === correctAnswers[questionId]) {
                            const formula = option.querySelector('.formula').textContent;
                            correctOptionText = formula;
                        }
                    });
                    
                    questionElement.querySelector('.result').textContent = `Vous n'avez pas sélectionné de réponse. La bonne réponse est : ${correctOptionText}. ${explanations[questionId]}`;
                }
            }
            
            // Afficher le score
            const scoreContainer = document.getElementById('score-container');
            const scoreElement = document.getElementById('score');
            const feedbackElement = document.getElementById('feedback');
            
            scoreElement.textContent = `${score}/${totalQuestions}`;
            scoreContainer.style.display = 'block';
            
            // Donner un feedback en fonction du score
            let feedback = '';
            if (score === totalQuestions) {
                feedback = 'Excellent ! Vous maîtrisez parfaitement ces propriétés.';
                feedbackElement.className = 'feedback good-feedback';
            } else if (score >= totalQuestions / 2) {
                feedback = 'Bon travail ! Vous connaissez bien la majorité des propriétés.';
                feedbackElement.className = 'feedback medium-feedback';
            } else {
                feedback = 'Continuez à réviser ces propriétés importantes.';
                feedbackElement.className = 'feedback poor-feedback';
            }
            
            feedbackElement.textContent = feedback;
            
            // Faire défiler jusqu'au résultat
            scoreContainer.scrollIntoView({ behavior: 'smooth' });
            
            // Recalculer MathJax pour les formules dans les résultats
            if (window.MathJax) {
                MathJax.typesetPromise();
            }
        }
        
        function resetQuiz() {
            // Réinitialiser toutes les sélections
            const allInputs = document.querySelectorAll('input[type="radio"]');
            allInputs.forEach(input => {
                input.checked = false;
            });
            
            // Réinitialiser les classes et résultats
            const allQuestions = document.querySelectorAll('.question');
            allQuestions.forEach(question => {
                question.classList.remove('correct', 'incorrect');
                question.querySelector('.result').textContent = '';
            });
            
            // Masquer le score
            document.getElementById('score-container').style.display = 'none';
        }
    </script>
</body>
</html> 