# Starbie

<img width="624" height="612" alt="Screenshot 2026-10-16 at 16 43 54" src="https://github.com/user-attachments/assets/8842b9bb-8ee1-405f-b50e-f9c2164441bb" />


This is a variation of the starbie project by Hackclub's Half life, made by me d3wzs. It has a refinded design of the original with a beautiful handmade star design based off old tomagochis. 

Starbie feautures a display, 2 buttons, in multiple layouts, an 0.96" oled as a screen, and a esp32 mini as the main controller. There are various other compenents that aernt as important that you can read of in the repository. 

# Features/Attributes

- Motion Sensing - MPU6050
- Enviromental Sensing - DHT11
- Physical Controls
- OLED display - 0.96" I2C OLED
- Star themed design
- Custom PCB

# Hardware

 - Seeed Studio XIAO ESP32-C3: Main contoller
 - 0.96-inch OLED display: display output
 - MPU6050: Motion Sensing
 - DHT11: Tempature & Humidity Sensing
 - 2× MX mechanical switches: Input
 - 2× keycaps: Cap for switches
 - Custom PCB: does this need explanation?
If you want more specifics refer to the BOM.

# Repository Guide

- Starbie-Code.ino — Main arduino Code
- Starbie-BOM.csv — bill om materials csv format
- BOM.md — bill of materials
- JOURNAL.md — project journal
- Gerbers/ — Manufacturing files, subfiles for each type
- Starbie-Design-Files/ — Design files, subfiles for each type

# Bill of Materials 

