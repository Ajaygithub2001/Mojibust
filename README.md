Mojibust 🎉
Mojibust is a simple, interactive web app that allows users to click on emojis to generate a playful animated burst of emojis on the screen. It provides a fun, creative way to interact with emojis, making it perfect for adding a bit of light-hearted fun to your web projects or as a standalone application.

Features ✨
Interactive Emoji Selection: Choose from a wide variety of preloaded emojis.
Animated Emoji Burst: Clicking on an emoji creates a burst of 3–4 animated emojis that move upwards and fade out.
Customizable Interface: Flexible UI elements such as emoji containers and animation behaviors.
Mobile-Friendly Design: Fully responsive design with zoom disabled for a better mobile experience.
No Framework Required: The app is built using pure HTML, CSS, and JavaScript. No dependencies.
Live Demo 🌐
Check out the live demo here! (Add a link if a live demo is available)

Table of Contents
Features
Live Demo
Getting Started
Usage
Customization
Contributing
License
Getting Started 🚀
Prerequisites
Make sure you have the following installed:

A modern web browser (Chrome, Firefox, Safari, etc.)
Installation
Clone the repository:

bash
Copy code
git clone https://github.com/Ajaygithub2001/Mojibust.git
Navigate to the project directory:

bash
Copy code
cd Mojibust
Open index.html in your web browser:

You can simply open the file by double-clicking or right-clicking and choosing the “Open With” option.

Alternatively, run a local server (optional but recommended for advanced users):

bash
Copy code
# For Python users:
python -m http.server
Then visit http://localhost:8000 in your browser.

Usage 🎮
Click an Emoji: Click on any emoji from the emoji container at the bottom of the screen.
Watch the Animation: The emoji you clicked will generate a burst of 3–4 copies that animate upwards and fade out.
Scroll for More Emojis: If there are more emojis than can fit in the view, use the horizontal scroll to see the full selection.
Customization ⚙️
Add or Remove Emojis
You can easily modify the predefined list of emojis by editing the JavaScript section in index.html:

javascript
Copy code
const predefinedEmojis = [
    "😊", "😂", "😍", "🥳", "🤔", "😎", "🤯", // Existing emojis
    "🎂", "🍕", "🍀", "🔥", "🚀" // Add or remove emojis here
];
Modify Animation
The timing and behavior of the emoji animation can be customized by changing the animateEmoji() function:

javascript
Copy code
function animateEmoji(emojiCopy) {
    setTimeout(() => {
        emojiCopy.style.transform = 'translateY(-100vh)'; // Change movement direction or speed
        emojiCopy.style.opacity = '0'; // Adjust fading behavior
    }, 0);
}
Customize Appearance
Modify the CSS to change the appearance of the app, including background color, emoji size, and container styling:

css
Copy code
#emoji-container {
    background-color: #f0f0f0; /* Change this to customize background color */
}

.emoji {
    font-size: 30px; /* Adjust emoji size */
}
Contributing 💡
Contributions are welcome! If you'd like to contribute to Mojibust, follow these steps:

Fork the repository.
Create a new branch (git checkout -b feature/YourFeature).
Make your changes.
Commit your changes (git commit -m 'Add some feature').
Push to the branch (git push origin feature/YourFeature).
Open a pull request.
Please ensure that your changes are well-documented and tested before submitting a pull request.
