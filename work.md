# IoT Project Deliverable 1

## Question 1: Rose Greenhouse Optimal Growing Parameters

The table below summarizes the optimal environmental and soil conditions for rose cultivation in a greenhouse setting.

| Parameter | Optimal Value / Range | Source |
| --- | --- | --- |
| Temperature Range | Daytime: 65-75F (18-24C); Nighttime: 60-70F (15-21C) | DryGair |
| Relative Humidity Range | 70-80% RH | DryGair |
| Recommended Soil Type | Rich in organic matter and nutrients, with excellent drainage, especially loam soil | Kikwetu Flowers |
| Soil Moisture Content | Consistent water supply required; each plant needs an average of 0.7-1 litre per day, depending on variety and weather | Standard Media |
| Soil pH | pH 6-7 | Kikwetu Flowers |
| Sunlight Exposure | At least 6-8 hours of direct sunlight per day | GreenHouseinKenya |

### Sources

1. DryGair: https://drygair.com/blog/rose-greenhouse/
2. Kikwetu Flowers: https://www.kikwetuflowers.com/the-science-of-perfect-roses-how-altitude-soil-and-care-create-the-ultimate-bloom/
3. GreenHouseinKenya: https://greenhouseinkenya.co.ke/greenhouses-for-rose-flower-farming/
4. Standard Media: https://www.standardmedia.co.ke/farmkenya/article/2001438998/the-art-of-farming-roses-eleven-things-you-need-to-know

## Question 2: Rose Greenhouse Hardware Components

| Category | Component | Qty | Purpose |
| --- | --- | --- | --- |
| Microcontroller | ESP32S DevKit WiFi + BLE Module | 1 | Processes sensor data and transmits to the cloud via WiFi |
| Environmental Sensor | DHT22 (AM2302) Temperature and Humidity Sensor | 1 | Measures greenhouse temperature and relative humidity |
| Environmental Sensor | Capacitive Soil Moisture Sensor | 1 | Measures soil moisture to support irrigation decisions |
| Environmental Sensor | Soil pH Sensor Module | 1 | Measures soil pH and ensures it stays within pH 6-7 |
| Environmental Sensor | BH1750 Light Intensity Sensor (or LDR Module) | 1 | Measures sunlight/light intensity received by roses |
| Gas Sensor | MQ-5 LPG, Natural Gas, and Coal Gas Sensor | 1 | Detects LPG levels and possible gas leaks from the heating system |
| Display | 1.3 in White IIC 128x64 OLED LCD | 1 | Displays environmental readings locally |
| Control Component | 5V 1-Channel Relay Module | 1 | Controls external devices such as irrigation pumps or heating systems |
| Power Supply | 200W Solar Panel | 1 | Provides renewable energy to the monitoring system |
| Power Supply | 12V 100Ah Battery | 1 | Stores excess solar energy for continuous operation |
| Power Supply | DC-DC Buck Converter (12V to 5V/3.3V) | 1 | Steps down battery voltage for sensors and ESP32 |
| Power Supply | Voltage Regulator | 1 | Provides stable voltage and protects components |
| Circuit Component | 10k Resistor | Several | Pull-up resistor for DHT22 and signal stabilization |
| Circuit Component | Voltage Divider Resistors | Several | Protects ESP32 inputs from excessive voltage |
| Circuit Component | Capacitors (100nF and 10uF) | Several | Filters electrical noise and stabilizes power supply |
| Prototyping Tool | Breadboard | 1 | Enables solderless circuit prototyping |
| Prototyping Tool | Male-to-Male Jumper Wires | Several | Connects components on the breadboard |
| Prototyping Tool | Male-to-Female Jumper Wires | Several | Connects modules to the ESP32 |
| Prototyping Tool | USB Cable | 1 | Programming and powering the ESP32 during development |
| Prototyping Tool | Multimeter | 1 | Testing voltage, continuity, and troubleshooting |

## Question 3: Components and Datasheets

