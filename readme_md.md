# 🏥 Bringolino - Krankenhaus Logistik App

Eine moderne Progressive Web App (PWA) für das Kepler Universitätsklinikum zur Verwaltung von DECT-Aufgaben und Logistik-Dokumentation.

![Bringolino Logo](https://via.placeholder.com/400x200/4F46E5/FFFFFF?text=Bringolino)

## ✨ Features

### 📱 Core Funktionalität
- **DECT-System Integration**: Vollständige Unterstützung für alle DECT-Codes (27518-27543)
- **Aufgabenverwaltung**: Interaktive To-Do Listen mit Zeitplanung
- **Real-time Dokumentation**: Live-Dokumentation für Wäsche, Transport, Medikamente
- **Progress Tracking**: Fortschrittsanzeige und Leistungsstatistiken
- **Punktesystem**: Gamification mit Belohnungen und Achievements

### 🚀 Technische Features
- **Progressive Web App (PWA)**: Offline-Funktionalität, App-Installation
- **Responsive Design**: Optimiert für Mobile, Tablet und Desktop
- **Real-time Sync**: Firebase Integration für Live-Updates
- **Advanced Analytics**: Detaillierte Leistungsanalysen und Dashboards
- **Leader Dashboard**: Management-Interface für Führungskräfte

### 📊 Spezial-Module
- **Mopp-Versorgung**: Komplette Stationsübersicht mit Anlieferungspunkten
- **Apotheken-Dokumentation**: Medikamentenverteilung und -kontrolle
- **Transport-Management**: Hauptmagazin Neu-/Altbau Koordination
- **Suchtgift-Kontrolle**: Spezielle Dokumentation für kontrollierte Substanzen
- **Kleiderbügel-Service**: Abholung bei Personalumkleiden
- **Bad Hall Versorgung**: Externe Standort-Koordination

## 🛠️ Installation & Setup

### Voraussetzungen
- Node.js 18+ 
- npm oder yarn
- Git

### Lokale Entwicklung

```bash
# Repository klonen
git clone https://github.com/yourusername/bringolino-app.git
cd bringolino-app

# Dependencies installieren
npm install

# Development Server starten
npm run dev

# App öffnet sich unter http://localhost:3000
```

### Build für Produktion

```bash
# Production Build erstellen
npm run build

# Build testen
npm run preview
```

## 🚀 Deployment auf Netlify

### Automatisches Deployment

1. **GitHub Repository** erstellen und Code pushen
2. **Netlify Account** erstellen/einloggen
3. **"New site from Git"** auswählen
4. **GitHub Repository** verbinden
5. **Build Settings** konfigurieren:
   - Build command: `npm run build`
   - Publish directory: `dist`
   - Node version: `18`

### Environment Variables (optional)
```
VITE_FIREBASE_API_KEY=your_api_key
VITE_FIREBASE_AUTH_DOMAIN=your_domain
VITE_FIREBASE_PROJECT_ID=your_project_id
```

## 📱 PWA Installation

### Mobile (iOS/Android)
1. Website in Safari/Chrome öffnen
2. "Zum Homebildschirm hinzufügen" wählen
3. App-Icon erscheint auf dem Homescreen

### Desktop (Chrome/Edge)
1. Website öffnen
2. Adressleiste: Install-Icon klicken
3. "Installieren" bestätigen

## 🏗️ Architektur

### Tech Stack
- **Frontend**: React 18 + TypeScript + Vite
- **Styling**: Tailwind CSS + Custom Glassmorphism
- **Icons**: Lucide React
- **PWA**: Vite-Plugin-PWA + Workbox
- **Backend**: Firebase Realtime Database (Optional)
- **Deployment**: Netlify

### Ordnerstruktur
```
bringolino-app/
├── public/                 # Statische Assets
├── src/
│   ├── components/        # React Komponenten
│   ├── services/         # Firebase & API Services
│   ├── types/            # TypeScript Definitionen
│   ├── utils/            # Hilfsfunktionen
│   ├── App.tsx           # Haupt-App Komponente
│   └── main.tsx          # Entry Point
├── dist/                 # Build Output
└── package.json         # Dependencies
```

## 🎯 DECT-Codes & Aufgaben

### Unterstützte DECTs
- **27527**: Kleiner Botendienst (9 Aufgaben)
- **27521**: Essen Service N & D (6 Aufgaben)  
- **27522**: Wäsche & Küchen Service (7 Aufgaben)
- **27525**: Bauteil C Service (7 Aufgaben)
- **27529**: Bauteil H & Kindergarten (9 Aufgaben)
- **27530**: Hauptmagazin Service (6 Aufgaben)
- **27519**: S3 Wochenende (7 Aufgaben)
- **27520**: LD Samstag/Sonntag (8 Aufgaben)
- **27543**: AK N Müllzentrale (7 Aufgaben)
- **27538**: Post Service Freitag (2 Aufgaben)
- **Und weitere...**

### Aufgaben-Features
- ⏰ Zeitbasierte Planung (06:30 - 18:30)
- 🔴 Prioritätsstufen (Hoch/Mittel/Niedrig/Pause)
- 📍 Standort-Information
- ⏱️ Geschätzte Dauer
- ℹ️ Spezielle Bedingungen
- ✅ Fortschritts-Tracking

## 📊 Analytics & Reporting

### Live Dashboard
- **Real-time Monitoring**: Alle DECT-Aktivitäten
- **Performance Metrics**: Abschlussraten, Effizienz
- **Department Ranking**: Leistungsvergleiche
- **Active Users**: Live Benutzer-Tracking

### Statistiken
- **Tägliche Performance**: Aufgaben, Zeit, Punkte
- **Wöchentliche Trends**: 5-Wochen Vergleich
- **Stündliche Aktivität**: Peak-Zeiten Analyse
- **Achievements**: Badges und Erfolge

## 🔧 Konfiguration

### PWA Manifest (`vite.config.ts`)
```typescript
manifest: {
  name: 'Bringolino - Krankenhaus Logistik',
  short_name: 'Bringolino',
  description: 'Kepler Universitätsklinikum Logistik App',
  theme_color: '#4F46E5',
  background_color: '#ffffff',
  display: 'standalone',
  orientation: 'portrait'
}
```

### Tailwind Konfiguration
- Custom Glassmorphism Styles
- Mobile-First Responsive Design
- Dark/Light Mode Support
- Accessibility Optimierungen

## 🤝 Contributing

1. Fork das Repository
2. Feature Branch erstellen (`git checkout -b feature/AmazingFeature`)
3. Changes committen (`git commit -m 'Add AmazingFeature'`)
4. Branch pushen (`git push origin feature/AmazingFeature`)
5. Pull Request öffnen

## 📄 Lizenz

Dieses Projekt ist für das Kepler Universitätsklinikum entwickelt.

## 🆘 Support

Bei Fragen oder Problemen:
- GitHub Issues erstellen
- IT-Support Kepler UK kontaktieren
- Dokumentation prüfen
## Deployment Status: Active

---

**Entwickelt mit ❤️ für das Kepler Universitätsklinikum**

*Moderne Technologie für bessere Patientenversorgung* 🏥✨
