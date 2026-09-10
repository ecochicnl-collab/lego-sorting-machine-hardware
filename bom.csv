import pandas as pd

# Translate the table to English and verify the grand total
data_english = [
    {"Category": "Computing & Vision", "Item": "Raspberry Pi 5 (8GB RAM)", "Status": "To Buy", "Quantity": 1, "Price": 80.00},
    {"Category": "Computing & Vision", "Item": "High-Res USB/CSI Cameras (top & bottom)", "Status": "To Buy", "Quantity": 2, "Price": 18.00},
    {"Category": "Computing & Vision", "Item": "High-brightness LED Lighting & Diffuser", "Status": "To Buy", "Quantity": 1, "Price": 14.00},
    {"Category": "Computing & Vision", "Item": "WS2812B Addressable LED Strip", "Status": "To Buy", "Quantity": 1, "Price": 12.00},
    {"Category": "Electronics & Power", "Item": "ESP32 Microcontroller (additional)", "Status": "To Buy", "Quantity": 1, "Price": 6.00},
    {"Category": "Electronics & Power", "Item": "Stepper Motor Drivers (TMC2209/DRV8825)", "Status": "To Buy", "Quantity": 3, "Price": 5.00},
    {"Category": "Electronics & Power", "Item": "VL53L1X ToF Distance Sensors (~1m)", "Status": "To Buy", "Quantity": 2, "Price": 10.00},
    {"Category": "Electronics & Power", "Item": "Cabling, power supplies & jumpers", "Status": "To Buy", "Quantity": 1, "Price": 25.00},
    {"Category": "Actuators & Mechanics", "Item": "Precision High-Torque Stepper Motors (Lift)", "Status": "To Buy", "Quantity": 2, "Price": 18.00},
    {"Category": "Actuators & Mechanics", "Item": "Mini Servo Motor", "Status": "To Buy", "Quantity": 1, "Price": 5.00},
    {"Category": "Actuators & Mechanics", "Item": "Small Stepper Motor (Cart)", "Status": "To Buy", "Quantity": 1, "Price": 10.00},
    {"Category": "Actuators & Mechanics", "Item": "Small Auxiliary Motor", "Status": "To Buy", "Quantity": 1, "Price": 8.00},
    {"Category": "Actuators & Mechanics", "Item": "Basic Train Motor & Servo (Wagons)", "Status": "To Buy", "Quantity": 1, "Price": 10.00},
    {"Category": "Structure & Framing", "Item": "2020 Aluminum Extrusion Profile - 120 cm", "Status": "To Buy", "Quantity": 4, "Price": 4.50},
    {"Category": "Structure & Framing", "Item": "2020 Aluminum Extrusion Profile - 100 cm", "Status": "To Buy", "Quantity": 4, "Price": 3.50},
    {"Category": "Structure & Framing", "Item": "2020 Aluminum Extrusion Profile - 50 cm", "Status": "To Buy", "Quantity": 4, "Price": 2.00},
    {"Category": "Consumables", "Item": "3D Printer Filament (10 rolls PLA/PETG)", "Status": "To Buy", "Quantity": 10, "Price": 10.00},
    {"Category": "Already Owned", "Item": "iPad (Touchscreen / Dashboard)", "Status": "Owned", "Quantity": 1, "Price": 0.00},
    {"Category": "Already Owned", "Item": "ESP32 Microcontroller", "Status": "Owned", "Quantity": 1, "Price": 0.00},
    {"Category": "Already Owned", "Item": "LEGO Hub", "Status": "Owned", "Quantity": 1, "Price": 0.00},
    {"Category": "Already Owned", "Item": "LEGO Motors (C-channel & carousel)", "Status": "Owned", "Quantity": 4, "Price": 0.00},
    {"Category": "Already Owned", "Item": "OpenCV Camera (Low Resolution)", "Status": "Owned", "Quantity": 1, "Price": 0.00}
]

df_en = pd.DataFrame(data_english)
df_en["Total Price (USD)"] = df_en["Quantity"] * df_en["Price"]
print(f"Total to Buy: ${df_en[df_en['Status'] == 'To Buy']['Total Price (USD)'].sum():.2f}")

df_en.to_csv("lego_sorter_bom_complete_en.csv", index=False)
