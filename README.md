# 🏝️ Island Battle Royale

A turn-based naval strategy game built with HTML, CSS, JavaScript and Firebase Realtime Database

![Game Banner](https://img.shields.io/badge/status-beta-blue) ![Firebase](https://img.shields.io/badge/Firebase-realtime-orange)

## 🎮 Features

- 🌊 **Build Islands & Deploy Assets** - Place your islands, turrets, and warships
- ⚔️ **Turn-Based Combat** - Attack other players to destroy their fleet
- 🔥 **Bonus System** - Hit enemy islands to gain bonus ammunition
- 👥 **Real-Time Multiplayer** - Uses Firebase for real-time data synchronization

## 🚀 Installation

### 1. Clone Repository

```bash
git clone https://github.com/YOUR_USERNAME/island-battle.git
cd island-battle
```

### 2. Setup Firebase

1. Go to [Firebase Console](https://console.firebase.google.com/)
2. Create a new project
3. Enable **Authentication** > **Anonymous** 
4. Create **Firestore Database** in Test Mode
5. Copy Firebase Config from Project Settings

### 3. Configure Config File

```bash
# Copy the template file
cp firebase-config.template.js firebase-config.js

# Edit firebase-config.js with a text editor
# Paste your Firebase Config
```

**⚠️ Important:** Don't forget to replace the values in `firebase-config.js` with your actual Firebase credentials!

### 4. Launch Game

Open `index.html` with a Web Browser (Chrome, Firefox, or Edge recommended)

```bash
# Or use Live Server if you have VS Code
# Right-click on index.html > Open with Live Server
```

## 📖 How to Play

### Phase 1: Setup
1. Click **Build Land** and create 32 connected island tiles
2. Place 3 turrets on your islands
3. Place 5 warships in the water (sizes: 4, 3, 2, 2, 1)
4. Press **Confirm Layout**

### Phase 2: Battle
1. Select a player to attack
2. Click cells to target (3 shots per round)
3. Press **FIRE** to confirm
4. Wait for other players to finish their turn to see results

## 🎯 Rules

- Hit enemy ship = Direct hit ✅
- Hit enemy island = Bonus +1 ammunition 🎁
- Hit water = Miss ❌
- All ships destroyed = Eliminated 💀

## 🛠️ Technologies

- **Frontend:** HTML5, TailwindCSS, JavaScript (ES6+)
- **Backend:** Firebase Firestore (Realtime Database)
- **Authentication:** Firebase Anonymous Auth
- **Icons:** Font Awesome 6
- **Fonts:** Google Fonts (Kanit)

## 📁 Project Structure

```
island-battle/
├── index.html              # Main game file
├── firebase-config.js      # ⚠️ Secret file (not uploaded to GitHub)
├── firebase-config.template.js  # Template for configuration
├── .gitignore             # Prevents uploading sensitive files
└── README.md              # This documentation
```

## 🔒 Security

- The `firebase-config.js` file **must NOT be uploaded** to GitHub
- Use Firebase Security Rules to protect data access
- Recommended to configure Firebase in Production mode when ready for deployment

## 📝 License

MIT License - Free to use and modify

## 👨‍💻 Developer

Created by **Kritin Kay**

---

🎮 **Enjoy the game!** If you like this project, don't forget to give it a ⭐ Star!
