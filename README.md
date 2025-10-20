# ZMK Config – Kabelloses Numpad mit Mediensteuerung

Dieses Repository enthält die ZMK-Konfiguration für ein kabelloses Numpad auf Basis des Tidbit-Keypads.

## Features

- 🔊 Mediensteuerung (Mute, Prev, Next, Play/Pause via Encoder)
- 🎚️ Rotary Encoder für Lautstärke und Play/Pause
- 🔢 Standard-Numpad mit Numlock, Operatoren und Zahlen
- ⌨️ Shift-Funktionen auf Layer 1 (Navigation, Sonderzeichen)
- 🧠 Kompatibel mit externer Layer-Aktivierung via Companion-Tastatur

## Layout-Datei

Die Keymap befindet sich in [`config/tidbit.keymap`](config/tidbit.keymap)

## Encoder-Funktionen

- Drehung: Lautstärke hoch/runter
- Klick: Play/Pause (Layer-Tap auf Func Layer)

## Kompilierung

```bash
west build -d build -b <board> -- -DSHIELD=tidbit_numpad
