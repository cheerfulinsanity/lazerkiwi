# LAZER KIWI GUILD WEBSITE – README

Welcome to the Lazer Kiwi Dota 2 Guild Website!
This modular HTML dashboard visualizes live guild stats, ranks, and weekly performance using Google Sheets endpoints.

Maintained by: Bag of Dicks

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
🔧 MODULES OVERVIEW
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Each tab is its own HTML module, linked via `index.html`:

• Home_Page_MASTER.html
  → Welcome message, visit counter, AI kiwi art, news feed (live).

• Turbo_Rank_Graphs_MASTER.html
  → Graphs turbo rank history for selected member (2-point line chart).

• Party_Average_Rank_Estimator_MASTER.html
  → Estimates 5-player party rank using dropdowns (static dataset).

• Weekly_Guild_Point_Leaderboard_MASTER.html
  → Weekly gains, sortable columns, rolling average, toggleable total/avg.

• Weekly_Point_Earning_Graphs_MASTER.html
  → Graphs weekly point gain comparison (2 players, live data).

• Guild_Estimated_Turbo_Rank_List_MASTER.html
  → Current turbo rank snapshot list for public data players.

• index.html
  → Tabbed navigation integrating all modules into one unified layout.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
🌐 LIVE JSON ENDPOINTS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
1. Turbo Rank History:
   https://script.google.com/macros/s/AKfycbzAOfvSd1CvLTCRj6YLlDLQEJSkfXHxvKE0PIhl5iU9gtTg3fVoE3mCn2M_aCI1OzL0hw/exec

2. Weekly Point Data (Leaderboard + Graphs):
   https://script.google.com/macros/s/AKfycbz3txnsBI5fLUtGxuw2RwvUTlfTthoyNiufE3pdxEa0F4ESsMoN439s85T2C2da1Mg/exec

3. Totals + 3/4-Week Average:
   https://script.google.com/macros/s/AKfycbxCm2fdYwdu-EHsDAT2AxnO6NsZ2d_mkg-4Meke-FTRBxTGEF5AmwLPifcbFOn5lYQY/exec

4. Visit Counter (Home):
   https://script.google.com/macros/s/AKfycbztKjPJahRvifOZBqlOA890PBXK5AqAqv2VksE7A1JlAHN84gQ98mxVjwDi98K6Sn6nsg/exec

5. News Feed (Home):
   https://script.google.com/macros/s/AKfycbzO8o3mKTDxHg5L2FGYe_ClEQtVZDy2HTW1JkXGsF5XJEbFNIoKejOU4jSDJGzMfqyXMg/exec

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
🎨 STYLING & VISUAL THEME
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
- Background: #000000 (black)
- Text/Highlight: #00FF00 (neon green)
- Accent/Borders: #ab6e11 (burnt orange)
- Font: Orbitron (Google Fonts)
- Graph Line Colors:
  • Player 1: Cyan (#00FFFF)
  • Player 2: Pink (#FF6699)
- Design Features:
  • Neon glows, hover effects, tab UI
  • All inline scripts for simplicity
  • Blinking “loading” messages via CSS keyframes

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
📋 SPECIAL BEHAVIOR
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
• Weekly Leaderboard:
  – Toggles extra columns (Total Points + 3/4 Week Avg)
  – Column label changes by week (e.g. 2-Week Avg)
  – Shader colors:
      Purple – Top 3 Avg
      Green  – Avg > 2000
      Orange – 1000–2000
      Red    – Avg < 1000

• Turbo Graphs:
  – Only 2 data points shown (minified display)
  – Y-axis labels reflect rank names
  – Dropdown filters players with data

• Party Estimator:
  – Dropdowns use static rank dataset
  – Renders average rank using internal map

• Visit Counter:
  – Dev/local mode suppresses incrementing
  – Value displayed with 🧿 icon

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
📂 FILE RULES & VERSIONING
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
• All working files use `_MASTER.html`
• New versions must follow suffix format:
  _v2, _PATCHED, _FINAL_FIXED, etc.
• You must request ChatGPT to implement any changes.
• Manual edits to HTML files are discouraged.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
📌 INTEGRATION NOTES
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
• All tabs are loaded into `index.html` using iframes.
• Banner located at: `home_gallery_assets/Banner.png`
• Image: `kiwi.png` used for future branding (not yet embedded).

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
🧠 MAINTENANCE & EXTENSIONS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Ideas for future:
• Add Dota stats (e.g., winrate overlays)
• Discord bot integration
• Guild member bios
• Steam image avatars
• Auto match updates (scraping or API)

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
END OF README
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
