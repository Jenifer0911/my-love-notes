# 🥰 My Love Notes

A free and private diary web app. Sign up with just your email, write your notes, and keep your secret folders locked.

**Live demo:** https://my-love-notes-jj.netlify.app

## Why I built it
Most diary apps ask you to pay. I wanted one that is free for everyone, with privacy as the main focus.

## Features
- 📁 Colourful folders with your own symbols
- 📝 Write, edit, save and delete notes, with a mood for each note
- 📎 Attach photos and files to notes
- 🔒 Lock a folder with a password. It stays hidden until you type that password in the search bar
- ☁️ Your notes sync between your laptop and phone
- 🎨 Cute, mild dark theme

## Privacy
- Each user can only see their own data (enforced by Firestore security rules).
- Locked folders are encrypted in the browser (AES-GCM, key derived from your password with PBKDF2) before they are saved, so the contents cannot be read in the database.
- If you forget a folder's password, it cannot be recovered.

## Built with
- HTML, CSS, JavaScript
- Firebase Authentication and Cloud Firestore
- Netlify (hosting)
- Built with help from Claude AI. I decided the idea, features and design, and tested and debugged each step.

## Run it yourself
1. Create a Firebase project and enable Email/Password sign-in and Firestore.
2. Paste your own `firebaseConfig` into `index.html`.
3. Add your site's domain under Authentication → Settings → Authorized domains.
4. Publish `index.html` on Netlify or GitHub Pages.

## About me
Jenifer, 3rd year BSc Computer Science student at Sri S. Ramasamy Naidu Memorial College. I enjoy web design, Canva and singing. Feedback is welcome!
