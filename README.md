# meinzeug HUD

[![Status: Prototyp](https://img.shields.io/badge/status-prototype-orange.svg)](#projekt-logbuch)
[![Focus: Self-hosting](https://img.shields.io/badge/focus-self--hosting-blue.svg)](#werte--prinzipien)
[![License: TBD](https://img.shields.io/badge/license-tbd-lightgrey.svg)](#lizenz)

> Privates HUD-Labor zum Verbinden deiner eigenen Hosts, Tokens und Repositories, ohne Werbung, Bezahlschranken oder fremde Tenants.

**Kurz gesagt**
- kostenloses Hobby-Projekt mit Fokus auf Lern- und Experimentier-Workflows
- alle Secrets bleiben bei dir; der Code läuft nur auf deinen Maschinen
- kleine Community, direkter Austausch via Mail oder Matrix (nach Einladung)

## Inhaltsverzeichnis
1. [Über das Projekt](#über-das-projekt)
2. [Repository-Überblick](#repository-überblick)
3. [Feature-Highlights](#feature-highlights)
4. [Werte & Prinzipien](#werte--prinzipien)
5. [Schnellstart](#schnellstart)
6. [Projekt-Logbuch](#projekt-logbuch)
7. [Roadmap](#roadmap)
8. [Mitwirken](#mitwirken)
9. [Support & Kontakt](#support--kontakt)
10. [Lizenz](#lizenz)

## Über das Projekt
meinzeug HUD ist ein persönliches Self-hosting-Labor, das ein zentrales Dashboard (HUD) mit deinen eigenen Ressourcen verbindet. Das Ziel ist es, Infrastruktur zu verstehen, Presets zu testen und Integrationen bewusst zu steuern statt Automationen zu verkaufen. Alles läuft lokal oder auf Servern, die dir gehören.

## Repository-Überblick
```
.
├── assets
│   ├── css
│   │   └── style.css        # zentrales Styling für das HUD
│   └── img
│       └── favicon.png      # Icon für Browser & PWA
├── index.html               # Landing-Page/Mockup für das HUD
└── README.md                # Projektbeschreibung (diese Datei)
```

## Feature-Highlights
- **Privates HUD** – läuft ausschließlich auf selbst verwalteten Maschinen.
- **Setup nach Bedarf** – verbindet SSH, Hetzner, AWS oder andere Provider, ohne Ownership abzugeben.
- **Manuelle Trigger** – Aktionen starten nur, wenn du sie auslöst; keine versteckten Chronjobs.
- **Secret Tresor** – Schlüssel werden clientseitig verschlüsselt und lassen sich jederzeit löschen.
- **Human-Scale Community** – Presets entstehen in kleinen Chats, nicht in öffentlichen Bundle-Stores.
- **Direkter Kontakt** – Support erfolgt freiwillig per Mail oder Matrix.
- **Experimentiermodus** – neue Nodes/APIs kommen als Hobby-Features ohne SLA hinzu.
- **HUD Shortcuts** – Command Palette und Hotkeys bleiben lokal anpassbar.

## Werte & Prinzipien
1. **Kein Verkauf** – es gibt keine Pläne, Stores oder Werbung.
2. **Eigenes Eigentum** – jede Ressource bleibt unter deiner Kontrolle.
3. **Transparenz** – Logbuch-Updates dokumentieren Experimente, Security Notes und rechtliche Hinweise.
4. **Privatsphäre zuerst** – keine zentrale Telemetrie; Logs bleiben in deinen Systemen.
5. **Lernorientiert** – jede Änderung soll dokumentiert und reproduzierbar sein.

## Schnellstart
### 1. Repository klonen
```bash
git clone https://github.com/<dein-user>/hud.git
cd hud
```

### 2. Statische Landing-Page ansehen
```bash
# beliebigen lokalen Static-Server starten
python -m http.server 4173
# oder
npx serve .
```
Öffne danach `http://localhost:4173/index.html`, um das HUD-Mockup inklusive Styles zu prüfen.

### 3. Eigene Presets dokumentieren
- Passe Inhalte in `index.html` an oder lege weitere Module im Ordner `assets/` ab.
- Nutze Issues oder das Logbuch im README, um Experimente nachvollziehbar zu halten.

## Projekt-Logbuch
| Datum        | Ereignis                         | Notizen |
|--------------|----------------------------------|---------|
| 16. Juli 2025 | Erster Prototyp veröffentlicht   | HUD-Dashboard ging intern live; frühes Feedback läuft. |
| 3. August 2025 | Start des Community-Programms   | Matrix-Chat geöffnet, Presets können geteilt werden. |

## Roadmap
- [x] Prototyp V1 online bringen (Juli 2025)
- [x] Community-Programm aufsetzen (August 2025)
- [ ] Secrets-Vault mit Hardware-Keys testen
- [ ] Self-hosting Installer (Ansible/Taskfile)
- [ ] Öffentliche Demo ohne Login bereitstellen
- [ ] Beta-Release mit dokumentierter API

## Mitwirken
1. **Issues** – nutze GitHub Issues für Bug-Reports, Security-Hinweise oder Ideen.
2. **Fork & Branch** – erstelle einen Fork, arbeite auf einem beschreibenden Branch (`feature/hud-shortcuts`).
3. **Style-Guides** – halte dich an das bestehende CSS und dokumentiere neue Komponenten direkt im README.
4. **Pull Request** – beschreibe, warum die Änderung nötig ist, welche Risiken bestehen und wie getestet wurde.
5. **Security-Disclosure** – melde potenzielle Schwachstellen nicht öffentlich, sondern per Direktkontakt.

## Support & Kontakt
- **E-Mail** – auf Anfrage (siehe Issues); kein offizieller Helpdesk, Support ist freiwillig.
- **Matrix** – Einladungslink wird individuell geteilt, sobald du Teil der kleinen Runde wirst.
- **Issues** – nutze GitHub, wenn du Feedback öffentlich dokumentieren möchtest.

## Lizenz
Es wurde noch keine Open-Source-Lizenz ausgewählt. Nutze den Code daher nur privat und frage vorher nach, wenn du Teile wiederverwenden möchtest.
