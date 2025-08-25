# Johnny-
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>From Struggling Trader to Funded</title>
    <style>
        :root {
            --primary-bg: #0A0A0A;
            --secondary-bg: #1A1A1A;
            --text-color: #EFEFEF;
            --accent-color: #00BFFF; /* A vibrant blue for a confident, professional feel */
            --button-hover: #009ACD;
            --divider-color: #333;
            --border-radius: 8px;
            --font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
        }

        /* CSS Reset and Normalization */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html, body {
            font-family: var(--font-family);
            background-color: var(--primary-bg);
            color: var(--text-color);
            line-height: 1.6;
            overflow-x: hidden;
            width: 100%;
        }

        .container {
            width: 100%;
            max-width: 900px;
            margin: 0 auto;
            padding: 0 1rem;
        }

        h1, h2, h3, h4, h5, h6 {
            color: var(--text-color);
            line-height: 1.2;
            margin-bottom: 0.5em;
        }
        
        strong, b {
            font-weight: 700;
        }

        em {
            font-style: italic;
        }

        a {
            color: var(--accent-color);
            text-decoration: none;
            transition: color 0.3s ease;
        }

        a:hover {
            color: var(--button-hover);
        }

        .text-center {
            text-align: center;
        }

        /* Utility classes for styling */
        .section {
            padding: 4rem 0;
            border-bottom: 1px solid var(--divider-color);
        }
        
        .hero-section {
            padding: 6rem 0;
            text-align: center;
        }

        .preheader {
            font-size: 1rem;
            text-transform: uppercase;
            letter-spacing: 2px;
            color: var(--accent-color);
            font-weight: 600;
            margin-bottom: 1rem;
        }

        .hero-header {
            font-size: clamp(2rem, 6vw, 4rem);
            font-weight: 800;
            margin-bottom: 0.5rem;
        }

        .hero-subheader {
            font-size: clamp(1.25rem, 3vw, 1.75rem);
            font-weight: 400;
            max-width: 700px;
            margin: 0 auto 2rem;
        }

        .vsl-container {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            gap: 0.75rem;
            cursor: pointer;
            margin-bottom: 2rem;
            position: relative;
        }

        .vsl-icon {
            width: 100%;
            max-width: 650px;
            aspect-ratio: 16/9;
            background-color: var(--secondary-bg);
            border: 2px solid var(--divider-color);
            border-radius: var(--border-radius);
            position: relative;
            display: flex;
            justify-content: center;
            align-items: center;
            transition: transform 0.3s ease;
        }

        .vsl-icon:hover {
            transform: scale(1.02);
        }
        
        .play-button {
            width: 70px;
            height: 70px;
            background-color: rgba(255, 255, 255, 0.2);
            border-radius: 50%;
            display: flex;
            justify-content: center;
            align-items: center;
            backdrop-filter: blur(10px);
            -webkit-backdrop-filter: blur(10px);
        }
        
        .play-button::after {
            content: '';
            width: 0;
            height: 0;
            border-top: 15px solid transparent;
            border-bottom: 15px solid transparent;
            border-left: 20px solid var(--text-color);
            margin-left: 5px;
        }
        
        .cta-text {
            font-size: 1rem;
            text-transform: uppercase;
            letter-spacing: 1px;
            color: var(--text-color);
            font-weight: 600;
        }

        .cta-button {
            display: inline-block;
            background-color: var(--accent-color);
            color: var(--primary-bg);
            padding: 1rem 2rem;
            font-size: 1.25rem;
            font-weight: 700;
            border-radius: 50px;
            transition: background-color 0.3s ease, transform 0.3s ease;
            text-align: center;
        }

        .cta-button:hover {
            background-color: var(--button-hover);
            transform: translateY(-2px);
        }

        /* Problem Section */
        .problem-section {
            background-color: var(--secondary-bg);
        }
        
        .problem-container {
            width: 100%;
            max-width: 700px;
            margin: 0 auto;
        }

        .problem-container h2 {
            font-size: clamp(1.5rem, 4vw, 2.5rem);
            text-align: center;
            margin-bottom: 2rem;
        }
        
        .problem-list {
            list-style: none;
            padding-left: 0;
        }

        .problem-list li {
            font-size: 1.15rem;
            line-height: 1.6;
            margin-bottom: 1.5rem;
            position: relative;
            padding-left: 1.5em;
        }
        
        .problem-list li::before {
            content: '•';
            color: var(--accent-color);
            font-size: 1.5em;
            position: absolute;
            left: 0;
            top: -0.1em;
        }

        /* Story Section */
        .story-section {
            background-color: var(--primary-bg);
        }
        
        .story-section p {
            font-size: 1.15rem;
            max-width: 700px;
            margin: 0 auto 1.5rem;
        }
        
        /* Solution Section */
        .solution-section {
            background-color: var(--secondary-bg);
        }

        .solution-section h2 {
            font-size: clamp(1.5rem, 4vw, 2.5rem);
            text-align: center;
            margin-bottom: 2rem;
        }

        .solution-grid {
            display: grid;
            gap: 2rem;
            grid-template-columns: 1fr;
        }
        
        @media (min-width: 768px) {
            .solution-grid {
                grid-template-columns: repeat(3, 1fr);
            }
        }
        
        .solution-card {
            background-color: var(--primary-bg);
            padding: 2rem;
            border-radius: var(--border-radius);
            text-align: center;
        }

        .solution-card h3 {
            font-size: 1.5rem;
            margin-bottom: 1rem;
        }

        .solution-card p {
            font-size: 1rem;
        }
        
        .benefit-list {
            list-style: none;
            text-align: left;
            margin-top: 2rem;
        }

        .benefit-list li {
            background-color: var(--primary-bg);
            padding: 1rem;
            border-radius: var(--border-radius);
            margin-bottom: 1rem;
            border-left: 4px solid var(--accent-color);
        }

        .benefit-list li strong {
            display: block;
            margin-bottom: 0.5em;
            font-size: 1.15rem;
        }

        /* Product Introduction */
        .product-section {
            background-color: var(--primary-bg);
        }
        
        .product-section h2 {
            font-size: clamp(1.5rem, 4vw, 2.5rem);
            text-align: center;
            margin-bottom: 2rem;
        }
        
        .product-list {
            list-style: none;
            padding: 0;
            display: grid;
            gap: 1.5rem;
        }
        
        .product-list li {
            background-color: var(--secondary-bg);
            padding: 1.5rem;
            border-radius: var(--border-radius);
        }
        
        .product-list li strong {
            display: block;
            font-size: 1.25rem;
            color: var(--accent-color);
            margin-bottom: 0.5em;
        }

        /* Offer Section */
        .offer-section {
            background-color: var(--secondary-bg);
        }
        
        .offer-container {
            width: 100%;
            max-width: 700px;
            margin: 0 auto;
            text-align: center;
        }

        .offer-container h2 {
            font-size: clamp(1.5rem, 4vw, 2.5rem);
            margin-bottom: 2rem;
        }
        
        .offer-card {
            background-color: var(--primary-bg);
            border-radius: var(--border-radius);
            padding: 2.5rem;
            border: 2px solid transparent;
            transition: border-color 0.3s ease;
        }
        
        .offer-card:hover {
            border-color: var(--accent-color);
        }
        
        .offer-card h3 {
            font-size: 2rem;
            color: var(--accent-color);
            margin-bottom: 0.5rem;
        }
        
        .offer-card p {
            font-size: 1.15rem;
            margin-bottom: 1.5rem;
        }
        
        /* FAQ Section */
        .faq-section {
            background-color: var(--primary-bg);
        }
        
        .faq-section h2 {
            font-size: clamp(1.5rem, 4vw, 2.5rem);
            text-align: center;
            margin-bottom: 2rem;
        }
        
        .faq-item {
            background-color: var(--secondary-bg);
            border-radius: var(--border-radius);
            padding: 1.5rem;
            margin-bottom: 1rem;
        }
        
        .faq-question {
            font-size: 1.25rem;
            font-weight: 600;
            margin-bottom: 0.75rem;
        }
        
        .faq-item p {
            font-size: 1rem;
        }
        
        .cta-section {
            background-color: var(--accent-color);
            padding: 4rem 1rem;
            text-align: center;
            color: var(--primary-bg);
            border-radius: var(--border-radius);
        }
        
        .cta-section h2 {
            color: var(--primary-bg);
            font-size: clamp(1.5rem, 4vw, 2.5rem);
            margin-bottom: 1rem;
        }
        
        .cta-section p {
            font-size: 1.25rem;
            max-width: 600px;
            margin: 0 auto 2rem;
            color: rgba(0,0,0,0.8);
        }
        
        .cta-section .cta-button {
            background-color: var(--primary-bg);
            color: var(--accent-color);
            font-size: 1.5rem;
            padding: 1.25rem 2.5rem;
        }
        
        .cta-section .cta-button:hover {
            background-color: #333;
            color: #fff;
        }

        /* Footer */
        .footer {
            text-align: center;
            padding: 2rem 0;
            font-size: 0.9rem;
            color: #666;
            border-top: 1px solid var(--divider-color);
        }
        
        @media (max-width: 768px) {
            .section {
                padding: 3rem 0;
            }
        }
    </style>
