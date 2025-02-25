SWEET LOGO NAMED MARKETLY
<!DOCTYPE html>
<html>
<head>
    <title>Marketing App Logo</title>
    <style>
        .logo-container {
            padding: 40px;
            background: linear-gradient(45deg, #6366f1, #3b82f6);
            border-radius: 20px;
            display: inline-block;
            box-shadow: 0 10px 30px rgba(99, 102, 241, 0.3);
            position: relative;
            overflow: hidden;
        }

        .logo {
            width: 180px;
            height: 180px;
            position: relative;
            animation: float 3s ease-in-out infinite;
        }

        /* Main Logo Symbol */
        .cube {
            position: absolute;
            width: 60px;
            height: 60px;
            background: rgba(255, 255, 255, 0.9);
            transform: rotate(45deg);
            top: 40px;
            left: 60px;
            border-radius: 12px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }

        .cube::before {
            content: '';
            position: absolute;
            width: 100%;
            height: 100%;
            background: rgba(255, 255, 255, 0.6);
            transform: translateX(30px) translateY(-30px) rotate(45deg);
            border-radius: 12px;
        }

        /* Surrounding Elements */
        .nodes {
            position: absolute;
            width: 100%;
            height: 100%;
        }

        .node {
            position: absolute;
            width: 20px;
            height: 20px;
            background: #fff;
            border-radius: 50%;
            animation: pulse 2s infinite;
        }

        .node:nth-child(1) { top: 20px; left: 80px; }
        .node:nth-child(2) { top: 80px; left: 20px; }
        .node:nth-child(3) { top: 80px; right: 20px; }
        .node:nth-child(4) { bottom: 20px; left: 80px; }

        .connections {
            position: absolute;
            width: 100%;
            height: 100%;
            stroke: white;
            stroke-width: 2;
            fill: none;
        }

        /* Text Element */
        .logo-text {
            position: absolute;
            bottom: -25px;
            left: 50%;
            transform: translateX(-50%);
            color: white;
            font-family: 'Arial', sans-serif;
            font-weight: bold;
            font-size: 1.4em;
            text-shadow: 0 2px 4px rgba(0,0,0,0.2);
            letter-spacing: 2px;
            background: linear-gradient(45deg, #fff, #e0e7ff);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        /* Animations */
        @keyframes float {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-10px); }
        }

        @keyframes pulse {
            0%, 100% { transform: scale(1); opacity: 0.8; }
            50% { transform: scale(1.2); opacity: 1; }
        }

        .logo-container::after {
            content: '';
            position: absolute;
            width: 200%;
            height: 200%;
            background: radial-gradient(circle, rgba(255,255,255,0.1) 0%, rgba(255,255,255,0) 70%);
            top: -50%;
            left: -50%;
            animation: glow 4s linear infinite;
        }

        @keyframes glow {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(360deg); }
        }
    </style>
</head>
<body>
    <div class="logo-container">
        <div class="logo">
            <div class="nodes">
                <div class="node"></div>
                <div class="node"></div>
                <div class="node"></div>
                <div class="node"></div>
            </div>
            <svg class="connections">
                <path d="M80 20L100 60L80 100L60 60Z" />
                <path d="M20 80L60 100L100 80L60 60Z" />
            </svg>
            <div class="cube"></div>
            <div class="logo-text">MARKETLY</div>
        </div>
    </div>
</body>
</html>
