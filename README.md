Create a mobile-friendly, GitHub Pages-ready travel guidebook website for a family Japan trip.

The website must be extremely simple, intuitive, and optimized for elderly users with large buttons and minimal confusion.

The final product should be a static website deployable via GitHub Pages:
`https://username.github.io/japan-trip-guide/`

Refer all required information and knowledge from japan_trip_handbook_full.md

Use only:

* HTML
* CSS
* Vanilla JavaScript
  (no frameworks required unless absolutely necessary)

All file paths must be relative for GitHub deployment.

---

# 1. SITE STRUCTURE (IMPORTANT)

The website must have a **HOME PAGE as the entry point**

## Home Page (index.html)

The home page should contain ONLY two main large buttons:

### 1. 📍 Itinerary

→ Leads to full trip details (day-by-day travel plan)

### 2. 📷 QR Codes

→ Leads to all QR-related documents and screenshots

No other clutter on the homepage.

Design requirement:

* Very large buttons
* Very clear labels
* Mobile-first layout
* Elderly-friendly UI

---

# 2. QR CODE SECTION (SEPARATE PAGE)

Inside the QR Code page:

## Structure:

### A. Immigration QR Codes

Create clickable buttons for each traveler:

* Kang Kong Yong
* Khoo Seok Fah
* Kang Huay Yee
* Kang Huay Wen
* Kang Huay Qi

### Behavior:

* Clicking a name displays that person’s QR code image
* QR codes are stored locally in:

```text id="qr_structure"
/immigration/
/shinkansen/
/usj/ (placeholder)
/amanohashidate/ (placeholder)
```

---

### B. Shinkansen QR Codes

Same structure as above or grouped separately.

---

### C. Other Tickets / Documents

Include placeholders for:

* USJ tickets (pending)
* Amanohashidate tickets (pending)
* Any other important screenshots

---

### IMPORTANT SAFETY FEATURE

At top of QR page include a warning:

> “Please download or screenshot all QR codes before travel. Internet may not be available at immigration.”

---

# 3. ITINERARY SECTION (SEPARATE PAGE)

This page contains full travel details organized by tabs or sections:

## Structure:

* Day 1
* Day 2
* Day 3
* Day 4
* Day 5
* Day 6
* Day 7
* Day 8
* Day 9

Each day should be clearly separated with:

* Date header
* Activities
* Transport
* Hotel info
* Notes

---

# 4. TRANSPORTATION FORMAT STANDARD (VERY IMPORTANT)

All transport information must follow a consistent format:

## Standard Template:

### Transport Mode:

(e.g. Train / Subway / Shinkansen / Walk / Taxi)

### Route:

Origin → Transfer → Destination

### Details:

* Duration: XX mins
* Line name (if applicable)
* Platform / Exit number

### Example:

**Transport Mode:** Train (Nankai Line)
**Route:** Kansai Airport → Namba Station → Hotel

**Details:**

* Duration: 56 mins
* Line: Nankai Kuko Line (Purple Line)
* Exit: Exit 8
* Walk: 800m (15 mins)
* Last train: 23:55

---

# 5. DESIGN REQUIREMENTS

* Large font sizes for readability
* High contrast UI
* Minimalist layout
* Big touch-friendly buttons
* No clutter or dense text blocks
* Mobile-first design
* Simple navigation back to Home Page

---

# 6. NAVIGATION RULES

Every page must include:

* A clear “Back to Home” button
* Simple navigation system (no deep menus)

---

# 7. OFFLINE-FIRST REQUIREMENT

Because QR codes are critical at airports:

* QR pages must work fully offline
* All images must be preloaded locally
* No dependency on internet for QR access

---

# FINAL OUTPUT GOAL

A fully functional GitHub Pages-ready travel handbook that:

* Starts from a simple homepage
* Has 2 main sections (Itinerary + QR Codes)
* Clearly separates travel info vs critical QR documents
* Works perfectly on mobile
* Is easy enough for elderly family members to use without confusion
