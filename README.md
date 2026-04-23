Technologies Used in This Project
The CLASSIFIED Data Monitoring System is a fully client-side web application. Below are the core technologies and libraries used:

Core Web Technologies
HTML5 – Document structure, semantic elements, form inputs, file upload, modals.

CSS3 – Custom styling with CSS variables (light/dark theme), flexbox, grid, glassmorphism (backdrop-filter), keyframe animations, responsive media queries.

JavaScript (ES6+) – All application logic, including authentication, data management, DOM manipulation, event handling, and asynchronous operations (Promises, async/await).

Fonts & Icons
Google Fonts – Inter (sans‑serif) and JetBrains Mono (monospace) for typography.

Font Awesome 6 (Free CDN) – Icons for UI elements (buttons, alerts, attachments, etc.).

Charting & Data Visualization
Chart.js 4.4.0 – Renders a dynamic bar chart showing threat level distribution (Low, Medium, High, Critical).

PDF Generation
html2pdf.js 0.10.1 – Converts the organisation table to a downloadable PDF report (uses html2canvas + jsPDF internally).

Cryptography
CryptoJS 4.2.0 – Implements AES encryption/decryption for the secure messaging module (messages stored encrypted in localStorage).

Client‑Side Storage
Web Storage API – localStorage for persisting organisation data, audit logs, encrypted messages, and automatic backups; sessionStorage for maintaining user login state across page reloads.

File Handling
FileReader API – Reads uploaded attachments (images, PDFs, text files, audio) as Base64 data URLs for storage and preview.

Blob API & URL.createObjectURL – Enables exporting JSON/CSV files and downloading attachments.

Security & Authentication (Client‑Side)
Base64 encoding – Simple obfuscation for stored password hashes (not for production use).

Role‑based access control – Admin, Analyst, Viewer roles enforced in JavaScript.

Other APIs & Features
setInterval / clearInterval – Simulates real‑time threat feed updates (random threat generation every 15 seconds).

HTML5 <canvas> – Rendered by Chart.js for the threat distribution chart.

CSS Grid / Flexbox – Responsive layouts for stats cards, filter bars, and table.

CSS Variables – Dynamic theming (light/dark mode toggle).

No Backend / Server
Pure front‑end application – All data is stored locally in the browser. No external database, API calls, or server‑side logic.

Note: This project is a functional prototype / demo intended for local or educational use. The authentication, encryption, and file storage are not secure for real‑world classified data.
