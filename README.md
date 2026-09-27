<div align="center">

  <!-- ==================== BANNER LED NEON OPETEER ==================== -->
  <svg viewBox="0 0 900 240" width="100%" xmlns="http://www.w3.org/2000/svg">
    <defs>
      <!-- Filter Glow Neon -->
      <filter id="neon-glow" x="-50%" y="-50%" width="200%" height="200%">
        <feGaussianBlur stdDeviation="3.5" result="coloredBlur"/>
        <feMerge>
          <feMergeNode in="coloredBlur"/>
          <feMergeNode in="coloredBlur"/>
          <feMergeNode in="SourceGraphic"/>
        </feMerge>
      </filter>
      
      <!-- Pola Grid Titik LED Fisik -->
      <pattern id="led-matrix-dots" width="8" height="8" patternUnits="userSpaceOnUse">
        <circle cx="4" cy="4" r="1.2" fill="#151922" />
      </pattern>

      <style>
        @keyframes neonFlicker {
          0%, 19%, 21%, 23%, 25%, 54%, 56%, 100% {
            opacity: 1;
            filter: drop-shadow(0 0 5px #00ffcc) drop-shadow(0 0 15px #00ffcc) drop-shadow(0 0 30px #00a6ff);
          }
          20%, 24%, 55% {
            opacity: 0.35;
            filter: none;
          }
        }

        @keyframes borderPulse {
          0%, 100% { stroke: #ff0055; filter: drop-shadow(0 0 4px #ff0055); }
          50% { stroke: #ff7700; filter: drop-shadow(0 0 8px #ff7700); }
        }

        .sign-border {
          stroke-dasharray: 8 6;
          animation: borderPulse 3s infinite ease-in-out;
        }

        .led-neon-text {
          font-family: 'Courier New', Courier, monospace, 'Segoe UI Black', Impact;
          font-size: 88px;
          font-weight: 900;
          letter-spacing: 14px;
          fill: #e6ffff;
          stroke: #00ffcc;
          stroke-width: 2.5px;
          stroke-dasharray: 4 6; /* Mengubah garis teks menjadi titik-titik LED */
          stroke-linecap: round;
          animation: neonFlicker 4s infinite;
        }

        .sub-bar {
          font-family: monospace;
          font-size: 13px;
          letter-spacing: 5px;
          fill: #ffe600;
          filter: drop-shadow(0 0 3px #ffcc00);
        }
      </style>
    </defs>

    <!-- Rangka Papan Rambu Lalu Lintas -->
    <rect x="15" y="15" width="870" height="210" rx="20" fill="#07090e" stroke="#1f2937" stroke-width="6"/>
    <!-- Background Matriks LED -->
    <rect x="25" y="25" width="850" height="190" rx="14" fill="#0b0f17"/>
    <rect x="25" y="25" width="850" height="190" rx="14" fill="url(#led-matrix-dots)"/>

    <!-- Lampu LED Sinyal Kuning / Amber Rambu -->
    <circle cx="50" cy="50" r="5" fill="#ffb700" filter="drop-shadow(0 0 4px #ffb700)"/>
    <circle cx="70" cy="50" r="5" fill="#ffb700" filter="drop-shadow(0 0 4px #ffb700)"/>
    <circle cx="830" cy="50" r="5" fill="#ffb700" filter="drop-shadow(0 0 4px #ffb700)"/>
    <circle cx="850" cy="50" r="5" fill="#ffb700" filter="drop-shadow(0 0 4px #ffb700)"/>

    <!-- Lis Neon Rambu Berkedip -->
    <rect x="35" y="35" width="830" height="170" rx="10" fill="none" class="sign-border" stroke-width="3"/>

    <!-- Banner Utama: OPETEER (Dot LED + Neon Flicker) -->
    <text x="50%" y="135" text-anchor="middle" class="led-neon-text">OPETEER</text>

    <!-- Sub-status bergaya Highway Matrix Sign -->
    <text x="50%" y="175" text-anchor="middle" class="sub-bar">● TRAFFIC: ACTIVE // SYSTEM: ONLINE ●</text>
  </svg>

  <br/><br/>

  <!-- Status / Headline -->
  <p>
    <code>const developer = "OPETEER";</code><br/>
    🚦 <i>Navigating through code, bugs, and nocturnal deployments.</i>
  </p>

  <!-- Badges / Tech Stack -->
  <p>
    <img src="https://img.shields.io/badge/STATUS-CODING-00ffcc?style=for-the-badge&logoColor=black&labelColor=07090e" alt="Status"/>
    <img src="https://img.shields.io/badge/FOCUS-FULLSTACK-ff0055?style=for-the-badge&logoColor=white&labelColor=07090e" alt="Focus"/>
    <img src="https://img.shields.io/badge/NIGHT_MODE-ALWAYS_ON-ffe600?style=for-the-badge&logoColor=black&labelColor=07090e" alt="Night Mode"/>
  </p>

</div>

---

### 📡 System Diagnostics

```yaml
Terminal:
  Location: Yogyakarta, ID
  Primary_Focus: Web Architecture & Systems
  Current_Routine: "Refactoring legacy code into lightweight engines"
  Status_Indicator: "🟢 Glowing bright on main branch"
