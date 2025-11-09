# 🎶 MP3 Metadata Reader & Editor – Tomáš Šmíd

## 📘 Popis projektu
Tento projekt byl vytvořen jako úkol pro lekci **Práce s daty – formát MP3**.  
Cílem programu je:
- načíst metadata z MP3 souboru pomocí knihovny **Mutagen**,  
- vypisovat je přehledně do konzole,  
- a jako **bonus** vytvořit **kopii MP3 souboru** s metadaty (bez změny originálu).

---

## 🧠 Použité technologie
- **Python 3.11+**
- **Mutagen** – knihovna pro čtení a zápis ID3 tagů MP3 souborů  
- **os, shutil** – práce se soubory a kopiemi

---

## ⚙️ Instalace knihovny
Před spuštěním je nutné nainstalovat knihovnu `mutagen`:

```bash
pip install mutagen
```

## 🚀 Spuštění programu

Ujisti se, že máš v adresáři se skriptem MP3 soubor
např. let_the_world_burn(hoodtrap_mylancore_remix).mp3

Ulož skript jako mp3_metadata_Smid.py

Spusť příkaz: 
```bash
python mp3_metadata_Smid.py
```

## 🧾 Co skript dělá

Načte a vypíše metadata z MP3 (název, interpret, album, bitrate, délka).
Zobrazí přehled všech ID3 tagů nalezených v souboru.
Zeptá se uživatele, zda chce vytvořit kopii souboru metadaty.
Vytvoří kopii souboru s příponou _upraveno.mp3, kam uloží údaje.
Znovu načte a vypíše nová metadata z kopie, aby bylo vidět, že úprava proběhla úspěšně.

## 📊 Ukázkový výstup
🎵 Informace o souboru: let_the_world_burn(hoodtrap_mylancore_remix).mp3
📏 Délka skladby: 210.32 sekund
📡 Bitrate: 320 kbps

🧾 Metadata:
  artist    : Hoodtrap
  title     : Let The World Burn
  album     : The Hood Mixtape
  genre     : Electronic
  date      : 2024

💾 Nový soubor s upravenými metadaty vytvořen: let_the_world_burn(hoodtrap_mylancore_remix)_upraveno.mp3

✅ Metadata v novém souboru:
🎵 Informace o souboru: let_the_world_burn(hoodtrap_mylancore_remix)_upraveno.mp3
📏 Délka skladby: 210.32 sekund
📡 Bitrate: 320 kbps

🧾 Metadata:
  artist    : Hoodtrap x Mylancore
  title     : Let The World Burn (Remix)
  album     : Python Demo Album
  genre     : Electronic
  date      : 2025


