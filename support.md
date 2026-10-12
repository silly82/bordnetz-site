---
title: Bordnetz – Support
permalink: /support/
---

# Bordnetz – Support

**Contact:** [bordnetz@zwx.ch](mailto:bordnetz@zwx.ch)

## Getting started

1. You need a Victron GX device (for example a Cerbo GX) with **Venus OS Large** and Node-RED switched on.
2. Install the **Bordnetz flow** in Node-RED and set your devices and an access token: step by step in the [setup guide](https://github.com/silly82/bordnetz-nodered#install).
3. Open Bordnetz → Settings and enter the address `https://<GX address>:1881/api/camper/status`, the token and the certificate fingerprint (**Read From Server**, then compare). Quicker: scan a setup code made with the guide's `setup-qr.swift`, with the Camera app or with **Scan Setup Code** in the settings.
4. Optional: a Victron VRM access token for the history and for values while the GX is out of reach (VRM portal → Preferences → Integrations → Access tokens). Bordnetz learns which devices to read there on the first connection to the GX.

Want to look around first? Tap **Try Demo** on the first screen.

## Common questions

- **No connection.** The iPhone must be in the vehicle's network, or connected to it, for example through Tailscale. The address ends in `/api/camper/status` and uses port 1881.
- **"The token was not accepted (401)."** The token in the app differs from `IOS_API_TOKEN` on the tab in Node-RED. Paste it rather than typing it.
- **Certificate error after a GX update or reset.** The GX may have a new certificate: read the fingerprint from the server again and compare it.
- **A row is missing** (solar, shore power, temperatures, door). Bordnetz shows only what the flow reports; set the device in the tab's environment variables and deploy again.
- **Siri and Control Center.** Say for example "How full is the battery in Bordnetz?" or "Turn on away mode in Bordnetz". Away mode is also a control for Control Center, the Lock Screen and the Action button.

---

# Bordnetz – Support (Deutsch)

**Kontakt:** [bordnetz@zwx.ch](mailto:bordnetz@zwx.ch)

## Erste Schritte

1. Du brauchst ein Victron-GX-Gerät (zum Beispiel einen Cerbo GX) mit **Venus OS Large** und eingeschaltetem Node-RED.
2. Installiere den **Bordnetz-Flow** in Node-RED und trag deine Geräte und ein Zugangstoken ein: Schritt für Schritt in der [Anleitung](https://github.com/silly82/bordnetz-nodered#deutsch).
3. Öffne Bordnetz → Einstellungen und trag die Adresse `https://<GX-Adresse>:1881/api/camper/status`, das Token und den Fingerabdruck des Zertifikats ein (**Vom Server lesen**, dann vergleichen). Schneller: einen Einrichtungscode scannen, den du mit `setup-qr.swift` aus der Anleitung erzeugst, mit der Kamera-App oder mit **Einrichtungscode scannen** in den Einstellungen.
4. Optional: ein Zugangstoken für Victron VRM für den Verlauf und für Werte, wenn das GX nicht erreichbar ist (VRM-Portal → Preferences → Integrations → Access tokens). Welche Geräte Bordnetz dort liest, lernt es bei der ersten Verbindung zum GX.

Zuerst umschauen? Tippe auf dem ersten Bildschirm auf **Demo ausprobieren**.

## Häufige Fragen

- **Keine Verbindung.** Das iPhone muss im Netzwerk des Fahrzeugs sein oder damit verbunden, zum Beispiel über Tailscale. Die Adresse endet auf `/api/camper/status` und nutzt Port 1881.
- **„Das Token wurde nicht akzeptiert (401).“** Das Token in der App weicht von `IOS_API_TOKEN` am Tab in Node-RED ab. Füg es ein, statt es abzutippen.
- **Zertifikatsfehler nach einem Update oder Reset des GX.** Das GX hat vielleicht ein neues Zertifikat: Fingerabdruck erneut vom Server lesen und vergleichen.
- **Eine Zeile fehlt** (Solar, Landstrom, Temperaturen, Tür). Bordnetz zeigt nur, was der Flow meldet; trag das Gerät in den Umgebungsvariablen des Tabs ein und mach erneut ein Deploy.
- **Siri und Kontrollzentrum.** Sag zum Beispiel „Wie voll ist die Batterie in Bordnetz?“ oder „Schalte Abwesend in Bordnetz ein“. „Abwesend“ gibt es auch als Steuerelement für Kontrollzentrum, Sperrbildschirm und Aktionstaste.