| Part | What it's for | Qty | Unit | Total | Vendor |
| --- | --- | --- | --- | --- | --- |
| [XIAO ESP32 C3](https://www.seeedstudio.com/Seeed-XIAO-ESP32C3-p-5431.html) | Main loop | 1 | $4.90 | $4.90 | [Seeedstudio](https://www.seeedstudio.com/Seeed-XIAO-ESP32C3-p-5431.html) |
| [0.96 OLED](https://www.amazon.com/dp/B0GBVWBWCR) | displaying | 1 | $5.99 | $5.99 | [Amazon](https://www.amazon.com/dp/B0GBVWBWCR) |
| [MPU6050](https://www.amazon.com/2PCS-Unsoldered-GY-521-MPU6050-Sensor/dp/B0H9JC8XZL/ref=sr_1_2?crid=2HMTTL0FXLVPM&dib=eyJ2IjoiMSJ9.GF7DFQi9gd8NKhx6V_Kx54zE7G-pUFaHGTFdI1bxn1lgIBWtABC80ZyLosDUxkiX.h0fwC8JUvUMM8VidYFL0DKhmxQGWfempETLgqr9Nq1g&dib_tag=se&keywords=gpu6050+sensor&qid=1791505260&refinements=p_36%3A-700&rnid=386419011&sprefix=gpu6050+sensor%2Caps%2C205&sr=8-2) | sensing movement | 1 | $2.79 | $2.79 | [Amazon](https://www.amazon.com/2PCS-Unsoldered-GY-521-MPU6050-Sensor/dp/B0H9JC8XZL/ref=sr_1_2?crid=2HMTTL0FXLVPM&dib=eyJ2IjoiMSJ9.GF7DFQi9gd8NKhx6V_Kx54zE7G-pUFaHGTFdI1bxn1lgIBWtABC80ZyLosDUxkiX.h0fwC8JUvUMM8VidYFL0DKhmxQGWfempETLgqr9Nq1g&dib_tag=se&keywords=gpu6050+sensor&qid=1791505260&refinements=p_36%3A-700&rnid=386419011&sprefix=gpu6050+sensor%2Caps%2C205&sr=8-2) |
| [DHT11](https://www.amazon.com/DHT-11-Digital-Temperature-Humidity-Arduino/dp/B0CRRXJ83F/ref=sr_1_11?crid=2CNQQ9VELYPKC&dib=eyJ2IjoiMSJ9.jRSeQ30kq_FIRLdvzNBOTkG9lhTC7lqueY-WplO9vzdyS3axrLQ5ovrcqE3y-dMG45Owu31GS7zptNVYy-Qvr5Djb8cpKJDHsCVGwkWqUstcx78q6lAJXwa_djHd2QKHxRJ5STrJP4CyG4VnJt7Vp1Z65GgB1SFLT9Oh2QcGg5n1ArHCLkeut7mqQ16zuJ456UtGp4vFo_73PKqRE00SskDj9HQD4URfETLdTPWzPwY.6n38OWLCKTZAzOoG0wdhrUb9RzbIEsuz5yCTbQYJdZM&dib_tag=se&keywords=dht11+sensor&qid=1791505191&refinements=p_36%3A-600&rnid=2661611011&sprefix=dht11+sensor%2Caps%2C225&sr=8-11) | sensing temp/humidity | 1 | $3.78 | $3.78 | [Amazon](https://www.amazon.com/DHT-11-Digital-Temperature-Humidity-Arduino/dp/B0CRRXJ83F/ref=sr_1_11?crid=2CNQQ9VELYPKC&dib=eyJ2IjoiMSJ9.jRSeQ30kq_FIRLdvzNBOTkG9lhTC7lqueY-WplO9vzdyS3axrLQ5ovrcqE3y-dMG45Owu31GS7zptNVYy-Qvr5Djb8cpKJDHsCVGwkWqUstcx78q6lAJXwa_djHd2QKHxRJ5STrJP4CyG4VnJt7Vp1Z65GgB1SFLT9Oh2QcGg5n1ArHCLkeut7mqQ16zuJ456UtGp4vFo_73PKqRE00SskDj9HQD4URfETLdTPWzPwY.6n38OWLCKTZAzOoG0wdhrUb9RzbIEsuz5yCTbQYJdZM&dib_tag=se&keywords=dht11+sensor&qid=1791505191&refinements=p_36%3A-600&rnid=2661611011&sprefix=dht11+sensor%2Caps%2C225&sr=8-11) |
| [MX Switches](https://www.amazon.com//dp/B0FQP8VYX4) | clicking/interacting | 2 | $0.18 | $0.36 | [Amazon](https://www.amazon.com//dp/B0FQP8VYX4) |
| [Keycaps](https://www.amazon.com/dp/B0CQ2XG16M?th=1) | making keys pleasent to click | 2 | $0.60 | $1.20 | [Amazon](https://www.amazon.com/dp/B0CQ2XG16M?th=1) |
| [PCB](https://www.jlcpcb.com/) | connecting parts | 1 | $4.00 | $4.00 | [JLCPCB](https://www.jlcpcb.com/) |
| **Parts subtotal** | — | — | — | **$23.02** | — |
| **Tax & shipping** | — | — | — | **$2.76** | — |
| **Total** | — | — | — | **$25.78** | — |


# Media

<img width="1220" height="860" alt="Screenshot 2026-10-16 at 16 44 41" src="https://github.com/user-attachments/assets/0ddde10b-3edb-4513-9d0d-9e0003909ae7" />
Schematic

<img width="631" height="614" alt="Screenshot 2026-10-16 at 16 44 12" src="https://github.com/user-attachments/assets/59504576-169e-4be7-b968-9106cdfb9769" />
Back of PCB

<img width="624" height="612" alt="Screenshot 2026-10-16 at 16 43 54" src="https://github.com/user-attachments/assets/40761e03-f67a-4d44-8644-b668d1781dc9" />
Front of PCB

<img width="571" height="695" alt="Screenshot 2026-10-16 at 16 43 43" src="https://github.com/user-attachments/assets/59dbf13c-ea81-43e9-b448-334b63b518a5" />
Back Routing

<img width="578" height="630" alt="Screenshot 2026-10-16 at 16 43 30" src="https://github.com/user-attachments/assets/5295ee02-363f-4aa3-8481-b39fb9ee5073" />
Front Routing


sorry for the formating, im not sure how to fix it

# Author

Big thanks to Hack Club, they did all of the hard work thinking this up. I just made my own version =)
- d3wzs(d3wzy)
- Hack Club

Thanks for checking out my Starbie repo
