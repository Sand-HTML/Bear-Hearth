<html>

<head>
    <title>Beating Heart</title>
    <style>
        @keyframes beat {
            0% {
                transform: scale(1);
            }

            50% {
                transform: scale(1.1);
            }

            100% {
                transform: scale(1);
            }
        }

        .heart {
            position: relative;
            width: 600px;
            height: 540px;
            animation: beat 1s infinite;
            margin: auto;
            top: 20%;
            transform: translateY(-50%);
        }

        .heart:before,
        .heart:after {
            position: absolute;
            content: "";
            left: 300px;
            top: 0;
            width: 300px;
            height: 480px;
            background: red;
            border-radius: 50px 50px 0 0;
            transform: rotate(-45deg);
            transform-origin: 0 100%;
        }

        .heart:after {
            left: 0;
            transform: rotate(45deg);
            transform-origin: 100% 100%;
        }

        body {
            background-color: #000;
            /* Dark background */
            display: flex;
            align-items: center;
            justify-content: center;
            height: 100vh;
        }

        .heart p {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            /* Center the text inside the heart */
            font-size: 20px;
            color: white;
            text-align: center;
        }
    </style>
</head>

<body>
    <div class="heart">
        <p>VERONICA</p>
    </div>
</body>

</html>
