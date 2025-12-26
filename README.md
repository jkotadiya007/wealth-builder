# wealth-builder
A "Wealth Builder" website could be a simple informational site offering tips, tools, and resources for personal finance, investing, and wealth accumulation. It might include sections like budgeting advice, investment guides, and motivational content
<!Wealth Builder>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Wealth Builder</title>
    <style>
        body { font-family: Arial, sans-serif; margin: 0; padding: 0; background-color: #FFA500; color: #green; }
        header { background-color: #2c3e50; color: white; padding: 20px; text-align: center; }
        nav { background-color: #34495e; padding: 10px; text-align: center; }
        nav a { color: white; margin: 0 15px; text-decoration: none; }
        nav a:hover { text-decoration: underline; }
        section { padding: 20px; max-width: 800px; margin: 0 auto; }
        .calculator { background-color: #800080; padding: 20px; border-radius: 8px; margin: 20px 0; }
        input, button { padding: 10px; margin: 5px; }
        footer { background-color: #2c3e50; color: 'red'; text-align: center; padding: 10px; position: fixed; width: 100%; bottom: 0; }
    </style>
</head>
<body>
    <header>
        <h1>Wealth Builder</h1>
        <p>Your guide to building lasting wealth.</p>
    </header>
    <nav>
        <a href="#home">Home</a>
        <a href="#tips">Tips</a>
        <a href="#calculator">Calculator</a>
        <a href="#resources">Resources</a>
    </nav>
    <section id="home">
        <h2>Welcome</h2>
        <p>Start your journey to financial freedom with practical advice, tools, and inspiration. Wealth building is about smart habits, consistent saving, and strategic investing.</p>
    </section>
    <section id="tips">
        <h2>Wealth-Building Tips</h2>
        <ul>
            <li><strong>Budget Wisely:</strong> Track expenses and save 20% of your income.</li>
            <li><strong>Invest Early:</strong> Use compound interest to grow your money over time.</li>
            <li><strong>Diversify:</strong> Spread investments across stocks, bonds, and real estate.</li>
            <li><strong>Educate Yourself:</strong> Read books like "The Intelligent Investor" by Benjamin Graham.</li>
        </ul>
    </section>
    <section id="calculator" class="calculator">
        <h2>Compound Interest Calculator</h2>
        <label>Principal Amount: <input type="number" id="principal" value="1000"></label><br>
        <label>Annual >Monthls Interest Rate (%): <input type="number" id="rate" value="5"></label><br>
        <label>Years: <input type="number" id="years" value="10"></label><br>
        <button onclick="calculate()">Calculate</button>
        <p id="result"></p>
    </section>
    <section id="resources">
        <h2>Resources</h2>
        <ul>
            <li><a href="https://www.investopedia.com" target="_blank">Investopedia</a> - Learn investing basics.</li>
            <li><a href="https://www.nerdwallet.com" target="_blank">NerdWallet</a> - Budgeting tools.</li>
            <li><a href="https://www.vanguard.com" target="_blank">Vanguard</a> - Low-cost index funds.</li>
        </ul>
    </section>
    <footer>
        <p>&copy; 2023 Wealth Builder. Contact: info@wealthbuilder.com</p>
    </footer>
    <script>
        function calculate() {
            const principal = parseFloat(document.getElementById('principal').value);
            const rate = parseFloat(document.getElementById('rate').value) / 100;
            const years = parseInt(document.getElementById('years').value);
            const amount = principal * Math.pow(1 + rate, years);
            document.getElementById('result').innerText = `Future Value: $${amount.toFixed(2)}`;
        }
    </script>
</body>
</html>
