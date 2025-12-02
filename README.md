# 💬 Telegram Web Clone – Modern Chat Interface

<div align="center">

![Version](https://img.shields.io/badge/Version-1.0.0-blue)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6-F7DF1E?logo=javascript)
![Responsive](https://img.shields.io/badge/Design-Responsive-green)
![License](https://img.shields.io/badge/License-MIT-green)

**A pixel-perfect, fully functional Telegram Web interface clone with real-time messaging, smooth animations, and authentic dark theme design — built with pure HTML, CSS & JavaScript.**

[Features](#-features) • [Demo](#-live-demo) • [Architecture](#-architecture) • [Setup](#-quick-start) • [Screenshots](#-screenshots) • [Author](#-author)

</div>

---

![Telegram Clone Preview](https://img.shields.io/badge/Preview-Live-success?style=for-the-badge)

---

## 🚀 Overview

This project is a **high-fidelity Telegram Web frontend clone** that replicates the beloved messaging platform's interface and user experience.

Built from scratch without any frameworks, this demonstrates:

✔ **Authentic UI/UX** – Matches Telegram's signature dark theme  
✔ **Real-time Messaging** – Send and receive messages instantly  
✔ **Smooth Animations** – Fade-in effects and hover transitions  
✔ **Chat Management** – Multiple conversations with active states  
✔ **Responsive Design** – Optimized for desktop viewing  
✔ **Zero Dependencies** – Pure vanilla JavaScript  

Perfect for learning modern web development, UI design patterns, or as a foundation for custom chat applications.

---

## 🎯 Primary Goal (MVP)

### **Functional Telegram-Style Chat Interface**

Your Telegram clone includes:

### 💬 **1. Dual-Panel Layout**

* **Left Sidebar** – Chat list with search functionality
* **Right Panel** – Active conversation view
* Clean separation with authentic styling

### 🎨 **2. Authentic Telegram Design**

* **Dark Theme** – Signature blue-gray color scheme
* **Typography** – System fonts matching native apps
* **Spacing** – Pixel-perfect padding and margins
* **Icons** – Emoji-based placeholders for quick loading

### ⚡ **3. Interactive Features**

* Click chats to switch conversations
* Type and send messages with Enter key
* Automatic timestamp generation
* Smooth scroll behavior
* Hover effects on interactive elements

---

## 🌟 Key Features Implemented

### 📱 **Chat Sidebar**

```javascript
✓ Search bar with icon
✓ Scrollable chat list
✓ Avatar with gradient backgrounds
✓ Last message preview
✓ Timestamp display
✓ Active chat highlighting
✓ Hover states
```

### 💬 **Message View**

```javascript
✓ Chat header with user info
✓ Scrollable message area
✓ Sent/Received message bubbles
✓ Different alignment for sent/received
✓ Timestamp on each message
✓ Smooth fade-in animations
```

### ⌨️ **Input Area**

```javascript
✓ Attachment button
✓ Auto-expanding text input
✓ Send button with hover effect
✓ Enter key to send
✓ Real-time message rendering
```

---

## ⭐ Features

### ✔ No Framework Dependencies (Pure JavaScript)

### ✔ Pixel-Perfect Telegram UI

### ✔ Real-Time Message Rendering

### ✔ Smooth CSS Animations

### ✔ Custom Scrollbar Styling

### ✔ Keyboard Shortcuts (Enter to Send)

### ✔ Multiple Chat Support

### ✔ Responsive Hover Effects

---

## 🎮 User Experience

Example interaction flow:

> 👤 **User clicks "John Doe" in chat list**

> 🎨 **Chat becomes highlighted with blue background**

> 📝 **User types: "Hey, how's it going?"**

> ⌨️ **User presses Enter**

> 💬 **Message appears instantly with timestamp**

> ⚡ **Message animates in with fade effect**

> 📜 **Chat scrolls to latest message automatically**

---

## 🛠️ Tech Stack

* **HTML5** – Semantic structure
* **CSS3** – Flexbox, animations, gradients
* **Vanilla JavaScript** – DOM manipulation
* **No Libraries** – Zero external dependencies
* **Custom Scrollbar** – Webkit styling
* **SVG Patterns** – Background textures

---

## 📁 Project Structure

```
/telegram-frontend
│
├── index.html          # Main HTML structure
├── styles.css          # All styling (embedded)
├── script.js           # Message handling logic (embedded)
├── README.md           # This file
│
└── assets/             # (Optional) External resources
    ├── screenshots/
    └── demo/
```

---

## ⚙️ Quick Start

### **1. Clone the Repository**

```bash
git clone https://github.com/yourusername/telegram-frontend-clone
cd telegram-frontend-clone
```

### **2. Open in Browser**

Simply open `index.html` in any modern browser:

```bash
# On macOS
open index.html

# On Linux
xdg-open index.html

# On Windows
start index.html
```

Or use a local server:

```bash
# Python 3
python -m http.server 8000

# Node.js (with http-server)
npx http-server
```

### **3. Start Chatting!**

* Click different chats in the sidebar
* Type messages in the input box
* Press Enter or click send button
* Watch messages appear in real-time

---

## 🎨 Color Palette

```css
Primary Background:    #0e1621
Secondary Background:  #17212b
Sidebar Background:    #212d3b
Active Chat:           #2b5278
Text Primary:          #ffffff
Text Secondary:        #8b98a5
Border:                #0f1419
```

---

## 📸 Screenshots

### Chat List View
![Chat Sidebar](https://via.placeholder.com/400x600/212d3b/ffffff?text=Chat+List)

### Active Conversation
![Message View](https://via.placeholder.com/800x600/0e1621/ffffff?text=Chat+View)

### Message Input
![Input Area](https://via.placeholder.com/800x100/17212b/ffffff?text=Message+Input)

---

## 💡 Code Highlights

### Send Message Function

```javascript
function sendMessage() {
    const text = messageInput.value.trim();
    if (text === '') return;

    const now = new Date();
    const time = now.getHours().toString().padStart(2, '0') + ':' + 
                now.getMinutes().toString().padStart(2, '0');

    const messageDiv = document.createElement('div');
    messageDiv.className = 'message sent';
    messageDiv.innerHTML = `
        <div class="message-content">
            <div class="message-text">${text}</div>
            <div class="message-time">${time}</div>
        </div>
    `;

    messagesContainer.appendChild(messageDiv);
    messagesContainer.scrollTop = messagesContainer.scrollHeight;
    messageInput.value = '';
}
```

### Smooth Animations

```css
@keyframes fadeIn {
    from { 
        opacity: 0; 
        transform: translateY(10px); 
    }
    to { 
        opacity: 1; 
        transform: translateY(0); 
    }
}

.message {
    animation: fadeIn 0.3s;
}
```

---

## 🎥 Live Demo

📎 [View Live Demo](#) *(Add your deployment link)*

Or watch the video demo:

[![Demo Video](https://img.shields.io/badge/▶️-Watch%20Demo-red?style=for-the-badge)](https://your-demo-link.com)

---

## 🔮 Future Enhancements

### Phase 1 (UI Improvements)
- [ ] Add emoji picker
- [ ] File upload functionality
- [ ] Voice message recording
- [ ] Image/video preview
- [ ] Typing indicators

### Phase 2 (Features)
- [ ] Message editing/deletion
- [ ] Reply functionality
- [ ] Search in messages
- [ ] User status (online/offline)
- [ ] Unread message badges

### Phase 3 (Backend Integration)
- [ ] WebSocket real-time sync
- [ ] User authentication
- [ ] Message persistence
- [ ] Multi-device support
- [ ] End-to-end encryption

### Phase 4 (Advanced)
- [ ] Group chats
- [ ] Channel broadcasts
- [ ] Voice/video calls
- [ ] Stories feature
- [ ] Bot integration

---

## 🤝 Contributing

Contributions are welcome! Here's how:

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

* Inspired by [Telegram Web](https://web.telegram.org)
* Design principles from Telegram's official interface
* Built as a learning project for modern web development

---

## 👨‍💻 Author

**Om Gedam**  
GitHub: **[@itsomg134](https://github.com/itsomg134)**  
Email: **omgedam123098@gmail.com**  
X (Twitter): **[@omgedam](https://twitter.com/omgedam)**  
LinkedIn: **[Om Gedam](https://linkedin.com/in/om-gedam)**  
Portfolio: **[https://ogworks.lovable.app](https://ogworks.lovable.app)**

Built with 💙 Telegram inspiration + ⚡ Pure Web Technologies

---

## 📊 Stats

![GitHub stars](https://img.shields.io/github/stars/yourusername/telegram-frontend-clone?style=social)
![GitHub forks](https://img.shields.io/github/forks/yourusername/telegram-frontend-clone?style=social)
![GitHub watchers](https://img.shields.io/github/watchers/yourusername/telegram-frontend-clone?style=social)

---

<div align="center">

**If you found this project helpful, please consider giving it a ⭐!**

[⬆ Back to Top](#-telegram-web-clone--modern-chat-interface)

</div>
