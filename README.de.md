🧵 FilaTrack – Günstiger Wifi-Filament-Manager

Ein leichtgewichtiges, webbasiertes Filament-Managementsystem, speziell für den ESP32 entwickelt. Verwalte mühelos deine 3D-Druckmaterialien, behalte den Überblick über Restbestände und drucke QR-Code-Etiketten direkt von deinem Mikrocontroller.
✨ Features

    ESP32-Unterstützung: Volle Kompatibilität mit der ESP32-Familie (S3, C3, C6 und klassischer ESP32).

    Web-Interface: Vollständig responsives UI mit Unterstützung für Dark & Light Mode, optimiert für Desktop und Mobilgeräte.

    QR-Code-Generator: Erstelle Etiketten für deine Spulen, die direkt zum Bearbeitungsmenü des jeweiligen Filaments verlinken.

    Bestandsmanagement: Speichere bis zu 250 Filamente mit Details wie Hersteller, Material, Farbe, Temperatureinstellungen und Gewicht.

    Verbrauchsrechner: Subtrahiere nach dem Druck einfach das verbrauchte Gewicht, um deinen Bestand präzise zu halten.

    Smarter Fortschrittsbalken: Ein farbcodierter Balken auf jeder Filament-Karte schrumpft automatisch mit sinkendem Restgewicht.

    Übersicht: Der Balken zeigt den Prozentsatz des verbleibenden Filaments an (basierend auf einer 1kg-Standardspule) – so siehst du sofort, welche Spulen leer werden.

    WiFi Captive Portal: Mühelose WLAN-Konfiguration über einen dedizierten Setup-Access-Point.

    Backup & Wiederherstellung: Lade deine gesamte Datenbank als Binärdatei herunter und stelle sie bei Bedarf jederzeit wieder her.

    30-Tage-Backup-Erinnerung: Der Tracker überwacht automatisch die Zeit seit deinem letzten Datenexport.

    Mehrsprachig: Unterstützt Deutsch und Englisch.

🏷️ Smarte QR-Code-Etiketten & Export

Der ESP Filament Tracker speichert nicht nur Daten; er schlägt die Brücke zwischen deinem digitalen Inventar und deinen physischen Spulen. Jeder Filamenteintrag kann ein individuelles, druckfertiges Etikett generieren.
Was steht auf dem Etikett?

Das generierte Etikett ist auf Klarheit optimiert und enthält alle wesentlichen Informationen für einen erfolgreichen Druck:

    Hersteller & Material: Großer, fettgedruckter Text zur schnellen Identifizierung.

    Dynamischer QR-Code: Ein scannbarer Code, der direkt zur Bearbeitungsseite des spezifischen Filaments auf deinem ESP32 verlinkt.

    Temperaturprofile: Gedruckte Werte für Düsen- (Hotend) und Druckbettbereiche.

    Druckfertiges Format: Ein klares Schwarz-Weiß-Design, optimiert für Standard-Thermodrucker oder normales Papier.

Wie es deinen Workflow verbessert

    Sofortiger Zugriff: Anstatt eine lange Liste zu durchsuchen, scanne einfach den QR-Code auf der physischen Spule mit deiner Smartphone-Kamera.

    Direktes Bearbeiten: Der Scan führt dich direkt zur Bearbeitungsseite, auf der du sofort das nach dem Druck verbrauchte Gewicht abziehen kannst.

    Kein Raten mehr: Alle technischen Daten (Temperaturen) sind physisch an der Spule angebracht, sodass du nie wieder die Spezifikationen des Herstellers heraussuchen musst.

🛠 Hardware-Anforderungen

    Mikrocontroller: ESP32-Serie (S3, C3, C6 oder Standard-ESP32).

    Speicher: Verwendet SPIFFS (Serial Peripheral Interface Flash File System) für die interne Datenspeicherung.

🚀 Installation
1. Web Flasher

Besuche den Web Flasher, wähle dein spezifisches Board aus und klicke auf Installieren.
2. Erstmalige Einrichtung (WiFi)

    Nach dem Flashen erstellt der ESP einen WLAN-Access-Point namens Filament-Tracker-Setup.

    Verbinde dich mit diesem Netzwerk über dein Smartphone oder deinen PC.

    Die Setup-Seite sollte sich automatisch öffnen (Captive Portal). Wähle dein Heim-WLAN aus und gib das Passwort ein.

    Der ESP startet neu und verbindet sich mit deinem Netzwerk. Er ist nun über seine zugewiesene IP-Adresse erreichbar.

📂 Dateistruktur & Datenspeicherung

Der Tracker verwaltet zwei Hauptdateien im internen Flash-Speicher:

    /wifi.txt: Speichert deine verschlüsselten WLAN-Zugangsdaten.

    /data.bin: Eine Binärdatei, die das gesamte Filament-Inventar enthält (struct Filament).

🖥 Screenshots / UI

    Dashboard: Übersicht aller Spulen mit visuellen Fortschrittsbalken für das verbleibende Filament.

    Bearbeitungsmodus: Anpassen von Temperaturen, Gewichten und Herstellerdetails.

    QR-Etikett: Eine druckfertige Ansicht für die physische Beschriftung deiner Filament-Regale oder Spulen.

📝 Lizenz

Dieses Projekt wird unter der MIT-Lizenz veröffentlicht. Du darfst es frei für private und kommerzielle Zwecke verwenden, modifizieren und verbreiten.