| Component | Datasheet |
| --- | --- |
| 1.3 in White IIC 128x64 OLED LCD Display | https://www.rajguruelectronics.com/Product/4437/OLED%204%20PIN%20128x64%20display%20module%201.3%20inch%20white.pdf |
| ESP32S DevKIT WiFi + BLE Module (30-Pin) | https://www.mouser.com/datasheet/2/891/esp-wroom-32_datasheet_en-1223836.pdf |
| DHT22 AM2302 Temperature and Humidity Sensor | https://www.berrybase.de/en/product-datasheet/019234a4258d7363b76c502b435342bc/create |
| MQ-5 LPG, Natural Gas, and Coal Gas Sensor | https://files.seeedstudio.com/wiki/Grove-Gas_Sensor-MQ5/res/MQ-5.pdf |
| 5V 1-Channel Low-Level Trigger Relay Module | https://handsontec.com/dataspecs/relay/1Ch-relay.pdf |

## Question 4A: Bill of Materials (BOM_EmbeddedIOT)

| ID | Name | Designator | Footprint | Qty | Manufacturer | Supplier | Supplier Part |
| --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | SSD1306-OLED-128X64-I2C | LCD1 | SSD1306-OLED-128X64-I2C | 1 | - | - | - |
| 2 | 2k Resistor | R1 | R805 | 1 | - | - | - |
| 3 | 1k Resistor | R2 | R805 | 1 | - | - | - |
| 4 | 10k Resistor | R3 | R805 | 1 | - | - | - |
| 5 | Grove - Gas Sensor (MQ5) | U1 | GROVE - GAS SENSOR(MQ5) | 1 | - | SeeedStudio | - |
| 6 | DHT22 | U3 | SENSOR-TH_HAIGU_DHT22 | 1 | HAIGU | LCSC | C2880291 |
| 7 | ESP32-DEVKITC | U4 | BULETM-SMD_ESP32-DEVKITC | 1 | ESPRESSIF | LCSC | C571180 |

## Question 4B: Bill of Materials (BOM_4B)

| ID | Name | Designator | Footprint | Qty | Supplier | Supplier Part |
| --- | --- | --- | --- | --- | --- | --- |
| 1 | Grove - Gas Sensor (MQ5) | U1 | GROVE - Gas Sensor(MQ5) | 1 | SeeedStudio | - |
| 2 | DHT22 | U3 | DHT22 | 1 | LCSC | C2880291 |
| 3 | ESP32-DEVKITC | U2 | ESP32-DEVKITC | 1 | LCSC | C571180 |
| 4 | ESP32-DEVKITC | U4 | ESP32-DEVKITC | 1 | LCSC | C571180 |
| 5 | 2k Resistor | R1 | R805 | 1 | - | - |
| 6 | 1k Resistor | R2 | R805 | 1 | - | - |
| 7 | 10k Resistor | R3 | R805 | 1 | - | - |

## Question 4C: Bill of Materials (Deliverable_1_4C)

| No. | Qty | Component | Designator | Footprint | Manufacturer Part | Manufacturer | Supplier Part | Supplier |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | 2 | 100nF Capacitor | C1, C2 | C0201 | - | - | - | - |
| 2 | 1 | 10k Resistor | R1 | R0603 | - | - | - | - |
| 3 | 2 | ESP32-C5-WROOM-1 | U1, U2 | COMM-SMD_37P-P1.27-L27.5-W18.0 | ESP32-C5-WROOM-1 | - | C9900205328 | LCSC |
| 4 | 1 | DHT22 | U4 | SENSOR-TH_HAIGU_DHT22 | DHT22 | HAIGU | C2880291 | LCSC |
| 5 | 1 | MQ-5 Gas Sensor | U5 | SENSOR-TH_MQ-5 | MQ-5 | Winsen | C99297 | LCSC |
| 6 | 1 | AZSR131-1AE-5D Relay | U6 | RELAY-TH_AZSR131-1AE-5D | AZSR131-1AE-5D | - | C9900008351 | LCSC |
