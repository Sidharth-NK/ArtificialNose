# ArtificialNose 🍵☕ 

A machine learning-based system to classify odors (coffee, tea, perfume, vinegar) using a **Multichannel Gas Sensor (GMXXX)** , **DHT22**and **Wio Terminal**. Designed for edge deployment with TinyML.

![Project Demo](demo.gif) *(Optional: Add a gif/video later)*

## 📌 Features
- **Real-time odor detection** using gas sensor arrays
- **Environment-aware classification** (works in both AC/non-AC spaces)
- **TinyML optimized** for deployment on Wio Terminal
- **4-class classifier** (Coffee, Tea, Perfume, Vinegar)

## 🛠 Hardware Requirements
| Component               | Specification                     |
|-------------------------|-----------------------------------|
| MCU                     | Wio Terminal (ATSAMD51)           |
| Gas Sensor              | Multichannel Gas Sensor V2 (GMXXX)|
| Temp/Humidity Sensor    | DHT22                             |
| Odor Samples            | Coffee grounds, Tea leaves, Perfume (alcohol-based), White vinegar |

## 📂 Dataset Structure
Collected data includes:
- **7 sensor features**:
  - `NO2`, `Ethanol`, `VOC`, `CO` (gas concentrations)
  - `Temperature`, `Humidity` (environmental)
  - `Location` (1=office/AC, 0=kitchen)
- **250+ samples per odor class**
