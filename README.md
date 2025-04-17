# Voice-Controlled Email Sender 🗣️📧

This Python project lets you **send emails using your voice**! It uses **speech recognition** to take the recipient's name and message, and **text-to-speech** to respond during the interaction.

## 🔧 Features

- 🎤 Voice input for both recipient and message
- 🔊 Spoken feedback using text-to-speech
- 📧 Email sending via Gmail SMTP
- 📚 Custom contact mapping

---

## 🚀 Getting Started

### 📦 Requirements

Make sure you have the following Python libraries installed:

```bash
pip install speechrecognition pyttsx3 pyaudio
```

> ⚠️ `PyAudio` might require additional setup depending on your OS. On Windows, try:
> ```bash
> pip install pipwin
> pipwin install pyaudio
> ```

---

## ✨ Usage

1. **Clone this repo** or download the script.

2. **Update email credentials** in the `send_email()` function:
   ```python
   sender_email = "youremail@gmail.com"
   sender_password = "yourapppassword"
   ```
   > 💡 Use an [App Password](https://support.google.com/accounts/answer/185833?hl=en) instead of your actual password for Gmail accounts.

3. **Edit contact mappings** in the `emails` dictionary:
   ```python
   emails = {
       "myself": "yourfriend@gmail.com"
   }
   ```

4. **Run the script:**
   ```bash
   python voice_email_sender.py
   ```

---

## 🧠 How It Works

1. The program asks who you want to email.
2. It listens to your voice and maps the name to an email.
3. It then asks for the message.
4. Once the message is captured, it sends the email and confirms the action.

---

## 🛡️ Disclaimer

This tool is a fun, voice-based utility. Do not use it for sensitive information or spam. Email credentials are stored in plain text—use responsibly.

---

## 📌 To Do

- [ ] Add email subject line support
- [ ] Confirm message before sending
- [ ] Store contacts in a separate JSON file
- [ ] Add GUI interface

---

## 🧑‍💻 Author

Made with 💙 by [Your Name]

---

## 📜 License

This project is licensed under the MIT License.
