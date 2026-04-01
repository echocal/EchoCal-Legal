# Jak hostować te pliki?

Te dwa pliki (privacy.html i terms.html) muszą być dostępne publicznie pod adresem URL, aby Apple i Google mogły zaakceptować Twoją aplikację.

### Metoda 1: GitHub Pages (Zalecane)
1. Wrzuć te pliki do swojego repozytorium na GitHub (np. do folderu `docs` lub po prostu do głównego katalogu).
2. Wejdź w ustawienia repozytorium na GitHub -> **Settings** -> **Pages**.
3. Wybierz źródło `Deploy from a branch` i wybierz swoją gałąź (np. `master`).
4. GitHub wygeneruje adres w stylu: `https://twoj-uzytkownik.github.io/EchoCal/privacy.html`

### Metoda 2: Własna strona / Hosting
1. Jeśli masz wykupiony hosting, po prostu wgraj te pliki przez FTP.
2. Adresy będą wyglądać tak: `https://twojadomena.pl/privacy.html`

### Metoda 3: Firebase Hosting / Vercel
1. Jeśli używasz Firebase w projekcie, możesz użyć `firebase deploy --only hosting`.
2. Adresy będą darmowe w domenie `.web.app`.

---
**Pamiętaj:** Kiedy już będziesz mieć adresy URL, musisz je wkleić w:
- App Store Connect (pole "Privacy Policy URL" i "EULA URL")
- Google Play Console (sekcja "Polityka prywatności")
- Aplikacji EchoCal (w komponencie Paywall i profilu, aby linki kierowały do żywych stron).