</head>
<body>
    
    <header class="hero-section">
        <div class="container">
            <p class="preheader">For the Aspiring Funded Trader</p>
            <h1 class="hero-header">The 1-6 Month Roadmap to Consistent $10K Months... With Zero Personal Risk.</h1>
            <p class="hero-subheader">...By passing prop firm evaluations and scaling accounts without blowing a single one.</p>
            
            <a href="#" class="vsl-container">
                <div class="vsl-icon">
                    <div class="play-button"></div>
                </div>
                <div class="cta-text">Click Here To See The: VSL I WROTE FOR YOU</div>
            </a>
            
            <a href="#" class="cta-button">Apply For The Masterclass</a>
        </div>
    </header>

    <section class="section problem-section">
        <div class="container problem-container">
            <h2>The truth about "trading success" nobody wants to talk about.</h2>
            <p>You’ve watched the videos. You’ve seen the screenshots of 5-figure days. You’ve bought the indicators and the "secret" strategies from a guy in a rented Lamborghini.</p>
            <p>You got into this for freedom. For the lifestyle. For the pride of doing something few people can do.</p>
            <p>But the reality feels different, doesn't it?</p>
            <ul class="problem-list">
                <li>You've blown more accounts than you can count, and the "evaluation fees" are starting to feel less like an investment and more like a bill you can’t afford to pay.</li>
                <li>You get a winning streak and feel like a genius… only to give it all back in one impulsive, revenge-filled trade.</li>
                <li>The promise of "trading with house money" feels like a distant fantasy, because you're stuck in the loop of paying for another evaluation, hoping this time will be different.</li>
            </ul>
            <p>Your charts are cluttered. Your mind is cluttered. And you're starting to wonder if you'll ever break free from the cycle of paying to lose, instead of getting paid to win.</p>
        </div>
    </section>

    <section class="section story-section">
        <div class="container">
            <h2>My journey from paying for evaluations to getting paid by prop firms.</h2>
            <p>A few years ago, I was you. I had the passion, but I lacked the discipline. I'd watch the market, spot a good trade, get in… and then get shaken out. Or I'd get too cocky and watch my P&L disappear in minutes.</p>
            <p>I blew my first two accounts in under a week. Then a third. And a fourth. I was bleeding money just to get a shot at a funded account, and I was losing faith in myself with every failed attempt.</p>
            <p>I realized that the problem wasn't my entry points. It was my lack of a system. The gurus sold me a strategy, but they didn’t give me a plan for when things went wrong. They taught me what to do, but not who to be.</p>
            <p>I stopped looking for the next shiny indicator and started building a real framework. I focused on risk management, psychology, and a clear, phased roadmap. And it worked.</p>
            <p>I finally passed an evaluation. Then another. And then I figured out how to use technology to scale my wins across multiple funded accounts, so a single good trade could generate income from several sources.</p>
            <p>This isn’t about guessing. It's about a repeatable process.</p>
        </div>
    </section>

    <section class="section solution-section">
        <div class="container">
            <h2>The 3-Phase Scaling Roadmap to predictable trading income.</h2>
            <p>Most traders focus on the wrong thing. They obsess over entries when they should be obsessing over their process. This is the simple roadmap I created to go from zero to consistently getting paid by prop firms, without ever risking personal money again.</p>
            <div class="solution-grid">
                <div class="solution-card">
                    <h3>Phase 1: Build Your Base</h3>
                    <p>We'll build the psychological framework and risk management rules you need to pass your first evaluation. This is where you get disciplined and prove to yourself that you can do this.</p>
                </div>
                <div class="solution-card">
                    <h3>Phase 2: Add Accounts</h3>
                    <p>Once you’ve passed one evaluation, we’ll set up 2-3 more funded accounts and use a trade copier to mirror your trades. Now, your wins are multiplied, and a single day's work can produce 2x or 3x the results.</p>
                </div>
                <div class="solution-card">
                    <h3>Phase 3: Scale For More</h3>
                    <p>After consistent payouts, you'll feel confident enough to slowly scale the contracts you trade. This is where you get to the $10K+ per month range, and trading becomes a reliable, full-time income source.</p>
                </div>
            </div>
            
            <ul class="benefit-list">
                <li>
                    <strong>You’ll pass your first evaluation.</strong>
                    You'll get a clear, step-by-step process so you can get your first funded account and feel the satisfaction of trading with capital that isn’t yours.
                </li>
                <li>
                    <strong>You’ll escape the cycle of fear.</strong>
                    You'll build a disciplined mindset and a reliable risk management plan so you can finally trade without the stress of blowing an account.
                </li>
                <li>
                    <strong>You’ll have a clear path to $10K/mo.</strong>
                    You'll get a real, phased roadmap for scaling your income, so you know exactly what to do to turn a side hustle into a sustainable business.
                </li>
            </ul>
        </div>
    </section>

    <section class="section product-section">
        <div class="container">
            <h2>What you get with the mentorship program.</h2>
            <p>I've packaged my entire process into a program that gives you the exact tools, strategies, and support you need to do this yourself.</p>
            <ul class="product-list">
                <li>
                    <strong>The 3-Phase Scaling Roadmap.</strong>
                    A complete, A-to-Z blueprint for going from a brand new trader to a funded one and beyond.
                </li>
                <li>
                    <strong>Exact setups for strategies like Flow State V2 and the Unicorn Model.</strong>
                    My personal rules and frameworks for low-stress, high-probability trades that get consistent results.
                </li>
                <li>
                    <strong>Comprehensive Risk Management.</strong>
                    A bulletproof set of rules to keep you from revenge trading or blowing accounts, no matter what happens in the market.
                </li>
                <li>
                    <strong>Psychology & Accountability Training.</strong>
                    The frameworks and daily check-ins to build the mindset of a professional, disciplined trader—not an impulsive gambler.
                </li>
            </ul>
        </div>
    </section>

    <section class="section offer-section">
        <div class="container offer-container">
            <h2>Your first step is the easiest one.</h2>
            <p>We need to make sure this is the right fit. The best way to do that is with a free masterclass that walks you through the entire framework. It's where I show you exactly how my students are passing evaluations and scaling their accounts to consistent profits.</p>
            
            <div class="offer-card">
                <h3>Free Masterclass This Sunday</h3>
                <p>Register for our live masterclass to learn the exact blueprint for getting funded and hitting consistent $10K months.</p>
                <a href="#" class="cta-button">Reserve My Spot</a>
            </div>
            
            <p class="subtle-text" style="margin-top: 2rem;">This is a live session with a limited number of attendees. We're keeping it small to make sure we can answer questions and keep it highly valuable.</p>
        </div>
    </section>
    
    <section class="section faq-section">
        <div class="container">
            <h2>Is this really for me?</h2>
            <div class="faq-item">
                <p class="faq-question">What if I can't pass an evaluation?</p>
                <p>That’s what this framework is for. Most traders fail because they don’t have a clear plan for risk management and a repeatable process. We’ll build a system for you that gives you the confidence to execute every day without fear of blowing the account.</p>
            </div>
            <div class="faq-item">
                <p class="faq-question">Why should I trust you? You’re just another "guru."</p>
                <p>I’m not a guru. I'm a trader who built a system that works, and now I'm sharing it. The masterclass is free for a reason: I want to show you the exact framework, with no fluff, so you can see for yourself that this is different. It's all about a simple, repeatable process, not vague promises.</p>
            </div>
            <div class="faq-item">
                <p class="faq-question">Can I do this with a full-time job?</p>
                <p>Yes. The strategies and frameworks we use are designed for precision, not time-in-market. We focus on specific setups during high-probability times, which allows you to be in and out of the market quickly. You don’t need to be glued to your screen all day.</p>
            </div>
            
            <div class="cta-section" style="margin-top: 4rem;">
                <h2>The time to stop paying to lose is now.</h2>
                <p>Stop wasting money on evaluations that go nowhere. Stop guessing. Get the plan that gets you funded, fast.</p>
                <a href="#" class="cta-button">Get My Free Blueprint</a>
            </div>
        </div>
    </section>

    <footer class="footer">
        <div class="container">
            <p>&copy; 2025. All Rights Reserved.</p>
        </div>
    </footer>

</body>
</html>
