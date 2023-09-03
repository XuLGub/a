<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Chat with GPT</title>
    <style>
        #chat-container {
            width: 400px;
            margin: 0 auto;
            padding: 20px;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
    </style>
</head>
<body>
    <div id="chat-container">
        <h1>Chat with GPT</h1>
        <div id="chat-output" style="height: 200px; overflow-y: scroll;"></div>
        <input type="text" id="user-input" placeholder="Type a message...">
        <button onclick="sendMessage()">Send</button>
    </div>

    <script>
        const chatOutput = document.getElementById('chat-output');
        const userInput = document.getElementById('user-input');

        function sendMessage() {
            const userMessage = userInput.value;
            if (userMessage.trim() === '') return;

            // Display the user's message in the chat
            appendMessage('You', userMessage);

            // Simulate a response from GPT (replace with actual GPT integration)
            const gptResponse = generateGptResponse(userMessage);

            // Display the GPT response in the chat
            appendMessage('GPT', gptResponse);

            // Clear the input box
            userInput.value = '';
        }

        function appendMessage(sender, message) {
            const messageElement = document.createElement('div');
            messageElement.innerHTML = `<strong>${sender}:</strong> ${message}`;
            chatOutput.appendChild(messageElement);

            // Scroll to the bottom of the chat
            chatOutput.scrollTop = chatOutput.scrollHeight;
        }

        function generateGptResponse(userMessage) {
            // Replace this with actual GPT integration or API call
            // For simplicity, this function just echoes the user's message.
            return `You said: ${userMessage}`;
        }
    </script>
</body>
</html>
