# Lobby Plugin für BungeeCord

Das Lobby Plugin für BungeeCord ermöglicht eine nahtlose Kommunikation zwischen dem BungeeCord-Server und dem Lobby-Server. Es bietet grundlegende Funktionen für die Verwaltung der Lobby-Umgebung und verbessert das Spielerlebnis.

## Inhaltsverzeichnis

- [Features](#features)
- [Technologien](#technologien)
- [Installation](#installation)
- [Konfiguration](#konfiguration)
- [Verwendung](#verwendung)
- [Beitrag leisten](#beitrag-leisten)
- [Lizenz](#lizenz)

## Features

- Verbindung zwischen BungeeCord- und Lobby-Server
- Spieler-Management (z. B. Teleportation, Statusanzeigen)
- Anpassbare Lobby-Umgebung
- Einfache Konfiguration über die `config.yml`

## Technologien

- [Java](https://www.oracle.com/java/technologies/javase-jdk11-downloads.html)
- [BungeeCord](https://www.spigotmc.org/wiki/bungeecord/)
- [Maven](https://maven.apache.org/) (für das Build-Management)

## Installation

1. Klone das Repository:

   ```bash
   git clone https://github.com/deinbenutzername/lobby-plugin.git
   cd lobby-plugin
   ```

2. Baue das Plugin mit Maven:

   ```bash
   mvn clean package
   ```

3. Kopiere die generierte JAR-Datei aus dem `target`-Ordner in den `plugins`-Ordner deines BungeeCord-Servers.

## Konfiguration

Die Konfiguration erfolgt über die `config.yml`, die im `plugins/LobbyPlugin`-Ordner generiert wird. Hier kannst du die Einstellungen für die Kommunikation zwischen dem BungeeCord-Server und dem Lobby-Server anpassen:

```yaml
bungeecord:
  host: "localhost"
  port: 25577

lobby:
  server-name: "Lobby"
  max-players: 100
```

## Verwendung

Starte deinen BungeeCord-Server und den Lobby-Server. Stelle sicher, dass die `config.yml` korrekt konfiguriert ist. Spieler können dann in die Lobby teleportiert werden und das Plugin wird die Kommunikation zwischen den Servern verwalten.

## Beitrag leisten

Beiträge sind willkommen! Bitte öffne ein Issue oder erstelle einen Pull Request, um Ideen oder Verbesserungen vorzuschlagen.

## Lizenz

Dieses Projekt steht unter der MIT-Lizenz. Siehe die [LICENSE](LICENSE)-Datei für weitere Informationen.