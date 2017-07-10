document.body.style.border = "10px solid red";

// Create WebSocket connection.
const socket = new WebSocket('ws://dalle-cort.fr:8080');

socket.send("Hello WebSockets!");

// Connection opened
socket.addEventListener('open', function (event) {
    socket.send('Hello Server!');
});

// Listen for messages
socket.addEventListener('message', function (event) {
    console.log('Message from server', event.data);
});
