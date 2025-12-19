
# Game Design Document - Struktur

## 1. Übersicht

**Spieltitel:** Virtual Hacking  
**Genre:** Multiplayer Echtzeit-Strategie / Base-Building / Cyberwarfare  
**Zielplattformen:** Mobile (iOS/Android), Web  
**Zielgruppe:** Casual-Spieler aller Altersgruppen  

**USP:**
- Echtzeit-Multiplayer-Hacking mit Base-Building und Cyber-Angriffen
- Casual-freundlich: Idle-Ressourcengenerierung, asynchrone Verteidigung, Auto-Resolve für QTEs
- Tiefgang: Allianzen, Events, Allianzkriege und dynamische QTEs für taktische Spieler





## 2. Spielkonzept

### 2.1 Kernidee
Spieler bauen und verteidigen ihr virtuelles Computernetzwerk, während sie gleichzeitig Angriffe auf andere Spieler oder NPC-Systeme durchführen. Das Spiel kombiniert Strategie, Ressourcenmanagement und Echtzeit-Interaktion in einer cyberpunk-lastigen, aber familienfreundlichen Umgebung.

### 2.2 Gameplay-Loop

**Login:** Spieler sieht die Rechner-Übersicht (Kachelansicht aller Systeme).

**Rechner-Management:**
- Klick auf einen Rechner öffnet ein Overlay mit Upgrade-Optionen (Hardware/Software)
- Bauzeiten für Upgrades (z. B. 1 Stunde für Firewall-Level 2)
- Upgrades können abgebrochen werden (Ressourcen werden teilweise zurückerstattet)

**Angriff/Verteidigung:**
- Angriffe werden über das Angriffsmenü gestartet (Zielauswahl, Angriffstyp)
- Quicktime-Events (QTEs) bei Angriffen/Verteidigungen (siehe Kapitel 4.3)
- Auto-Resolve-Option für Casual-Spieler (QTEs werden übersprungen, aber mit Malus auf Erfolgschance)

**Asynchrone Verteidigung:**
- Angriffe auf den Spieler laufen auch offline ab
- Push-Benachrichtigungen bei Angriffen (konfigurierbar)
- Event-Log zeigt Ergebnisse nach dem Login

**Allianzen & Events:**
- Spieler können Allianzen beitreten (Beitrittsregeln werden von Allianzen selbst festgelegt)
- PvP/PvE-Events (z. B. „Server-Sturm", „Daten-Rettung") mit Bonus-Belohnungen
- Allianzkriege (Allianzen kämpfen um Territorien oder exklusive Upgrades)


## 3. Spielwelt

### 3.1 Rechner-Übersicht

**Visuelle Darstellung:**
- Kachelansicht aller Rechner mit Status-Icons (Online, Unter Angriff, Offline)
- Farbcodierung (grün = sicher, gelb = Warnung, rot = kritisch)

**Overlay-Funktionen:**
- Hardware/Software-Übersicht (aktuelle Komponenten und deren Level)
- Upgrade-Optionen mit Bauzeiten und Ressourcenkosten
- Schnell-Upgrade-Button für häufig genutzte Aktionen

### 3.2 Schnellzugriffsleiste & Menü

**Schnellzugriffsleiste (unten):**
- Angriff starten (Icon: Schwert)
- Verteidigung (Icon: Schild)
- Ressourcen (Icon: Münze)
- Allianz (Icon: Gruppen-Symbol)

**Hamburger-Menü:**
- Forschung (Tech-Baum)
- Events (aktuelle Challenges)
- Einstellungen (Benachrichtigungen, Grafik)
- Statistiken (Erfolge, Highscores)

## 4. Mechaniken & Systeme

### 4.1 Rechner-Upgrades

**Hardware-Upgrades:**
- CPU (erhöht Rechenleistung für Angriffe)
- RAM (ermöglicht mehr gleichzeitige Prozesse)
- Festplatte (erhöht Speicherkapazität für Ressourcen)

**Software-Upgrades:**
- Firewall (reduziert Angriffsschaden)
- Antivirus (erhöht Erfolgschance bei Abwehr)
- Hacking-Tools (verbessert Angriffserfolg)

**Bauzeiten & Kosten:**
- Beispiel: Firewall Level 2 → 1 Stunde Bauzeit, 50 Ressourcen
- Upgrades können abgebrochen werden (50% Ressourcen-Rückerstattung)

### 4.2 Angriffe & Verteidigung

**Angriffstypen:**
- Spionage (Daten klauen)
- Malware-Injektion (Gegner-Systeme beschädigen)
- DDOS (Gegner lahmlegen)
- Datenklau (Ressourcen stehlen)
- Sabotage (Gegner-Upgrades zerstören)

**Quicktime-Events (QTEs):**
- Dynamische Minispiele je nach Angriffstyp
- Auto-Resolve: QTEs werden übersprungen, aber Erfolgschance sinkt um 20%

### 4.3 QTE-Mechaniken

| Angriffstyp | QTE-Mechanik | Beispiel |
|---|---|---|
| Spionage | Reaktionsspiel | Tasten schnell drücken |
| Malware-Injektion | Logik-Puzzle | Codezeilen sortieren |
| DDOS | Rhythmus-Spiel | Tasten im Takt drücken |
| Datenklau | Memory-Spiel | Richtige Datenblöcke auswählen |
| Sabotage | Präzisionsklick | Kritische Systeme treffen |

### 4.4 Asynchrone Verteidigung

**Push-Benachrichtigungen:**
- „Dein Rechner [Name] wird angegriffen!"
- „Angriff abgewehrt! Ressourcenverlust: 5%"
- Einstellungen: Spieler kann Benachrichtigungstypen filtern

**Event-Log:**
- Übersicht der letzten 24 Stunden (Zeitstempel, Angriffstyp, Ergebnis)

### 4.5 Allianzen & Events

**Allianz-System:**
- Beitritt: Spieler können Allianzen gründen/beitreten (Regeln werden von Allianzen festgelegt)
- Ränge: Mitglieder, Offiziere, Leader (mit unterschiedlichen Rechten)
- Allianz-Basis: Gemeinsame Upgrades (z. B. „Allianz-Firewall")

**PvP/PvE-Events:**
- „Server-Sturm": Allianz greift gemeinsam einen NPC-Boss an (Belohnung: Bonus-Ressourcen)
- „Daten-Rettung": Allianz verteidigt einen Server gegen NPC-Hacker (Belohnung: Exklusive Upgrades)

**Allianzkriege:**
- Allianzen kämpfen um Territorien oder exklusive Boni
- Kriegserklärung: Nur durch Allianz-Leader möglich
- Belohnungen: Sieger-Allianz erhält Dauer-Boni (z. B. +10% Ressourcen)

## 5. Nächste Schritte

- **Mockups erstellen:** Rechner-Übersicht (Kachelansicht + Overlay), QTE-Prototypen
- **Balancing:** Bauzeiten, Upgrade-Kosten, QTE-Schwierigkeit
- **Event-Kalender:** Wöchentliche/Monatliche Events mit Belohnungsstruktur


