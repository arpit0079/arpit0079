<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Best Friend Proposal</title>
    <style>
        body {
            font-family: 'Verdana', sans-serif;
            background-color: #fbd5b5; /* Light Peach */
            color: #333;
            text-align: center;
            margin: 20px;
        }

        h1 {
            color: #e74c3c; /* Alizarin Red */
        }

        p {
            font-size: 18px;
            margin-bottom: 20px;
        }

        img {
            width: 300px;
            border-radius: 50%;
            margin-top: 20px;
        }

        #ring {
            width: 150px;
            margin-top: 20px;
            cursor: pointer;
            animation: bounce 0.8s infinite alternate;
        }

        @keyframes bounce {
            to {
                transform: translateY(-10px);
            }
        }

        #response {
            font-size: 24px;
            font-weight: bold;
            margin-top: 20px;
        }

        #acceptButton {
            background-color: #2ecc71; /* Emerald Green */
            color: #fff;
            padding: 15px 20px;
            font-size: 16px;
            border: none;
            border-radius: 5px;
            transition: background-color 0.3s, transform 0.3s;
        }

        #acceptButton:hover {
            background-color: #27ae60; /* Nephritis */
            transform: scale(1.1);
            cursor: pointer;
        }

        #declineButton {
            background-color: #e74c3c; /* Alizarin Red */
            color: #fff;
            padding: 15px 20px;
            font-size: 16px;
            border: none;
            border-radius: 5px;
            transition: background-color 0.3s, transform 0.3s, margin-top 0.3s;
            pointer-events: none;
        }

        #declineButton:hover {
            background-color: #c0392b; /* Pomegranate */
            transform: translateY(-30px); /* Move the button down further */
            margin-top: 30px; /* Change margin-top to move the button further */
            cursor: not-allowed; /* Disable the cursor */
        }
    </style>
</head>

<body>
    <h1>Best Friend Forever Proposal</h1>
    <p>Dear Aashie ,</p>
    <p>Our friendship is like a rare gem, and I want to cherish it forever. Will you be my partner in crime, my confidant, and officially my best friend forever? Let's make this official!</p>
    <img src="Snapchat-1026496589.jpg" alt="" width="300px">
    <br>
    <img id="Ring" src="best_friend_ring.png" alt="Best Friend Ring">
    <div id="response"></div>

    <script>
        var responseDiv = document.getElementById('response');

        function acceptProposal() {
            responseDiv.innerHTML = "Absolutely! I'm thrilled to be your best friend forever! 🎉💖";
            responseDiv.style.color = '#2ecc71'; /* Emerald Green */
        }

        function declineProposal() {
            responseDiv.innerHTML = "I appreciate it, but let's keep our awesome friendship as it is! 😊";
            responseDiv.style.color = '#3498db'; /* Dodger Blue */
        }
    </script>

    <button id="acceptButton" onclick="acceptProposal()">Accept Proposal</button>
    <button id="declineButton" onclick="declineProposal()">Decline Proposal</button>
</body>

</html>

