# PushRank AI v0.2 – Auth

Cleane Push-up-App mit:
- Login
- Account erstellen
- geschützte Bereiche
- Workout mit Kamera
- erster KI-Zählung via MediaPipe Pose
- Rangliste
- Profil

## Start

```powershell
npm.cmd install
npm.cmd run dev
```

Dann öffnen:

```text
http://localhost:3000
```

## Login

Ohne Firebase läuft die App im Demo-Modus: Accounts werden lokal im Browser gespeichert.

Für echte Online-Accounts:

1. Firebase-Projekt erstellen
2. Authentication → Email/Password aktivieren
3. `.env.example` zu `.env.local` kopieren
4. Firebase-Web-App-Keys eintragen

```env
NEXT_PUBLIC_FIREBASE_API_KEY=
NEXT_PUBLIC_FIREBASE_AUTH_DOMAIN=
NEXT_PUBLIC_FIREBASE_PROJECT_ID=
NEXT_PUBLIC_FIREBASE_STORAGE_BUCKET=
NEXT_PUBLIC_FIREBASE_MESSAGING_SENDER_ID=
NEXT_PUBLIC_FIREBASE_APP_ID=
```

Für Handy-Browser am besten über Vercel deployen, weil Kamera HTTPS braucht.
