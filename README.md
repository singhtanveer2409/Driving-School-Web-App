# 🚗 Driving School Web App

![License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square)
![Status](https://img.shields.io/badge/status-development-orange.svg?style=flat-square)
![Platform](https://img.shields.io/badge/platform-web-lightgrey.svg?style=flat-square)

A modern, responsive web application designed to streamline the management of driving school operations. Built on top of the robust **AdminLTE 3** framework, this application offers an intuitive dashboard for administrators to manage schedules, students, and instructors efficiently.

---

## ✨ Features

*   **📱 Fully Responsive**: Optimized for desktops, tablets, and mobile devices using Bootstrap 4.
*   **📊 Interactive Dashboard**: Visual insights into school performance and statistics.
*   **📅 Schedule Management**: Integrated **FullCalendar** for managing driving lessons and exams.
*   **🔒 Security**: Includes custom lock screens and secure authentication layouts.
*   **🎨 Modern UI/UX**: Clean aesthetic with dark mode support and customizable themes.
*   **⚠️ Error Handling**: Custom designed 404 and 500 error pages.
*   **🧩 Modular Components**: Utilizes jQuery UI and various plugins for enhanced functionality.

## 🛠️ Tech Stack

The project is built on a classic, robust stack centered around **AdminLTE 3**.

### Core Technologies

| Component | Technology | Role & Implementation |
| :--- | :--- | :--- |
| **UI Framework** | **[AdminLTE 3](https://adminlte.io/)** (Bootstrap 4) | Provides the skeleton (Sidebar, Header, Footer) and responsive grid. Ensures mobile/desktop compatibility. |
| **Styling** | **[SASS/SCSS](https://sass-lang.com/)** | Used for modular CSS, utilizing variables and mixins for a maintainable codebase. |
| **Scripting** | **[jQuery](https://jquery.com/)** | Primary engine for DOM manipulation and UI component initialization. |
| **Scheduling** | **FullCalendar** | Renders interactive lesson/exam schedules. |
| **Visualization** | **Raphael** | Vector graphics library for dashboard charts. |
| **Interactivity** | **jQuery UI** & **Mousewheel** | Provides advanced interactions like drag-and-drop and custom scrolling. |

### Implementation Strategy

The project follows a **compile-to-dist** workflow where source code in `build/` is compiled into browser-ready assets in `dist/`.

#### 1. Modular SCSS Architecture
Styles are written in SCSS using a modular import system. The manifest file (`_adminlte.raw.scss`) acts as the central hub, importing variables, mixins, core styles, and components in a specific order. This allows for global theming via variable overrides.

#### 2. Component Isolation
Specific pages (like the Lockscreen) have isolated styles to prevent CSS leakage. The application supports **Dark Mode** by toggling a `.dark-mode` class on the `<body>`, which triggers specific overrides in component files.

#### 3. Print Optimization
The application is optimized for physical office workflows. The `_print.scss` file defines utility classes like `.no-print` to hide navigation bars during printing, ensuring invoices and schedules are formatted correctly for paper.

## 🚀 Getting Started

Follow these instructions to get a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

*   A modern web browser.
*   A local web server (e.g., Live Server, Apache, Nginx) or Node.js environment if building assets.

### Installation

1.  **Clone the repository**
    ```bash
    git clone https://github.com/your-username/Driving-School-Web-App.git
    ```

2.  **Navigate to the project directory**
    ```bash
    cd Driving-School-Web-App
    ```

3.  **Install Dependencies** (If using npm/yarn for build tools)
    ```bash
    npm install
    ```

4.  **Run the Application**
    Open `index.html` in your browser or serve via a local server.

## 📂 Project Structure

```text
Driving-School-Web-App/
├── build/          # Development folder: SCSS source files and build scripts
├── dist/           # Production folder: Compiled CSS and JS files ready for the browser
├── pages/          # HTML templates for specific views (Lockscreen, Errors, etc.)
├── plugins/        # Self-contained repository of third-party dependencies
└── README.md       # Project documentation
```

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/NewFeature`)
3.  Commit your Changes (`git commit -m 'Add some NewFeature'`)
4.  Push to the Branch (`git push origin feature/NewFeature`)
5.  Open a Pull Request

## 📄 License

This project is open source and available under the MIT License.

---
*Made with ❤️ for better driving education.*