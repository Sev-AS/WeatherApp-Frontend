# WeatherApp

**WeatherApp** is a modern web platform for meteorological data visualization, designed with a focus on high-end readability, minimalist typography, and a technical, efficient user interface.

The application implements a **modular component architecture** and a **design system based on a high-contrast color palette**.

---

# Technical Specifications

## Interface and User Experience

### Advanced Search System
Implementation of a **reactive modal** with support for:

- **Escape key (ESC)** closing
- **Click-outside-to-dismiss** functionality

### Data Normalization
Automatic processing of **text inputs to uppercase** to maintain visual consistency throughout the interface.

### Adaptive Layout
Responsive design that transitions:

- **Mobile:** vertical flow layout  
- **Large screens:** dual-column grid system (**L/H Screen**)

### Visual Optimization
- Use of **backdrop-blur filters**
- **Scale transitions** via CSS transforms  
- Focus on **fluid user interaction**

---

# Technology Stack

### HTML5 & JavaScript (ES6+)
- Direct **DOM manipulation**
- No heavy dependencies
- Optimized for **performance and low latency**

### Tailwind CSS
Custom configuration extending the project’s visual identity through **design tokens**:

- Colors
- Typography
- Spacing

### Typography

| Font | Usage |
|-----|------|
| **Space Grotesk** | Numerical data display and headers |
| **Inter** | Body text and general reading content |

---

# File Architecture

```
├── index.html 
├── src/
│ └── main.js 
├── js/
│ └── tailwind.config.js 
```
---

# Design System Configuration

The project utilizes a **custom color palette** defined within the Tailwind configuration file.

| Variable | Hexadecimal | Function |
|--------|-------------|---------|
| `primary` | `#000000` | Principal text and emphasis elements |
| `background` | `#FFFFFF` | General application background |
| `surface` | `#F5F5F5` | Card containers and secondary elements |
| `accent` | `#FF3300` | Active borders, indicators, and calls to action |
| `muted` | `#888888` | Low-hierarchy informational text |

---

# Usage Instructions

### Opening the Search
Click on the **current city name** or trigger the **search icon**.

### Modal Interaction
- Begin typing to search for a new location.
- The system automatically displays a **clear button** when text is detected in the input field.

### Closing the Interface
The modal can be dismissed via:

- The **[ESC] button**
- The **Escape key**
- Clicking the **overlay area outside the modal**

---

# Future Implementation

- **Real-time geolocation API integration**
- Connection with **dynamic meteorological data services (OpenWeather API)**
- **User preference persistence** via `LocalStorage`