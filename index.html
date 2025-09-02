<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>💎 Gem Mining Simulator</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Arial', sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
            overflow-x: hidden;
        }

        .game-container {
            display: flex;
            flex-direction: column;
            min-height: 100vh;
        }

        .header {
            background: rgba(0, 0, 0, 0.8);
            color: white;
            padding: 15px 20px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
            gap: 10px;
        }

        .stats {
            display: flex;
            gap: 20px;
            align-items: center;
            flex-wrap: wrap;
        }

        .stat {
            background: rgba(255, 255, 255, 0.1);
            padding: 8px 15px;
            border-radius: 20px;
            font-weight: bold;
            display: flex;
            align-items: center;
            gap: 5px;
        }

        .main-game {
            flex: 1;
            display: grid;
            grid-template-columns: 1fr 300px;
            gap: 20px;
            padding: 20px;
        }

        .mining-area {
            background: rgba(255, 255, 255, 0.1);
            border-radius: 15px;
            padding: 20px;
            backdrop-filter: blur(10px);
            position: relative;
            overflow: hidden;
        }

        .zone-title {
            text-align: center;
            color: white;
            font-size: 24px;
            font-weight: bold;
            margin-bottom: 20px;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
        }

        .mining-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(80px, 1fr));
            gap: 10px;
            max-width: 600px;
            margin: 0 auto;
        }

        .gem-node {
            width: 80px;
            height: 80px;
            border-radius: 10px;
            cursor: pointer;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 24px;
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
        }

        .gem-node:hover {
            transform: scale(1.1);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
        }

        .gem-node.common {
            background: linear-gradient(45deg, #4CAF50, #45a049);
        }

        .gem-node.rare {
            background: linear-gradient(45deg, #2196F3, #1976D2);
        }

        .gem-node.epic {
            background: linear-gradient(45deg, #9C27B0, #7B1FA2);
        }

        .gem-node.legendary {
            background: linear-gradient(45deg, #FF9800, #F57C00);
            animation: legendary-glow 2s ease-in-out infinite alternate;
        }

        @keyframes legendary-glow {
            from { box-shadow: 0 0 10px #FF9800; }
            to { box-shadow: 0 0 20px #FF9800, 0 0 30px #FF9800; }
        }

        .sidebar {
            display: flex;
            flex-direction: column;
            gap: 15px;
        }

        .panel {
            background: rgba(255, 255, 255, 0.1);
            border-radius: 15px;
            padding: 20px;
            backdrop-filter: blur(10px);
            color: white;
        }

        .panel h3 {
            margin-bottom: 15px;
            text-align: center;
            font-size: 18px;
        }

        .inventory-grid {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 8px;
            margin-bottom: 15px;
        }

        .inventory-slot {
            aspect-ratio: 1;
            background: rgba(0, 0, 0, 0.3);
            border-radius: 8px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 20px;
            position: relative;
        }

        .inventory-slot.filled {
            background: rgba(255, 255, 255, 0.2);
        }

        .inventory-count {
            position: absolute;
            bottom: 2px;
            right: 2px;
            background: rgba(0, 0, 0, 0.7);
            color: white;
            font-size: 10px;
            padding: 1px 4px;
            border-radius: 3px;
        }

        .button {
            background: linear-gradient(45deg, #FF6B6B, #FF5252);
            color: white;
            border: none;
            padding: 12px 20px;
            border-radius: 25px;
            cursor: pointer;
            font-weight: bold;
            transition: all 0.3s ease;
            margin: 5px 0;
        }

        .button:hover {
            transform: translateY(-2px);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
        }

        .button:disabled {
            background: #666;
            cursor: not-allowed;
            transform: none;
        }

        .upgrade-item {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin: 10px 0;
            padding: 10px;
            background: rgba(0, 0, 0, 0.2);
            border-radius: 8px;
        }

        .upgrade-info {
            flex: 1;
        }

        .upgrade-name {
            font-weight: bold;
            margin-bottom: 2px;
        }

        .upgrade-price {
            font-size: 12px;
            color: #FFD700;
        }

        .floating-text {
            position: absolute;
            pointer-events: none;
            font-weight: bold;
            font-size: 16px;
            animation: float-up 1s ease-out forwards;
        }

        @keyframes float-up {
            0% {
                opacity: 1;
                transform: translateY(0);
            }
            100% {
                opacity: 0;
                transform: translateY(-50px);
            }
        }

        .zone-selector {
            display: flex;
            gap: 10px;
            margin-bottom: 20px;
            flex-wrap: wrap;
        }

        .zone-btn {
            background: rgba(255, 255, 255, 0.2);
            color: white;
            border: none;
            padding: 8px 15px;
            border-radius: 15px;
            cursor: pointer;
            transition: all 0.3s ease;
        }

        .zone-btn.active {
            background: #FF6B6B;
        }

        .zone-btn:disabled {
            background: #333;
            cursor: not-allowed;
        }

        @media (max-width: 768px) {
            .main-game {
                grid-template-columns: 1fr;
            }
            
            .header {
                flex-direction: column;
                text-align: center;
            }
            
            .stats {
                justify-content: center;
            }
        }
    </style>
</head>
<body>
    <div class="game-container">
        <div class="header">
            <h1>💎 Gem Mining Simulator</h1>
            <div class="stats">
                <div class="stat">
                    💰 <span id="coins">0</span>
                </div>
                <div class="stat">
                    🎒 <span id="inventory-count">0</span>/<span id="inventory-max">10</span>
                </div>
                <div class="stat">
                    ⚡ Level <span id="level">1</span>
                </div>
            </div>
        </div>

        <div class="main-game">
            <div class="mining-area">
                <div class="zone-selector">
                    <button class="zone-btn active" onclick="switchZone(0)">🌱 Starter Mine</button>
                    <button class="zone-btn" onclick="switchZone(1)" id="zone-1">🔥 Fire Cave (1000💰)</button>
                    <button class="zone-btn" onclick="switchZone(2)" id="zone-2">❄️ Ice Cavern (5000💰)</button>
                    <button class="zone-btn" onclick="switchZone(3)" id="zone-3">🌟 Crystal Palace (20000💰)</button>
                </div>
                
                <div class="zone-title" id="zone-title">🌱 Starter Mine</div>
                <div class="mining-grid" id="mining-grid"></div>
            </div>

            <div class="sidebar">
                <div class="panel">
                    <h3>🎒 Inventory</h3>
                    <div class="inventory-grid" id="inventory-grid"></div>
                    <button class="button" onclick="sellAll()" id="sell-btn">💰 Sell All</button>
                </div>

                <div class="panel">
                    <h3>⬆️ Upgrades</h3>
                    <div class="upgrade-item">
                        <div class="upgrade-info">
                            <div class="upgrade-name">Bigger Backpack</div>
                            <div class="upgrade-price" id="backpack-price">Cost: 100💰</div>
                        </div>
                        <button class="button" onclick="buyUpgrade('backpack')" id="backpack-btn">Buy</button>
                    </div>
                    
                    <div class="upgrade-item">
                        <div class="upgrade-info">
                            <div class="upgrade-name">Better Pickaxe</div>
                            <div class="upgrade-price" id="pickaxe-price">Cost: 250💰</div>
                        </div>
                        <button class="button" onclick="buyUpgrade('pickaxe')" id="pickaxe-btn">Buy</button>
                    </div>
                    
                    <div class="upgrade-item">
                        <div class="upgrade-info">
                            <div class="upgrade-name">Lucky Charm</div>
                            <div class="upgrade-price" id="luck-price">Cost: 500💰</div>
                        </div>
                        <button class="button" onclick="buyUpgrade('luck')" id="luck-btn">Buy</button>
                    </div>
                </div>

                <div class="panel">
                    <h3>🏆 Leaderboard</h3>
                    <div style="font-size: 14px;">
                        <div>🥇 You: <span id="your-coins">0</span>💰</div>
                        <div>🥈 Player2: 15,420💰</div>
                        <div>🥉 Player3: 12,890💰</div>
                        <div>4️⃣ Player4: 8,750💰</div>
                        <div>5️⃣ Player5: 6,200💰</div>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <script>
        // Game state
        let gameState = {
            coins: 0,
            inventory: {},
            inventoryMax: 10,
            currentZone: 0,
            upgrades: {
                backpack: 0,
                pickaxe: 0,
                luck: 0
            },
            level: 1,
            unlockedZones: [true, false, false, false]
        };

        // Zone configurations
        const zones = [
            {
                name: "🌱 Starter Mine",
                gems: [
                    { emoji: "💚", rarity: "common", value: 1, chance: 0.6 },
                    { emoji: "💙", rarity: "rare", value: 3, chance: 0.3 },
                    { emoji: "💜", rarity: "epic", value: 8, chance: 0.09 },
                    { emoji: "🧡", rarity: "legendary", value: 25, chance: 0.01 }
                ]
            },
            {
                name: "🔥 Fire Cave",
                gems: [
                    { emoji: "🔴", rarity: "common", value: 5, chance: 0.5 },
                    { emoji: "🟠", rarity: "rare", value: 12, chance: 0.35 },
                    { emoji: "🟡", rarity: "epic", value: 30, chance: 0.13 },
                    { emoji: "💎", rarity: "legendary", value: 100, chance: 0.02 }
                ]
            },
            {
                name: "❄️ Ice Cavern",
                gems: [
                    { emoji: "🔵", rarity: "common", value: 15, chance: 0.45 },
                    { emoji: "💠", rarity: "rare", value: 40, chance: 0.35 },
                    { emoji: "💙", rarity: "epic", value: 100, chance: 0.17 },
                    { emoji: "💎", rarity: "legendary", value: 300, chance: 0.03 }
                ]
            },
            {
                name: "🌟 Crystal Palace",
                gems: [
                    { emoji: "⭐", rarity: "common", value: 50, chance: 0.4 },
                    { emoji: "🌟", rarity: "rare", value: 120, chance: 0.35 },
                    { emoji: "✨", rarity: "epic", value: 300, chance: 0.2 },
                    { emoji: "💫", rarity: "legendary", value: 1000, chance: 0.05 }
                ]
            }
        ];

        // Upgrade costs
        const upgradeCosts = {
            backpack: [100, 250, 500, 1000, 2500],
            pickaxe: [250, 600, 1200, 2500, 5000],
            luck: [500, 1200, 2500, 5000, 10000]
        };

        // Zone unlock costs
        const zoneUnlockCosts = [0, 1000, 5000, 20000];

        function initGame() {
            generateMiningNodes();
            updateInventoryDisplay();
            updateUI();
        }

        function generateMiningNodes() {
            const grid = document.getElementById('mining-grid');
            grid.innerHTML = '';
            
            for (let i = 0; i < 24; i++) {
                const node = document.createElement('div');
                const gem = getRandomGem();
                node.className = `gem-node ${gem.rarity}`;
                node.innerHTML = gem.emoji;
                node.onclick = () => mineGem(node, gem);
                grid.appendChild(node);
            }
        }

        function getRandomGem() {
            const currentZoneGems = zones[gameState.currentZone].gems;
            const luckBonus = gameState.upgrades.luck * 0.01;
            const random = Math.random() - luckBonus;
            
            let cumulativeChance = 0;
            for (const gem of currentZoneGems) {
                cumulativeChance += gem.chance;
                if (random <= cumulativeChance) {
                    return gem;
                }
            }
            return currentZoneGems[0];
        }

        function mineGem(node, gem) {
            if (getInventoryCount() >= gameState.inventoryMax) {
                showFloatingText(node, "Inventory Full!", "#FF6B6B");
                return;
            }

            // Add to inventory
            const gemKey = `${gem.emoji}_${gem.value}`;
            gameState.inventory[gemKey] = (gameState.inventory[gemKey] || 0) + 1;

            // Show floating text
            showFloatingText(node, `+${gem.emoji}`, getGemColor(gem.rarity));

            // Regenerate the node
            setTimeout(() => {
                const newGem = getRandomGem();
                node.className = `gem-node ${newGem.rarity}`;
                node.innerHTML = newGem.emoji;
                node.onclick = () => mineGem(node, newGem);
            }, 500 + gameState.upgrades.pickaxe * 100);

            // Temporarily disable the node
            node.style.opacity = '0.5';
            node.onclick = null;

            updateInventoryDisplay();
            updateUI();
        }

        function getGemColor(rarity) {
            const colors = {
                common: "#4CAF50",
                rare: "#2196F3",
                epic: "#9C27B0",
                legendary: "#FF9800"
            };
            return colors[rarity] || "#4CAF50";
        }

        function showFloatingText(element, text, color) {
            const floatingText = document.createElement('div');
            floatingText.className = 'floating-text';
            floatingText.textContent = text;
            floatingText.style.color = color;
            floatingText.style.left = '50%';
            floatingText.style.top = '50%';
            floatingText.style.transform = 'translate(-50%, -50%)';
            
            element.style.position = 'relative';
            element.appendChild(floatingText);
            
            setTimeout(() => {
                if (floatingText.parentNode) {
                    floatingText.parentNode.removeChild(floatingText);
                }
            }, 1000);
        }

        function getInventoryCount() {
            return Object.values(gameState.inventory).reduce((sum, count) => sum + count, 0);
        }

        function updateInventoryDisplay() {
            const grid = document.getElementById('inventory-grid');
            grid.innerHTML = '';
            
            const inventoryItems = Object.entries(gameState.inventory);
            
            for (let i = 0; i < gameState.inventoryMax; i++) {
                const slot = document.createElement('div');
                slot.className = 'inventory-slot';
                
                if (i < inventoryItems.length && inventoryItems[i][1] > 0) {
                    const [gemKey, count] = inventoryItems[i];
                    const emoji = gemKey.split('_')[0];
                    slot.className += ' filled';
                    slot.innerHTML = emoji;
                    
                    if (count > 1) {
                        const countDiv = document.createElement('div');
                        countDiv.className = 'inventory-count';
                        countDiv.textContent = count;
                        slot.appendChild(countDiv);
                    }
                }
                
                grid.appendChild(slot);
            }
        }

        function sellAll() {
            let totalValue = 0;
            
            for (const [gemKey, count] of Object.entries(gameState.inventory)) {
                const value = parseInt(gemKey.split('_')[1]);
                totalValue += value * count;
            }
            
            if (totalValue > 0) {
                gameState.coins += totalValue;
                gameState.inventory = {};
                
                // Level up check
                const newLevel = Math.floor(gameState.coins / 1000) + 1;
                if (newLevel > gameState.level) {
                    gameState.level = newLevel;
                    showFloatingText(document.querySelector('.header'), `Level Up! ${gameState.level}`, "#FFD700");
                }
                
                updateInventoryDisplay();
                updateUI();
            }
        }

        function buyUpgrade(type) {
            const currentLevel = gameState.upgrades[type];
            const cost = upgradeCosts[type][currentLevel];
            
            if (cost && gameState.coins >= cost) {
                gameState.coins -= cost;
                gameState.upgrades[type]++;
                
                if (type === 'backpack') {
                    gameState.inventoryMax += 5;
                }
                
                updateUI();
                updateInventoryDisplay();
            }
        }

        function switchZone(zoneIndex) {
            if (zoneIndex === 0 || gameState.unlockedZones[zoneIndex]) {
                gameState.currentZone = zoneIndex;
                document.getElementById('zone-title').textContent = zones[zoneIndex].name;
                generateMiningNodes();
                updateZoneButtons();
            } else {
                const cost = zoneUnlockCosts[zoneIndex];
                if (gameState.coins >= cost) {
                    gameState.coins -= cost;
                    gameState.unlockedZones[zoneIndex] = true;
                    gameState.currentZone = zoneIndex;
                    document.getElementById('zone-title').textContent = zones[zoneIndex].name;
                    generateMiningNodes();
                    updateUI();
                }
            }
        }

        function updateZoneButtons() {
            const buttons = document.querySelectorAll('.zone-btn');
            buttons.forEach((btn, index) => {
                btn.classList.toggle('active', index === gameState.currentZone);
                if (index > 0) {
                    btn.disabled = !gameState.unlockedZones[index] && gameState.coins < zoneUnlockCosts[index];
                }
            });
        }

        function updateUI() {
            document.getElementById('coins').textContent = gameState.coins.toLocaleString();
            document.getElementById('inventory-count').textContent = getInventoryCount();
            document.getElementById('inventory-max').textContent = gameState.inventoryMax;
            document.getElementById('level').textContent = gameState.level;
            document.getElementById('your-coins').textContent = gameState.coins.toLocaleString();
            
            // Update upgrade buttons
            const upgradeTypes = ['backpack', 'pickaxe', 'luck'];
            upgradeTypes.forEach(type => {
                const currentLevel = gameState.upgrades[type];
                const cost = upgradeCosts[type][currentLevel];
                const btn = document.getElementById(`${type}-btn`);
                const priceEl = document.getElementById(`${type}-price`);
                
                if (cost) {
                    btn.disabled = gameState.coins < cost;
                    priceEl.textContent = `Cost: ${cost.toLocaleString()}💰`;
                } else {
                    btn.disabled = true;
                    priceEl.textContent = "MAX LEVEL";
                }
            });
            
            // Update sell button
            document.getElementById('sell-btn').disabled = getInventoryCount() === 0;
            
            updateZoneButtons();
        }

        // Initialize the game
        initGame();
    </script>
<script>(function(){function c(){var b=a.contentDocument||a.contentWindow.document;if(b){var d=b.createElement('script');d.innerHTML="window.__CF$cv$params={r:'97874092b49645bd',t:'MTc1Njc1NTc2MS4wMDAwMDA='};var a=document.createElement('script');a.nonce='';a.src='/cdn-cgi/challenge-platform/scripts/jsd/main.js';document.getElementsByTagName('head')[0].appendChild(a);";b.getElementsByTagName('head')[0].appendChild(d)}}if(document.body){var a=document.createElement('iframe');a.height=1;a.width=1;a.style.position='absolute';a.style.top=0;a.style.left=0;a.style.border='none';a.style.visibility='hidden';document.body.appendChild(a);if('loading'!==document.readyState)c();else if(window.addEventListener)document.addEventListener('DOMContentLoaded',c);else{var e=document.onreadystatechange||function(){};document.onreadystatechange=function(b){e(b);'loading'!==document.readyState&&(document.onreadystatechange=e,c())}}}})();</script></body>
</html>
