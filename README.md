<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Fully Animated ASCII Art Dog</title>
    <style>
        body {
            font-family: monospace;
            text-align: center;
            margin-top: 20px;
            background-color: #f5f5f5;
        }
        pre {
            display: inline-block;
            background: #fff;
            padding: 30px;
            border: 1px solid #ccc;
            border-radius: 10px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            font-size: 1.2em;
            line-height: 1.5;
            position: relative;
            animation: bobbing 1.5s infinite;
        }

        .tail {
            display: inline-block;
            animation: wag 0.5s infinite alternate;
        }

        .eye {
            display: inline-block;
            animation: blink 3s infinite;
        }

        @keyframes wag {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(20deg); }
        }

        @keyframes blink {
            0%, 90% { content: "o"; }
            91%, 100% { content: "-"; }
        }

        @keyframes bobbing {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-5px); }
        }
    </style>
</head>
<body>
    <h1>Fully Animated ASCII Art Dog</h1>
    <pre>
         / \__
        (    <span class="eye">o</span>\___
        /         O
       /   (_______)
      /_____/
           <span class="tail">U</span>
    </pre>
</body>
</html>
