# Schulplaner

1. supabase.com: Konto, neues Projekt. SQL Editor: Inhalt von supabase.sql ausfuehren.
2. Project Settings > API: URL und anon public Key in config.js eintragen.
3. Authentication > Providers > Email: "Confirm email" abschalten (oder Bestaetigungsmail nutzen).
4. Alle Dateien in ein GitHub Repository, Settings > Pages > Branch main, Ordner /root.
5. iPhone/iPad: Safari, Teilen, "Zum Home Bildschirm". Einmal online oeffnen und anmelden.

## Mehrere Nutzer
- In config.js nur den anon public Key verwenden, niemals den service_role Key.
- Authentication > URL Configuration: Site URL und Redirect URL auf die GitHub Pages Adresse setzen, sonst funktioniert "Passwort vergessen" nicht.
- Jeder Nutzer sieht nur seine eigenen Daten (Row Level Security aus supabase.sql). Das SQL muss ausgefuehrt sein.
- Neue Nutzer starten mit leerem Stundenplan.
