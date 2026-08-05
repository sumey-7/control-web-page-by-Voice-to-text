#control-web-page-by-Voice-to-text

# 🤖 Smart Robot Voice & Control Pad

A smart web-based robot control panel that supports both **traditional buttons** and **Arabic/English voice commands**, directly linked to an **InfinityFree** database to store and update movement states in real-time (`f`, `b`, `l`, `r`, `S`).

---

## 📽️ Project Video Demo
*(Drag and drop your MP4 screen recording file directly here in the GitHub editor, or use the HTML snippet below after uploading the video to your repository)*

```html
<video src="assets/demo.mp4" controls width="100%"></video>
```

📁 Project Structure (5 Essential Files)
These five core files should be uploaded together inside the htdocs directory on your hosting server:

📄 db.php: Database connection script.

🛠️ setup.sql: SQL script to create the robot_state table (executed once in phpMyAdmin).

🔄 update_command.php: Receives commands (from buttons or voice), maps them, and updates the database.

📡 get_state.php: Fetches the current robot state from the database.

---
🎙️ Voice Control Feature (Speech-to-Text)
The system utilizes the browser's native Web Speech API.

Clicking the "🎤 Click & Speak (Voice Command)" button and granting microphone access allows you to speak commands like:

"أمام" or "forward" ➔ mapped to character f (Forward)

"خلف" or "backward" ➔ mapped to character b (Backward)

"يسار" or "left" ➔ mapped to character l (Left)

"يمين" or "right" ➔ mapped to character r (Right)

"قف", "توقف", or "stop" ➔ mapped to character S (Stop)



🌐 index.html: Interactive user interface featuring control buttons and voice recognition.

