# DesiRig: Assembler 🖥️ 🇮🇳

**DesiRig: Assembler** is a premium, client-side web application designed for the Indian PC gaming community. It allows users to visually build custom PCs, check compatibility, estimate power consumption, and get price estimates in Indian Rupees (₹).

🔗 **Live Demo:** [https://adityasync.github.io/DesiRig/](https://adityasync.github.io/DesiRig/)

---

## 📑 Table of Contents
- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [APIs & Data Sources](#-apis--data-sources)
- [Getting Started](#-getting-started)
- [Contributing](#-contributing)
- [License](#-license)
- [Credits](#-credits--author)

---

## ✨ Features

* **Interactive Visualizer:** A dynamic SVG-based PC case visualizer that updates in real-time as you add components (motherboard, GPU, fans, cables).
* **Smart Compatibility Engine:** Automatically filters parts based on compatibility logic (e.g., matching CPU socket types, RAM generations).
* **Indian Market Pricing:** Integrated curated database of popular components with pricing in INR (₹).
* **Wattage Calculator:** Real-time TDP calculation to assist in selecting the appropriate Power Supply Unit (PSU).
* **Responsive Hybrid Design:**
    * *Desktop:* Fixed, app-like "cockpit" interface.
    * *Mobile:* Vertical scroll layout optimized for touch.
* **PDF Build Sheet:** One-click generation of a branded, printable invoice/build summary.
* **Direct Purchase Links:** Integrated "Buy" buttons that redirect to Amazon India search results for specific parts.

---

## 🛠️ Tech Stack

This project is architected as a **Single File Application (SFA)** for maximum portability and ease of demonstration.

| Component | Technology |
| :--- | :--- |
| **Core Framework** | React.js (v18, via CDN) |
| **Styling** | Tailwind CSS (via CDN) |
| **Transpiler** | Babel (Standalone) |
| **Icons** | Custom Inline SVGs (Lucide-style) |
| **Typography** | Space Grotesk |

---

## 🔌 APIs & Data Sources

### Note on Data Architecture
To ensure this application runs entirely client-side without complex backend dependencies or CORS issues during the preview phase, the component database is simulated internally.

* **Internal Database (`INITIAL_DB`):** The app uses a structured JSON object containing curated data for CPUs, GPUs, Motherboards, RAM, Storage, PSUs, and Cases. This data represents estimated market pricing in India as of Dec 2024/Jan 2025.
* **Simulated Async Operations:** The "Sync Stock" feature simulates a live network fetch request (`setTimeout`) to update prices and availability, providing a realistic "loading" state and UI feedback.
* **External Integrations (Amazon India):** The application dynamically generates search URLs (`https://www.amazon.in/s?k=...`) based on the selected product names to facilitate purchase.

---

## 🚀 Getting Started

You can run this project locally without any Node.js environment or build steps.

### Prerequisites
* A modern web browser (Chrome, Edge, Firefox, Safari).
* An active internet connection (to load React & Tailwind from CDNs).

### Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/adityasync/DesiRig.git
    ```

2.  **Navigate to the project folder:**
    ```bash
    cd DesiRig
    ```

3.  **Run the App:**
    Simply open the `index.html` file in your browser.

---

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1.  Fork the project
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the Branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request

---

## 📄 License

Distributed under the **MIT License**. See `LICENSE` for more information.

---

## ❤️ Credits & Author

This project was conceptually designed, developed, and maintained by **Aditya**.

<div align="center">
  <br />
  <h3>Aditya</h3>
  <p>Made with ♥ in India</p>
</div>
