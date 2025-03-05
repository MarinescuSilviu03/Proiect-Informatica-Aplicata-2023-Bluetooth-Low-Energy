# Proiect Informatică Aplicată - ESP32 & Bluetooth LE

## Descriere
Acest proiect explorează utilizarea modulului **ESP32** pentru comunicarea fără fir prin **Bluetooth Low Energy (BLE)** și **WiFi**, cu scopul de a interoga un API și de a transmite date către o aplicație mobilă. Sistemul permite schimbul de date utilizând protocolul **HTTP** și **JSON** pentru a structura și transmite informații relevante.

## Tehnologii Utilizate
- **ESP32** - Microcontroler cu suport BLE și WiFi
- **Bluetooth Low Energy (BLE)** - Comunicare eficientă energetic între dispozitive
- **WiFi** - Conectivitate la rețea pentru interogarea API-ului
- **HTTP Client** - Solicitări către server pentru obținerea datelor
- **Arduino JSON** - Parsarea și formatarea datelor JSON
- **Arduino BLE Library** - Implementare BLE pe ESP32

## Funcționalități
1. **Inițializarea modulului ESP32**
   - Configurarea și pornirea serverului **BLE**
   - Crearea și gestionarea caracteristicilor BLE pentru schimbul de date

2. **Conectarea la WiFi**
   - Scanarea rețelelor disponibile și conectarea la o rețea WiFi

3. **Interogarea unui API extern**
   - Trimiterea cererilor HTTP către un server
   - Obținerea și parsarea răspunsurilor JSON
   - Extragerea informațiilor relevante din API

4. **Transmiterea datelor prin Bluetooth LE**
   - Dispozitivul ESP32 primește cereri de la un client BLE
   - Răspunde cu date JSON structurate, obținute de la API

5. **Gestionarea conexiunilor BLE**
   - Detectarea conectării și deconectării dispozitivelor
   - Notificarea clientului BLE asupra schimbărilor de stare

## Instalare și Utilizare
### 1. Configurarea ESP32
- Instalați **Arduino IDE** și adăugați suportul pentru ESP32
- Instalați bibliotecile necesare: `ArduinoJson`, `WiFi`, `BLEDevice`, `HTTPClient`
- Încărcați codul pe placa **ESP32**

### 2. Testarea conexiunii
- Asigurați-vă că API-ul este accesibil
- Conectați un dispozitiv BLE (ex. telefon, alt ESP32) și solicitați date
- Monitorizați răspunsurile prin **Serial Monitor**

## Concluzie
Acest proiect demonstrează integrarea **ESP32**, **WiFi**, **BLE** și **API-uri HTTP**, facilitând comunicarea eficientă între dispozitive. BLE este utilizat pentru transfer rapid și eficient energetic, în timp ce WiFi permite obținerea datelor de la un server. Această soluție poate fi extinsă pentru automatizări, IoT sau aplicații de monitorizare.

## Bibliografie
- [Espressif ESP32 Docs](https://www.espressif.com/)
- [Arduino JSON](https://arduinojson.org/)
- [Bluetooth SIG](https://www.bluetooth.com/)

