# JuniorBlendz
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pre-Order Center</title>
    <style>
        body { font-family: sans-serif; background: #f0f2f5; margin: 0; padding: 20px; display: flex; flex-direction: column; align-items: center; }
        .card { background: white; padding: 30px; border-radius: 12px; box-shadow: 0 4px 12px rgba(0,0,0,0.1); width: 100%; max-width: 400px; margin-bottom: 20px; }
        h2 { margin-top: 0; color: #333; }
        label { display: block; margin-top: 15px; font-weight: bold; color: #555; }
        input { width: 100%; padding: 10px; margin-top: 5px; border: 1px solid #ccc; border-radius: 6px; box-sizing: border-box; }
        button { width: 100%; background: #007bff; color: white; border: none; padding: 12px; margin-top: 20px; border-radius: 6px; font-size: 16px; cursor: pointer; font-weight: bold; }
        button:hover { background: #0056b3; }
        .order-item { background: #f8f9fa; border-left: 4px solid #007bff; padding: 10px; margin-top: 10px; border-radius: 4px; }
    </style>
</head>
<body>

    <!-- The Form to Enter Pre-Orders -->
    <div class="card">
        <h2>Place a Pre-Order</h2>
        <form id="preOrderForm">
            <label for="name">Your Name</label>
            <input type="text" id="name" placeholder="Alex Smith" required>

            <label for="item">Product Item</label>
            <input type="text" id="item" placeholder="Super Widget" required>

            <label for="quantity">How Many?</label>
            <input type="number" id="quantity" value="1" min="1" required>

            <button type="submit">Save Pre-Order</button>
        </form>
    </div>

    <!-- The List Where Pre-Orders Appear Immediately -->
    <div class="card">
        <h2>Saved Pre-Orders</h2>
        <div id="orderList">No pre-orders saved yet.</div>
    </div>

    <!-- Link your logic file -->
    <script src="app.js"></script>
</body>
</html>
