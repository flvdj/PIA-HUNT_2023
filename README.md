# ESP32 Bluetooth Communication - PIAHUNT 2023

## Descriere
Acest proiect reprezintă implementarea unei comunicări Bluetooth între două dispozitive **ESP32**, unde unul acționează ca **Master**, iar celălalt ca **Slave**. Codul prezentat este pentru **Master** și are rolul de a transmite și procesa datele primite prin Bluetooth. Proiectul a fost realizat pentru **concursul PIAHUNT 2023**, unde a obținut **Premiul 2**.

## Autori
- **Nistor Flaviu-Cristian**
- **Marinescu Silviu-Andrei**
- **Grupa:** 412B, **UNSTPB București**
- **Profesor coordonator:** Dr. Ing. Prof. Bogdan Florea

## Tehnologii utilizate
- **ESP32** - Microcontroler cu suport Bluetooth.
- **BluetoothSerial Library** - Permite comunicarea Bluetooth între dispozitive ESP32.
- **CRC16** - Algoritm utilizat pentru verificarea integrității datelor transmise.
- **Arduino IDE** - Platforma de dezvoltare și testare a codului.

## Funcționalități implementate
1. **Inițializare ESP32 Master** pentru comunicare Bluetooth.
2. **Conectare la dispozitivul Slave** folosind numele „PHNT3”.
3. **Trimiterea unei comenzi de verificare** (`AT+U322`) către Slave.
4. **Primirea și procesarea datelor** de la dispozitivul Slave.
5. **Calcularea unui checksum CRC16** pentru verificarea integrității datelor.
6. **Reconectare automată** în cazul pierderii conexiunii.

## Instalare și utilizare
1. **Clonați repository-ul:**
   ```bash
   git clone https://github.com/username/repository.git
   ```
2. **Configurați mediul de dezvoltare:**
   - Instalați **Arduino IDE**.
   - Adăugați **ESP32 Board Manager**.
   - Instalați librăriile necesare (`BluetoothSerial`, `CRC16`).
3. **Încărcați codul pe ESP32 Master** folosind Arduino IDE.
4. **Asigurați-vă că dispozitivul Slave este pornit** și accesibil prin Bluetooth.
5. **Monitorizați serial output-ul** pentru a vedea datele transmise și primite.

## Exemplu de Output
```
The device "ESP32-BT-Master" started in master mode, make sure slave BT device is on!
Connecting to slave BT device named "PHNT3"
Connected Successfully!
Received data: 1234
Processed Data: 2111CRC_OK
Reconnecting...
Reconnected Successfully!
```

## Concluzii
Acest proiect demonstrează utilizarea **ESP32 și Bluetooth** pentru realizarea unei comunicări eficiente între dispozitive, având aplicații practice în **sisteme IoT, automatizări și securitate**. Codul a fost optimizat pentru performanță și fiabilitate, incluzând mecanisme de **reconectare automată și verificare a integrității datelor**.

## Licență
Acest proiect a fost realizat în cadrul **Universității Naționale de Știință și Tehnologie Politehnica București, Facultatea de Electronică, Telecomunicații și Tehnologia Informației**, pentru **concursul PIAHUNT 2023**.

