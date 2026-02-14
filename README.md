# 🕵️ Silent Leaks - Discord Auth Admin Panel

A premium-styled leak/script database with a secure Discord OAuth2 login system.

## ⚙️ Configuration (Crucial)

### 1. Create a Discord Bot
1. Go to the [Discord Developer Portal](https://discord.com/developers/applications).
2. Click **"New Application"** and give it a name.
3. On the left, click **"OAuth2"** -> **"General"**.
4. In the **"Redirects"** section, click **"Add Redirect"**.
5. Enter: `http://localhost:3000/auth/discord/callback`
6. Click **"Save Changes"**.
7. Copy the **Client ID** and **Client Secret**.

### 2. Setup Environment Variables
1. Open the `.env` file in the project folder.
2. Fill in your credentials:
   ```env
   DISCORD_CLIENT_ID=GIB_HIER_DEINE_CLIENT_ID_EIN
   DISCORD_CLIENT_SECRET=GIB_HIER_DEIN_CLIENT_SECRET_EIN
   DISCORD_CALLBACK_URL=http://localhost:3000/auth/discord/callback
   SESSION_SECRET=waehle_ein_starkes_geheimnis
   ADMIN_IDS=DEINE_DISCORD_ID_HIER,ID2,ID3
   PORT=3000
   ```
   > [!IMPORTANT]
   > Du findest deine Discord ID, indem du den **Developer Mode** in Discord aktiviert hast und rechts auf dein Profil klickst -> **"User ID kopieren"**.

## 🚀 Installation & Start

1. **Install dependencies:**
   ```bash
   npm install
   ```

2. **Start the server:**
   ```bash
   npm start
   ```

3. **Development Mode (Auto-restart):**
   ```bash
   npm run dev
   ```

## 🛠️ Tech Details
- **Backend**: Express.js + Passport.js (Discord Strategy)
- **Frontend**: Vanilla CSS + Glassmorphism + Orbitron Font
- **Icons**: FontAwesome 6

## 📄 License
MIT - Leak it, use it, love it.

Made with 🖤 by Silent.

---

## 🎨 Branding entfernen (Customization)
Wenn du das "Made by Silent" Branding entfernen möchtest:
1. Suche in `index.html` nach dem Text `"MADE BY SILENT"` und `"Made by Silent"`.
2. Entferne die entsprechenden `<div>` Elemente (Zeile ~1095 und am Ende des Dokuments).
3. Suche im CSS nach `.bg-text` und `.watermark`, um die Hintergrund-Effekte zu löschen.
