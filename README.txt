════════════════════════════════════════════
  THE HAPPENING SPACE — WEBSITE QUICK GUIDE
════════════════════════════════════════════

YOUR FILES
──────────
index.html            → Homepage
workshop-detail.html  → Workshop enrollment page (all artists)
HOW-TO-EDIT.html      → Full editing guide (open in browser)
images/               → Put all your photos here

BEFORE GOING LIVE — DO THESE 3 THINGS
───────────────────────────────────────
1. Add Razorpay Key in workshop-detail.html
   Search: const RAZORPAY_KEY
   Replace: 'rzp_live_XXXXXXXXXXXXXXXXXX'
   With:    your actual key from Razorpay dashboard

2. Add Google Sheets URL in workshop-detail.html
   Search: const SHEETS_URL
   Replace: 'https://script.google.com/macros/s/YOUR_SCRIPT_ID/exec'
   With:    your Apps Script web app URL

3. Update workshop dates, prices, spots in workshop-detail.html
   Search: const WORKSHOPS
   Edit each artist's slots and packages

GO LIVE
───────
1. Go to netlify.com/drop
2. Drag your whole folder onto the page
3. Done — you get a live URL instantly

UPDATE THE SITE
───────────────
1. Edit the file in VS Code
2. Save it
3. Drag updated folder to Netlify dashboard → Deploys
4. Live in 30 seconds

CHANGE A PRICE
──────────────
workshop-detail.html → find artist → find package → change price: 900

ADD A NEW DATE
──────────────
workshop-detail.html → find artist → slots: [ ] → add:
{ id: 's3', date: 'Saturday, 21 Jun 2025', time: '11:00 AM – 1:00 PM', spots: 20 },

ADD A REAL POSTER IMAGE
───────────────────────
1. Put image in images/ folder
2. workshop-detail.html → find artist → change posterBg:
   From: 'linear-gradient(145deg,#1a0407,#bc1f2e)'
   To:   'url(images/heet-poster.jpg) center/cover no-repeat'

CONTACT
───────
For help editing: Open HOW-TO-EDIT.html in your browser
════════════════════════════════════════════
