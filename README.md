# 🚨 Frigate Telegram Notify 🚀

Un Blueprint per Home Assistant per ricevere notifiche Telegram (Snapshot e Clip) direttamente da Frigate. 

## ✨ Caratteristiche Principali

* 👥 **Supporto Multi-ID:** Vuoi mandare l'allarme a te e a tua moglie? Inserisci i `chat_id` separati da virgola. Il bot invierà la notifica a tutti senza dover creare gruppi Telegram appositi.
* 🎛️ **Toggle "Opt-In":** Foto, Video e Notifiche Silenziose sono controllati da interruttori (spenti di default). Decidi tu cosa attivare, senza sorprese.
* ✍️ **Testo 100% Personalizzabile:** Basta coi messaggi robotici. Scrivi tu il testo della notifica supportando le variabili (es. `🚨 Rilevato {{ label }} dalla telecamera: {{ camera_name }}`).

## 📋 Prerequisiti

Per usare questo blueprint devi avere:
1.  **Home Assistant** funzionante.
2.  L'integrazione **Frigate** e un broker **MQTT** (es. Mosquitto) configurati.
3.  L'integrazione **Telegram** configurato e funzionante 

## ⚙️ Come si configura (Attenzione ai dettagli!)

Quando crei l'automazione da questo blueprint, fai attenzione a questi due campi fondamentali per non far fallire l'automazione:

1.  **Nome Telecamera Frigate:** Inserisci il nome **ESATTO** così come lo legge Frigate via MQTT, rispettando rigorosamente le MAIUSCOLE e minuscole (es. se su Frigate si chiama `Cancello` con la C maiuscola, scrivi `Cancello`, altrimenti l'automazione la ignorerà).
2.  **URL Base Home Assistant:** Inserisci l'indirizzo del tuo Home Assistant completo di porta (es. `http://192.168.1.100:8123` oppure il tuo indirizzo DuckDNS/NabuCasa). Questo serve a Home Assistant per trovare fisicamente i file immagine e video da inviare ai server di Telegram.

## 📥 Installazione

Importa il Blueprint sul tuo Home Assistant tramite il seguente link:

[![Importa Blueprint in Home Assistant](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https://raw.githubusercontent.com/SalvatoreITA/domhouse-octopus-card/main/blueprints/octopus_tracker_luce.yaml)

## ☕ Supporta il Progetto

Ogni piccolo supporto fa un'enorme differenza: mi aiuta a mantenere vivo l'entusiasmo e mi stimola a creare e condividere nuove soluzioni per la community. Grazie di cuore per il tuo aiuto! 🚀

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/salvatore_dh)

## ❤️ Crediti
Sviluppato da [Salvatore Lentini - DomHouse.it](https://www.domhouse.it)
