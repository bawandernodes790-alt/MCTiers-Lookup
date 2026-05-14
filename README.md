<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MCTiers Clone</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

<div class="container">
    <h2>🏆 Minecraft Rankings</h2>
    
    <div class="icon-bar">
        <img src="vanilla.svg" title="Vanilla">
        <img src="smp.svg" title="SMP">
        <img src="sword.svg" title="Sword">
        <img src="mace.svg" title="Mace">
        <img src="uhc.svg" title="UHC">
        <img src="pot.svg" title="Pot">
    </div>

    <table class="leaderboard">
        <thead>
            <tr>
                <th>#</th>
                <th>PLAYER</th>
                <th>REGION</th>
                <th>TIERS</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td class="rank">1.</td>
                <td class="player-info">
                    <img src="https://mc-heads.net/avatar/ItzRealMe/32" alt="Skin">
                    <div class="name-box">
                        <span class="name">ItzRealMe</span>
                        <span class="title">Combat Master</span>
                    </div>
                </td>
                <td><span class="region na">NA</span></td>
                <td class="tiers">
                    <span class="tier ht1">HT1</span>
                    <span class="tier lt2">LT2</span>
                    <img src="hardcoreHeart.svg" class="heart-icon">
                </td>
            </tr>
            
            <tr>
                <td class="rank">2.</td>
                <td class="player-info">
                    <img src="https://mc-heads.net/avatar/coldified/32" alt="Skin">
                    <div class="name-box">
                        <span class="name">coldified</span>
                        <span class="title">Combat Master</span>
                    </div>
                </td>
                <td><span class="region eu">EU</span></td>
                <td class="tiers">
                    <span class="tier lt1">LT1</span>
                    <span class="tier ht3">HT3</span>
                </td>
            </tr>
        </tbody>
    </table>
</div>

</body>
</html>
body {
    background-color: #0f111a;
    color: white;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

.container {
    max-width: 900px;
    margin: 50px auto;
    padding: 20px;
}

/* Icon Navigation */
.icon-bar {
    display: flex;
    gap: 15px;
    background: #1a1d29;
    padding: 10px;
    border-radius: 8px;
    margin-bottom: 20px;
}

.icon-bar img {
    width: 25px;
    cursor: pointer;
    filter: grayscale(1);
    transition: 0.3s;
}

.icon-bar img:hover {
    filter: grayscale(0);
}

/* Table Style */
.leaderboard {
    width: 100%;
    border-collapse: collapse;
    background: #161923;
    border-radius: 10px;
    overflow: hidden;
}

th {
    text-align: left;
    padding: 15px;
    background: #1a1d29;
    font-size: 12px;
    color: #888;
}

td {
    padding: 12px 15px;
    border-bottom: 1px solid #252836;
}

/* Player Section */
.player-info {
    display: flex;
    align-items: center;
    gap: 10px;
}

.player-info img {
    width: 32px;
    height: 32px;
    border-radius: 4px;
}

.name-box .name {
    display: block;
    font-weight: bold;
    font-size: 14px;
}

.name-box .title {
    font-size: 11px;
    color: #ffcc00;
}

/* Regions & Tiers */
.region {
    padding: 2px 6px;
    border-radius: 4px;
    font-size: 10px;
    font-weight: bold;
}

.na { background: #ff4444; }
.eu { background: #44bb44; }

.tier {
    padding: 2px 6px;
    border-radius: 12px;
    font-size: 10px;
    margin-right: 5px;
    font-weight: bold;
}

.ht1 { background: gold; color: black; }
.lt1 { background: #c0c0c0; color: black; }
.lt2 { background: #cd7f32; color: black; }

.heart-icon {
    width: 18px;
    vertical-align: middle;
}
