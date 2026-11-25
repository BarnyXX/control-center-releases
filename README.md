# Control Center – Installer

Hier liegen nur die fertigen Installer des Control Centers (Steuerung für RGB-Beleuchtung, Lüfter und Displays unter
Windows). Der Quellcode ist nicht öffentlich.

## Installieren

1. Unter **[Releases](../../releases/latest)** die Datei **ControlCenter-Setup.exe** herunterladen.
2. Ausführen. Der Installer ist nicht mit einem Zertifikat signiert – Windows SmartScreen fragt deshalb einmal nach:
   „Weitere Informationen“ → „Trotzdem ausführen“.
3. Der Ziel-PC braucht kein .NET. Deinstallieren geht über Windows → Einstellungen → Apps.

## Updates

Ab Version 1.0.622 aktualisiert sich das Control Center selbst: Es sucht alle sechs Stunden hier nach einer neuen
Version und installiert sie (nie während eines Spiels; Einstellungen bleiben erhalten). Abschalten lässt sich das unter
Einstellungen → Allgemein → Updates.

Jede Version trägt neben dem Installer eine Signatur (`ControlCenter-Setup.exe.sig`). Das Control Center installiert
nur Dateien, deren Signatur zum eingebauten Schlüssel passt – ein Installer, der hier ausgetauscht würde, wird nicht
installiert.
