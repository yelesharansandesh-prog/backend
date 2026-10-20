# backend
const express = require('express');
const app = express();
const PORT = process.env.PORT || 3000;

// Middleware to parse JSON bodies
app.express.json();

// Test route
app.get('/', (req, res) => {
    res.send('Backend is running successfully!');
});

// Start the server
app.listen(PORT, () => {
    console.log(`Server is running on port ${PORT}`);
});