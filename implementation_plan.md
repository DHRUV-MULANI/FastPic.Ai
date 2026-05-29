# FastPic.AI — Complete Design System & All Pages

## Overview
Premium AI-powered photography platform. Full interactive prototype built as HTML/CSS/JS with all pages inter-connected (simulating Google Stitch flows). Dark, Google Pixel–inspired aesthetic with glassmorphism, fluid gradients, and premium motion.

## Design System

### Color Palette
- **Background:** `#08080F` (near black)
- **Surface:** `#0F0F1A` (dark navy)
- **Card:** `#13131F` with glassmorphism
- **Primary:** `#6366F1` (indigo-violet)
- **Primary Glow:** `#818CF8`
- **Accent:** `#22D3EE` (cyan)
- **Success:** `#10B981`
- **Warning:** `#F59E0B`
- **Text Primary:** `#F8FAFC`
- **Text Secondary:** `#94A3B8`
- **Border:** `rgba(255,255,255,0.08)`

### Typography
- **Headings:** Plus Jakarta Sans (700/800)
- **Body:** Inter (400/500)
- **Mono:** JetBrains Mono

## Pages to Build (15 Screens)

### MARKETING SITE
1. **Landing Page** (`index.html`) — Hero + Features + How It Works + Pricing + FAQ + Footer
2. **Pricing Page** (`pricing.html`) — Storage plans comparison
3. **Guest Gallery Entry** (`gallery-entry.html`) — Link / PIN / QR / Selfie Access

### AUTH
4. **Login / Register** (`auth.html`) — Sign in, Sign up tabs

### PHOTOGRAPHER DASHBOARD
5. **Dashboard Home** (`dashboard.html`) — Stats, events list, storage meter
6. **Events / Groups Page** (`events.html`) — Event cards, create event modal
7. **Event Gallery** (`event-gallery.html`) — Folders + photo grid + upload
8. **Photo Viewer** (`photo-viewer.html`) — Fullscreen photo, actions, face tags
9. **AI Face Search** (`face-search.html`) — Selfie upload → face match results
10. **Team Management** (`settings-team.html`) — Roles, invite, permissions
11. **Business Branding** (`settings-branding.html`) — Logo, GST, social links
12. **Watermark Engine** (`settings-watermark.html`) — Dual watermark, position, opacity
13. **Activity Logs** (`settings-logs.html`) — Immutable audit trail
14. **Billing / Storage** (`settings-billing.html`) — Plan upgrade, usage meter

### GUEST VIEW
15. **Guest Gallery View** (`guest-gallery.html`) — Anonymous gallery with favorites + face-filtered view

## Inter-page Connections (Navigation Flow)
```
Landing → Auth → Dashboard → Events → Event Gallery → Photo Viewer
                                    → AI Face Search
Dashboard → Settings (Branding / Watermark / Team / Logs / Billing)
Landing → Pricing
Landing → Guest Gallery Entry → Guest Gallery View
```

## Implementation Strategy
- Single shared `design-system.css` for all design tokens
- Responsive desktop-first (1440px canvas)
- Glassmorphism cards with `backdrop-filter`
- Sidebar navigation for dashboard pages
- Animated transitions between pages
- Real image placeholders via Unsplash CDN

## Files Structure
```
/home/boss/Projects/FastPic.AI/design/
├── design-system.css
├── index.html          (Landing)
├── pricing.html
├── auth.html
├── gallery-entry.html
├── dashboard.html
├── events.html
├── event-gallery.html
├── photo-viewer.html
├── face-search.html
├── guest-gallery.html
├── settings-branding.html
├── settings-watermark.html
├── settings-team.html
├── settings-logs.html
└── settings-billing.html
```
