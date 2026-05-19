# Currency Converter

A lightweight, responsive, and real-time Currency Converter web application built using Vanilla JavaScript, HTML5, and customized CSS3 layout modules.

## 🚀 Features

*   **Real-Time Rates**: Fetches live exchange rates using the decentralized, open-source Currency API.
*   **Global Support**: Supports over 100+ global fiat currencies mapped directly to their respective country codes.
*   **Dynamic Flag Updates**: Seamlessly updates national country flags on selection changes via the FlagsAPI integration.
*   **Input Sanitization**: Automatically handles empty or negative input fields, defaulting gracefully to a base value of 1.
*   **Custom Interface UI**: Designed with a soft green aesthetic featuring clean borders, fully customized dropdown fields, and clear text feedback.

## 🎨 Design & Styling Specifications

The styling in `style.css` leverages modern CSS layouts to build a smooth visual layout:
*   **Centering Engine**: Uses `flexbox` layout on the global `body` parameters to perfectly center the utility app card vertically and horizontally.
*   **Color Profile**: Utilizes a fresh natural palette with `#78bc61` for the main canvas backdrop and `#c0c781` for the central container panel.
*   **Component Structure**: Employs responsive border radii (`0.75rem`), normalized layout controls (`width: 100%`), and smooth inputs tailored with `aliceblue` background fills.

## 📦 Third-Party Integrations

This project fetches asset vectors and data blocks from these endpoints:
*   **Exchange Rates API**: `https://pages.dev`
*   **Flag Icons Engine**: `https://flagsapi.com`
*   **Icon Library**: FontAwesome v6.7.2 CDN Vector Icons

## 🛠️ Getting Started

Follow these steps to view this project on your local computer:

### 1. Clone the Repository
```bash
git clone https://github.com
cd Currency-Converter
```

### 2. Run the Application
Since this project consists of standard browser scripts, no installation steps (`npm install`) are required:
*   Simply open the `index.html` file directly in any modern web browser.
*   *Alternative*: Use the **Live Server** extension in Visual Studio Code for local hot-reloading features.

## 📁 Project Structure

```text
├── index.html      # Structural layout built with HTML5 semantic tags
├── style.css       # Custom stylesheet handling layouts, padding, and theme colors
├── codes.js        # Internal data matrix mapping ISO codes to country locations
└── app.js          # Main program engine managing asynchronous data fetching and DOM events
```

## 💻 Technical Implementation Highlights

*   **Asynchronous Fetch Workflow**: Uses the native JavaScript `async/await` syntax to securely fetch real-time JSON exchange objects over network calls.
*   **Dynamic Options Loading**: Iterates directly over data objects to inject options into the select elements programmatically without messy hardcoded markup.
