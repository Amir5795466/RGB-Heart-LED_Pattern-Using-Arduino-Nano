# RGB-LED-Heart_Pattern-Using-Arduino-Nano
❤️ **LED Heart Pattern Using Arduino Nano**  Create a beautiful heart-shaped LED lighting pattern using Arduino Nano. This beginner-friendly electronics project demonstrates LED control, sequential blinking, and creative lighting effects using simple Arduino programming. Perfect for learning electronics and exploring DIY Arduino projects! ⚡
_________________________________________________________________________________
----------------------------------------------------------------
# LED position map (seen from the BACK)
<img width="2752" height="1536" alt="LED_position_map" src="https://github.com/user-attachments/assets/e63967b3-6fa6-4f04-92cb-854f35658243" />

-----------------------------------------------------------------

## 🔌 Circuit Block Diagram

```mermaid
flowchart LR
    A["3.7V LiPo Battery"] --> C["TP4056 Module<br/>Charger + DW01 Protection"]
    B["USB Charging"] --> C

    C --> D["ON/OFF Slide Switch"]

    D --> E["MT3608 Boost Converter<br/>Set to 5.1V"]
    D --> F["10kΩ Resistor"]

    E --> G["VOUT+ → 5V Pin"]
    F --> H["A6 Battery Sense"]

    G --> I["Arduino Nano"]
    H --> I
    J["Push Button"] --> I

    I --> K["16 × 220Ω Resistors"]
    K --> L["16 LEDs"]

    style A fill:#263b59,color:#fff,stroke:#60a5fa
    style C fill:#174b42,color:#fff,stroke:#34d399
    style E fill:#65451b,color:#fff,stroke:#fbbf24
    style I fill:#174b42,color:#fff,stroke:#34d399
    style L fill:#542b63,color:#fff,stroke:#c084fc
```


--------------------------------------------------------------------
- The TP4056 charges the LiPo over USB and protects it from over-charge, over-discharge and shorts.
- The slide switch turns everything on and off.
- The MT3608 boosts the battery's 3.0–4.2 V up to a steady ~5.1 V, which goes straight into the Nano's 5V pin.
- Each of the 16 LEDs has its own pin and its own 220 Ω resistor, so every LED can be controlled on its own.
- A 10 kΩ resistor feeds the battery voltage into A6. The code reads it and shuts the LEDs off before the battery gets too low.
- The push button on D2 goes to GND and switches between the light modes.
-----------------------------------------------------------------------
# Nano pinout (seen from the BACK)
<img width="2752" height="1536" alt="Arduino pin out" src="https://github.com/user-attachments/assets/14621d46-66e8-4718-bac5-7db84003ef05" />

-----------------------------------------------------------------------
# Arduino_Nano Wiring with LEDs Positions 
<img width="2752" height="1536" alt="Arduino nano wiring" src="https://github.com/user-attachments/assets/4009cbe6-2c41-4aec-b6c7-b4533fa917f6" />

------------------------------------------------------------------------
# Full Circuid Diagram
[heart_led_portable (1).pdf](https://github.com/user-attachments/files/34896030/heart_led_portable.1.pdf)

------------------------------------------------------------------------
# Code
[Uploading LED_Heart_Arduino_Code.ino…]()


