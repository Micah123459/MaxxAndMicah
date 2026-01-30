<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Horizon Festival Clicker</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Segoe+UI:wght@300;400;700;900&display=swap');

        :root {
            --h-pink: #ff007f;
            --h-cyan: #00f2ff;
            --h-purple: #bd00ff;
            --h-yellow: #ffcc00;
            --h-dark: #121212;
            --h-panel: rgba(20, 20, 20, 0.95);
            --text-main: #ffffff;
            --text-dim: #a0a0a0;
        }

        body {
            margin: 0;
            background-color: var(--h-dark);
            background-image: linear-gradient(135deg, #1a0b1a 0%, #0b1a1a 100%);
            color: var(--text-main);
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            height: 100vh;
            overflow: hidden;
            display: flex;
            flex-direction: column;
            user-select: none;
        }

        /* Background Animated Elements */
        .bg-gradient {
            position: absolute;
            top: 0; left: 0; width: 100%; height: 100%;
            background: radial-gradient(circle at 50% 100%, rgba(255, 0, 127, 0.15), transparent 60%);
            z-index: -1;
            pointer-events: none;
        }

        /* Layout */
        #game-container {
            display: grid;
            grid-template-columns: 350px 1fr 350px;
            height: 100%;
            gap: 20px;
            padding: 20px;
            box-sizing: border-box;
            position: relative;
        }

        /* Panels */
        .panel {
            background: var(--h-panel);
            border-radius: 4px;
            border-top: 4px solid var(--h-pink);
            display: flex;
            flex-direction: column;
            overflow: hidden;
            box-shadow: 0 10px 30px rgba(0,0,0,0.5);
            transition: transform 0.3s ease-in-out, opacity 0.3s;
        }

        .panel-header {
            padding: 15px;
            font-weight: 900;
            text-transform: uppercase;
            letter-spacing: 2px;
            font-size: 1.2rem;
            background: rgba(255,255,255,0.05);
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .close-panel-btn {
            display: none;
            background: transparent;
            border: 1px solid rgba(255,255,255,0.3);
            color: white;
            padding: 5px 10px;
            cursor: pointer;
            text-transform: uppercase;
            font-weight: bold;
            font-size: 0.8rem;
        }

        .scroll-area {
            flex: 1;
            overflow-y: auto;
            padding: 10px;
        }

        .scroll-area::-webkit-scrollbar { width: 6px; }
        .scroll-area::-webkit-scrollbar-thumb { background: var(--h-pink); border-radius: 3px; }
        .scroll-area::-webkit-scrollbar-track { background: rgba(0,0,0,0.3); }

        /* Center Stage */
        #center-stage {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            position: relative;
            z-index: 1;
        }

        /* Navigation Buttons */
        .nav-controls {
            display: none;
            gap: 10px;
            margin-top: 20px;
            width: 100%;
            justify-content: center;
            flex-wrap: wrap;
        }

        .nav-btn {
            padding: 10px 15px;
            font-size: 0.9rem;
            font-weight: 900;
            text-transform: uppercase;
            border: none;
            cursor: pointer;
            color: white;
            box-shadow: 0 4px 15px rgba(0,0,0,0.3);
            transition: transform 0.1s;
            letter-spacing: 1px;
            flex: 1;
            min-width: 100px;
            text-align: center;
        }

        .nav-btn:active { transform: scale(0.95); }

        .btn-shop { 
            background: linear-gradient(135deg, var(--h-pink), #bf0060); 
            border-bottom: 3px solid #800040;
        }
        .btn-fest { 
            background: linear-gradient(135deg, var(--h-purple), #8000b0); 
            border-bottom: 3px solid #550075;
        }
        .btn-upg {
            background: linear-gradient(135deg, var(--h-yellow), #b38f00);
            color: #121212;
            border-bottom: 3px solid #997a00;
        }

        /* Stats Header */
        .stats-bar {
            position: absolute;
            top: 0;
            width: 100%;
            display: flex;
            justify-content: space-between;
            padding: 20px;
            box-sizing: border-box;
            text-shadow: 0 2px 10px rgba(0,0,0,0.5);
            pointer-events: none;
        }

        .stat-group {
            text-align: center;
            pointer-events: auto;
        }

        .stat-label {
            font-size: 0.8rem;
            color: var(--text-dim);
            text-transform: uppercase;
            font-weight: 700;
            letter-spacing: 1px;
        }

        .stat-value {
            font-size: 2.5rem;
            font-weight: 300;
        }

        .cr-symbol { color: var(--h-cyan); font-weight: 700; margin-right: 5px; }

        /* Drive Button / Car */
        #drive-btn {
            width: 280px;
            height: 280px;
            border-radius: 50%;
            background: radial-gradient(circle, rgba(255,255,255,0.1) 0%, rgba(0,0,0,0.5) 70%);
            border: 8px solid rgba(255,255,255,0.1);
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            transition: all 0.1s;
            position: relative;
            box-shadow: 0 0 50px rgba(0, 242, 255, 0.1);
            margin-top: 40px;
        }

        #drive-btn:active {
            transform: scale(0.95);
            border-color: var(--h-pink);
            box-shadow: 0 0 80px rgba(255, 0, 127, 0.4);
        }

        #drive-btn:hover {
            border-color: var(--h-cyan);
        }

        .drive-text {
            font-size: 1.5rem;
            font-weight: 900;
            text-transform: uppercase;
            letter-spacing: 4px;
            pointer-events: none;
        }

        /* Cards */
        .card {
            background: rgba(255,255,255,0.05);
            border-bottom: 1px solid rgba(255,255,255,0.1);
            padding: 15px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            transition: background 0.2s;
            cursor: pointer;
            position: relative;
            overflow: hidden;
        }

        .card:hover { background: rgba(255,255,255,0.1); }
        .card:active { background: rgba(255,255,255,0.15); transform: translateX(2px); }
        .card.disabled { opacity: 0.5; pointer-events: none; filter: grayscale(1); }

        .card-info h3 { margin: 0; font-size: 1rem; font-weight: 700; }
        .card-info p { margin: 2px 0 0; font-size: 0.8rem; color: var(--text-dim); }
        
        .card-price {
            text-align: right;
            font-weight: 700;
            color: var(--h-cyan);
            display: flex;
            flex-direction: column;
            align-items: flex-end;
        }

        .card-owned {
            font-size: 0.7rem;
            color: var(--h-pink);
            text-transform: uppercase;
            letter-spacing: 1px;
            margin-top: 2px;
        }

        .buy-hint {
            font-size: 0.7rem;
            background: rgba(255,255,255,0.1);
            padding: 4px 8px;
            border-radius: 4px;
            margin-top: 4px;
            display: inline-block;
            transition: background 0.2s;
            color: white;
        }
        
        .card:hover .buy-hint {
            background: var(--h-cyan);
            color: #000;
        }

        .card.upgrade-card {
            border-left: 4px solid var(--h-yellow);
        }
        .card.upgrade-card .buy-hint {
            background: rgba(255,204,0,0.2);
            color: var(--h-yellow);
        }
        .card.upgrade-card:hover .buy-hint {
            background: var(--h-yellow);
            color: #000;
        }

        .rarity-strip {
            position: absolute;
            left: 0; top: 0; bottom: 0;
            width: 4px;
        }
        
        .class-d { background: #607d8b; }
        .class-c { background: #ffeb3b; }
        .class-b { background: #ff9800; }
        .class-a { background: #f44336; }
        .class-s1 { background: #9c27b0; }
        .class-s2 { background: #3f51b5; }
        .class-x { background: #00e676; box-shadow: 0 0 10px #00e676; }
        .class-hyper { background: #00bcd4; box-shadow: 0 0 15px #00bcd4; }
        .class-concept { background: #e91e63; box-shadow: 0 0 15px #e91e63; }
        .class-future { background: #9c27b0; box-shadow: 0 0 15px #9c27b0; }
        .class-cosmic { background: white; box-shadow: 0 0 20px white; }

        /* Influence Level */
        .level-badge {
            background: var(--h-pink);
            color: white;
            width: 40px;
            height: 40px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: 900;
            font-size: 1.2rem;
            box-shadow: 0 0 15px var(--h-pink);
        }

        /* Notifications */
        .float-text {
            position: absolute;
            font-weight: bold;
            pointer-events: none;
            animation: floatUp 1s forwards;
            font-size: 1.2rem;
            text-shadow: 0 2px 4px rgba(0,0,0,0.8);
        }

        @keyframes floatUp {
            0% { transform: translateY(0) scale(1); opacity: 1; }
            100% { transform: translateY(-50px) scale(1.2); opacity: 0; }
        }

        /* Wheelspin Modal */
        #modal-overlay {
            position: fixed; top: 0; left: 0; width: 100%; height: 100%;
            background: rgba(0,0,0,0.9);
            display: none;
            justify-content: center;
            align-items: center;
            z-index: 100;
        }

        .spin-container {
            text-align: center;
        }

        .spin-result {
            font-size: 4rem;
            font-weight: 900;
            color: var(--h-cyan);
            margin: 20px 0;
            text-shadow: 0 0 30px var(--h-cyan);
            animation: popIn 0.5s;
        }

        .spin-btn {
            padding: 15px 40px;
            background: var(--h-pink);
            border: none;
            color: white;
            font-size: 1.5rem;
            font-weight: bold;
            text-transform: uppercase;
            cursor: pointer;
            box-shadow: 0 0 20px var(--h-pink);
        }

        /* --- RESPONSIVE / CHROMEBOOK FIXES --- */
        @media (max-width: 1000px) {
            #game-container {
                display: block; /* Stack everything */
                padding: 0;
            }

            #center-stage {
                height: 100%;
                width: 100%;
            }

            .panel {
                position: fixed;
                top: 0; left: 0;
                width: 100%; height: 100%;
                z-index: 50;
                border-radius: 0;
                border-top: none;
                transform: translateY(100%);
                opacity: 0;
                pointer-events: none;
            }

            .panel.active {
                transform: translateY(0);
                opacity: 1;
                pointer-events: auto;
            }

            .nav-controls {
                display: flex;
            }

            .close-panel-btn {
                display: block;
            }

            #drive-btn {
                width: 240px;
                height: 240px;
            }
        }
    </style>
</head>
<body>

    <div class="bg-gradient"></div>

    <div id="game-container">
        <!-- Left Panel: Autoshow -->
        <div class="panel" id="panel-autoshow">
            <div class="panel-header">
                <div>AUTOSHOW <span>Get Cars</span></div>
                <button class="close-panel-btn" onclick="togglePanel('panel-autoshow')">Back</button>
            </div>
            <div class="scroll-area" id="autoshow-list"></div>
        </div>

        <!-- Center Stage -->
        <div id="center-stage">
            <div class="stats-bar">
                <div class="stat-group" style="text-align: left;">
                    <div class="stat-label">Credits</div>
                    <div class="stat-value" style="color:var(--h-cyan)"><span class="cr-symbol">CR</span><span id="cr-display">0</span></div>
                    <div class="stat-label" style="margin-top:5px; font-size: 0.7rem;">+<span id="income-display">0</span> CR/s</div>
                </div>
                <div class="stat-group" style="text-align: right;">
                    <div class="stat-label">Influence</div>
                    <div style="display:flex; align-items:center; justify-content: flex-end; gap: 10px;">
                        <span class="stat-value" id="inf-display">0</span>
                        <div class="level-badge" id="level-display">1</div>
                    </div>
                    <div class="stat-label" style="margin-top:5px; font-size: 0.7rem;" id="wheelspin-notify">Next Wheelspin: 2,500</div>
                </div>
            </div>

            <div id="drive-btn">
                <div class="drive-text">DRIVE</div>
            </div>

            <!-- Navigation Buttons -->
            <div class="nav-controls">
                <button class="nav-btn btn-shop" onclick="togglePanel('panel-autoshow')">Autoshow</button>
                <button class="nav-btn btn-upg" onclick="togglePanel('panel-upgrades')">Upgrades</button>
                <button class="nav-btn btn-fest" onclick="togglePanel('panel-festival')">Festival</button>
            </div>
        </div>

        <!-- Upgrades Panel -->
        <div class="panel" id="panel-upgrades" style="display: none;">
            <div class="panel-header">
                <div>GARAGE <span>Upgrades</span></div>
                <button class="close-panel-btn" onclick="togglePanel('panel-upgrades')">Back</button>
            </div>
            <div class="scroll-area" id="upgrades-list"></div>
        </div>

        <!-- Right Panel: Festival -->
        <div class="panel" id="panel-festival">
            <div class="panel-header">
                <div>FESTIVAL <span>Expansion</span></div>
                <button class="close-panel-btn" onclick="togglePanel('panel-festival')">Back</button>
            </div>
            <div class="scroll-area" id="sites-list"></div>
        </div>
    </div>

    <!-- Wheelspin Modal -->
    <div id="modal-overlay">
        <div class="spin-container">
            <h1 style="text-transform: uppercase; font-style: italic;">HORIZON WHEELSPIN</h1>
            <div id="spin-animation" style="font-size: 1.5rem; color: #aaa; margin-bottom: 20px;">Spinning...</div>
            <div class="spin-result hidden" id="spin-result">CR 50,000</div>
            <button class="spin-btn hidden" id="claim-btn">CLAIM REWARD</button>
        </div>
    </div>

<script>
    /* --- Data Generation --- */
    
    // Tier Config - Scaling to 100 Qi
    // 50 to 10^20 (100 Quintillion) over 100 steps
    // Roughly 1.52 multiplier per step
    const TIER_CONFIG = [
        { id: 'class-d', name: 'D', startPrice: 50, powerMult: 1, count: 15 },
        { id: 'class-c', name: 'C', startPrice: 5000, powerMult: 50, count: 15 },
        { id: 'class-b', name: 'B', startPrice: 500000, powerMult: 2500, count: 15 },
        { id: 'class-a', name: 'A', startPrice: 50000000, powerMult: 150000, count: 15 },
        { id: 'class-s1', name: 'S1', startPrice: 5000000000, powerMult: 10000000, count: 15 },
        { id: 'class-s2', name: 'S2', startPrice: 500000000000, powerMult: 800000000, count: 15 },
        { id: 'class-x', name: 'X', startPrice: 50000000000000, powerMult: 50000000000, count: 10 }
    ];

    const BRANDS = ['Ford', 'Honda', 'Toyota', 'Subaru', 'BMW', 'Nissan', 'Audi', 'Chevrolet', 'Dodge', 'Ferrari', 'Lamborghini', 'Bugatti', 'Koenigsegg'];
    const MODELS = ['Focus', 'Civic', 'Supra', 'Impreza', 'M3', 'GTR', 'R8', 'Corvette', 'Viper', '488', 'Huracan', 'Chiron', 'Jesko'];
    
    let game = {
        cr: 0,
        influence: 0,
        level: 1,
        nextLevelReq: 2500,
        cars: [],
        sites: [],
        upgrades: []
    };

    function initGameData() {
        game.cars = [];
        let carIdCounter = 0;

        TIER_CONFIG.forEach(tier => {
            for (let i = 0; i < tier.count; i++) {
                // Scale within tier
                let baseCost = tier.startPrice * Math.pow(1.6, i); 
                let basePower = tier.powerMult * Math.pow(1.5, i);
                
                let owned = 0;
                let name = "";
                
                if (carIdCounter === 0) {
                    baseCost = 43.47826; 
                    basePower = 1;
                    owned = 1; 
                    name = "Starter Hatch";
                } else {
                    const brand = BRANDS[Math.floor(Math.random() * BRANDS.length)];
                    const model = MODELS[Math.floor(Math.random() * MODELS.length)];
                    name = `${brand} ${model} ${tier.name}`;
                }

                game.cars.push({
                    id: `c${carIdCounter}`,
                    name: name,
                    class: tier.id,
                    baseCost: baseCost, 
                    basePower: Math.floor(basePower),
                    owned: owned
                });
                carIdCounter++;
            }
        });

        // Ensure final car is EXACTLY 100 Qi
        // 100 Qi = 100 * 10^18 = 1e20
        // Wait, request was "100 qi" - usually quintillion in games is 10^18. 
        // Let's set the last generated car to specifically be 100 Quintillion to match request.
        game.cars[game.cars.length - 1].baseCost = 100 * 1e18; // 100 Quintillion
        game.cars[game.cars.length - 1].name = "Bugatti Chiron X";
        game.cars[game.cars.length - 1].basePower = 1e15; // Massive power

        game.sites = [
            { id: 's1', name: 'Horizon Main Stage', desc: 'The heart of the festival.', baseCost: 100, baseIncome: 2, owned: 0 },
            { id: 's2', name: 'Apex Outpost', desc: 'Road Racing events.', baseCost: 10000, baseIncome: 150, owned: 0 },
            { id: 's3', name: 'Wilds Outpost', desc: 'Dirt Racing events.', baseCost: 1000000, baseIncome: 12000, owned: 0 },
            { id: 's4', name: 'Baja Outpost', desc: 'Cross Country events.', baseCost: 100000000, baseIncome: 800000, owned: 0 },
            { id: 's5', name: 'Rush Outpost', desc: 'PR Stunts.', baseCost: 10000000000, baseIncome: 50000000, owned: 0 },
            { id: 's6', name: 'Street Scene', desc: 'Underground races.', baseCost: 1000000000000, baseIncome: 4000000000, owned: 0 }
        ];

        game.upgrades = [
            { id: 'u1', name: 'Weight Reduction', desc: '+10% Driving Income', baseCost: 5000, multiplier: 0.1, type: 'active', owned: 0 },
            { id: 'u2', name: 'Sponsorship Deal', desc: '+10% Passive Income', baseCost: 5000, multiplier: 0.1, type: 'passive', owned: 0 },
            { id: 'u3', name: 'Turbocharger', desc: '+20% Driving Income', baseCost: 250000, multiplier: 0.2, type: 'active', owned: 0 },
            { id: 'u4', name: 'TV Commercial', desc: '+20% Passive Income', baseCost: 250000, multiplier: 0.2, type: 'passive', owned: 0 },
            { id: 'u5', name: 'Engine Swap', desc: '+50% Driving Income', baseCost: 100000000, multiplier: 0.5, type: 'active', owned: 0 },
            { id: 'u6', name: 'Viral Marketing', desc: '+50% Passive Income', baseCost: 100000000, multiplier: 0.5, type: 'passive', owned: 0 },
            { id: 'u7', name: 'Race Transmission', desc: '+100% Driving Income', baseCost: 500000000000, multiplier: 1.0, type: 'active', owned: 0 },
            { id: 'u8', name: 'Global Broadcast', desc: '+100% Passive Income', baseCost: 500000000000, multiplier: 1.0, type: 'passive', owned: 0 }
        ];
    }

    initGameData();

    // Try load logic
    function loadGame() {
        const saved = localStorage.getItem('horizonClickerSave');
        if (saved) {
            try {
                const s = JSON.parse(saved);
                game.cr = s.cr || 0;
                game.influence = s.influence || 0;
                game.level = s.level || 1;
                game.nextLevelReq = s.nextLevelReq || 2500;
                
                // Restore owned counts
                if(s.cars) s.cars.forEach((c, i) => { if(game.cars[i]) game.cars[i].owned = c.owned; });
                if(s.sites) s.sites.forEach((site, i) => { if(game.sites[i]) game.sites[i].owned = site.owned; });
                if(s.upgrades) s.upgrades.forEach((u, i) => { if(game.upgrades[i]) game.upgrades[i].owned = u.owned; });
            } catch(e) { console.log('Save corrupt'); }
        }
    }

    function saveGame() {
        // Minify save to just owned counts to save space/logic
        const s = {
            cr: game.cr,
            influence: game.influence,
            level: game.level,
            nextLevelReq: game.nextLevelReq,
            cars: game.cars.map(c => ({ owned: c.owned })),
            sites: game.sites.map(s => ({ owned: s.owned })),
            upgrades: game.upgrades.map(u => ({ owned: u.owned }))
        };
        localStorage.setItem('horizonClickerSave', JSON.stringify(s));
    }

    loadGame();

    /* --- HELPERS --- */
    function formatNumber(num) {
        if (num >= 1e21) return (num / 1e21).toFixed(2) + 'Sx';
        if (num >= 1e18) return (num / 1e18).toFixed(2) + 'Qi';
        if (num >= 1e15) return (num / 1e15).toFixed(2) + 'Qa';
        if (num >= 1e12) return (num / 1e12).toFixed(2) + 'T';
        if (num >= 1e9) return (num / 1e9).toFixed(2) + 'B';
        if (num >= 1e6) return (num / 1e6).toFixed(2) + 'M';
        if (num >= 1000) return (num / 1000).toFixed(1) + 'k';
        return Math.floor(num).toLocaleString();
    }

    function getCost(base, count) {
        return Math.floor(base * Math.pow(1.15, count));
    }

    /* --- GAME LOGIC --- */
    function getMultipliers() {
        let activeMult = 1;
        let passiveMult = 1;
        
        game.upgrades.forEach(u => {
            if (u.owned > 0) {
                if (u.type === 'active') activeMult += (u.multiplier * u.owned);
                if (u.type === 'passive') passiveMult += (u.multiplier * u.owned);
            }
        });
        return { active: activeMult, passive: passiveMult };
    }

    function getClickPower() {
        let power = 0;
        game.cars.forEach(car => {
            power += car.basePower * car.owned;
        });
        return Math.floor(power * getMultipliers().active);
    }

    function getPassiveIncome() {
        let income = 0;
        game.sites.forEach(site => {
            income += site.baseIncome * site.owned;
        });
        return Math.floor(income * getMultipliers().passive);
    }

    function addCredits(amount) {
        game.cr += amount;
        game.influence += (amount * 0.1);
        if (game.influence >= game.nextLevelReq) {
            levelUp();
        }
        updateStatsUI();
    }

    /* --- UI UPDATES --- */
    function updateStatsUI() {
        document.getElementById('cr-display').textContent = formatNumber(game.cr);
        document.getElementById('income-display').textContent = formatNumber(getPassiveIncome());
        document.getElementById('inf-display').textContent = formatNumber(game.influence);
        document.getElementById('level-display').textContent = game.level;
        document.getElementById('wheelspin-notify').textContent = `Next Wheelspin: ${formatNumber(game.nextLevelReq)}`;
    }

    function renderShops() {
        renderShop('autoshow-list', game.cars, buyCar, 'Power');
        renderShop('sites-list', game.sites, buySite, '/s');
        renderShop('upgrades-list', game.upgrades, buyUpgrade, 'Bonus');
    }

    function refreshAllUI() {
        updateStatsUI();
        renderShops();
    }

    function renderShop(elementId, items, buyFn, suffix) {
        const container = document.getElementById(elementId);
        container.innerHTML = '';
        items.forEach((item, index) => {
            const cost = getCost(item.baseCost, item.owned);
            const el = document.createElement('div');
            el.className = `card ${game.cr < cost ? 'disabled' : ''}`;
            if(item.type) el.className += ' upgrade-card'; // Special styling for upgrades
            
            el.onclick = () => { buyFn(index); playClickSound(); };
            
            let statText = "";
            if (item.class) statText = `+${formatNumber(Math.floor(item.basePower * getMultipliers().active))} ${suffix}`;
            else if (item.baseIncome) statText = `+${formatNumber(Math.floor(item.baseIncome * getMultipliers().passive))} ${suffix}`;
            else statText = item.desc;

            let strip = '';
            if (item.class) strip = `<div class="rarity-strip ${item.class}"></div>`;
            else if (item.type) strip = `<div class="rarity-strip" style="background:var(--h-yellow)"></div>`;
            else strip = `<div class="rarity-strip" style="background:var(--h-purple)"></div>`;

            el.innerHTML = `
                ${strip}
                <div class="card-info">
                    <h3>${item.name}</h3>
                    <p>${statText}</p>
                    <div class="card-owned">Owned: ${item.owned}</div>
                </div>
                <div class="card-price">
                    <div><span class="cr-symbol">CR</span>${formatNumber(cost)}</div>
                    <div class="buy-hint">BUY</div>
                </div>
            `;
            container.appendChild(el);
        });
    }

    /* --- INPUTS --- */
    function buyCar(index) {
        const item = game.cars[index];
        const cost = getCost(item.baseCost, item.owned);
        if (game.cr >= cost) {
            game.cr -= cost;
            item.owned++;
            saveGame();
            refreshAllUI();
        }
    }

    function buySite(index) {
        const item = game.sites[index];
        const cost = getCost(item.baseCost, item.owned);
        if (game.cr >= cost) {
            game.cr -= cost;
            item.owned++;
            saveGame();
            refreshAllUI();
        }
    }

    function buyUpgrade(index) {
        const item = game.upgrades[index];
        const cost = getCost(item.baseCost, item.owned);
        if (game.cr >= cost) {
            game.cr -= cost;
            item.owned++;
            saveGame();
            refreshAllUI();
        }
    }

    function clickDrive(e) {
        const amount = Math.max(1, getClickPower());
        addCredits(amount);
        
        let cx = e.clientX || (e.touches && e.touches[0].clientX) || window.innerWidth/2;
        let cy = e.clientY || (e.touches && e.touches[0].clientY) || window.innerHeight/2;
        createFloatingText(cx, cy, `+${formatNumber(amount)}`);
        
        playEngineSound();
        const btn = document.getElementById('drive-btn');
        btn.style.transform = 'scale(0.95)';
        setTimeout(() => btn.style.transform = 'scale(1)', 50);
    }

    /* --- AUDIO & FX --- */
    const AudioContext = window.AudioContext || window.webkitAudioContext;
    const audioCtx = new AudioContext();

    function playEngineSound() {
        if (audioCtx.state === 'suspended') audioCtx.resume();
        const osc = audioCtx.createOscillator();
        const gain = audioCtx.createGain();
        osc.frequency.value = 100 + (Math.random() * 50);
        gain.gain.setValueAtTime(0.1, audioCtx.currentTime);
        gain.gain.exponentialRampToValueAtTime(0.001, audioCtx.currentTime + 0.1);
        osc.connect(gain);
        gain.connect(audioCtx.destination);
        osc.start();
        osc.stop(audioCtx.currentTime + 0.1);
    }

    function playClickSound() {}

    function createFloatingText(x, y, text) {
        const el = document.createElement('div');
        el.className = 'float-text';
        el.style.left = x + 'px';
        el.style.top = y + 'px';
        el.innerText = text;
        document.body.appendChild(el);
        setTimeout(() => el.remove(), 800);
    }

    function levelUp() {
        game.level++;
        game.nextLevelReq = Math.floor(game.nextLevelReq * 1.5);
        saveGame();
        
        const modal = document.getElementById('wheelspin-modal');
        const res = document.getElementById('spin-result');
        const btn = document.getElementById('claim-btn');
        const anim = document.getElementById('spin-animation');
        
        modal.style.display = 'flex';
        res.classList.add('hidden');
        btn.classList.add('hidden');
        anim.classList.remove('hidden');
        
        setTimeout(() => {
            const power = Math.max(100, getClickPower());
            const reward = Math.floor(power * 100 * (Math.random() + 0.5));
            game.cr += reward;
            saveGame();
            
            anim.classList.add('hidden');
            res.textContent = `CR ${formatNumber(reward)}`;
            res.classList.remove('hidden');
            btn.classList.remove('hidden');
            
            btn.onclick = () => {
                modal.style.display = 'none';
                refreshAllUI();
            };
        }, 1500);
    }

    /* --- PANEL TOGGLE --- */
    function togglePanel(id) {
        if (window.innerWidth > 1000) {
            const p = document.getElementById(id);
            if (id === 'panel-upgrades') {
                p.style.display = p.style.display === 'none' ? 'flex' : 'none';
                p.style.position = 'absolute';
                p.style.zIndex = '30';
                p.style.width = '300px';
                p.style.height = '500px';
                p.style.left = '50%';
                p.style.top = '50%';
                p.style.transform = 'translate(-50%, -50%)';
            }
        } else {
            const p = document.getElementById(id);
            document.querySelectorAll('.panel.active').forEach(el => {
                if(el.id !== id) el.classList.remove('active');
            });
            p.style.display = 'flex';
            p.style.position = 'fixed';
            p.style.transform = '';
            p.classList.toggle('active');
        }
    }

    /* --- LOOPS --- */
    setInterval(() => {
        const income = getPassiveIncome();
        if (income > 0) {
            addCredits(income);
        }
        saveGame(); // Auto save every second
    }, 1000);

    refreshAllUI();

    /* --- LISTENERS --- */
    document.getElementById('drive-btn').addEventListener('mousedown', clickDrive);
    document.getElementById('drive-btn').addEventListener('touchstart', (e) => { 
        e.preventDefault(); clickDrive(e.touches[0]); 
    });

</script>
</body>
</html>

