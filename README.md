# CCTV-monitoring-software
Sure! Here's a detailed **README.md** for your **SecureSight CCTV Monitoring Dashboard** project, based on the frontend and backend scope you described.

# 📹 SecureSight — CCTV Monitoring Dashboard

SecureSight is a fictional CCTV surveillance dashboard that allows monitoring up to **3 live camera feeds** with real-time incident detection powered by computer vision (e.g. gun threats, unauthorized access). This project represents a frontend prototype integrated with a basic backend API to simulate incident data and camera feeds.

## 🔧 Features

### ✅ Mandatory Scope:
- **Navbar:** Navigation bar with branding and user controls
- **Incident Player:** Video player to view live or recorded incident footage
- **Incident List:** Scrollable list of ongoing or past incidents

### 💡 Optional (Implemented):
- **Incident Timeline:** Scrollable timeline to view when incidents occurred
- **3D Dashboard Hover Effect:** Simulates a subtle 3D transform effect for immersive UI
- **Critical Alerts Animation:** Flashing pulse around high-severity incident cards
- **Live Simulated Data (Frontend Only):** New incidents appear every 15 seconds

## 📁 Project Structure

```
securisight-dashboard/
├── index.html       # Main HTML layout
```

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/securisight-dashboard.git
cd securisight-dashboard
```

### 2. Open the App (No Installation Required)

This is a **static frontend project**. Simply open `index.html` in your browser:

```bash
open index.html    # macOS
xdg-open index.html # Linux
start index.html    # Windows
```

> ✅ Tailwind and FontAwesome are loaded via CDN.
>   
> 📽️ Videos play from simulated video tags (add your own files to `assets/`).

## ⚙ Backend (Mock API)

You can simulate basic API functionality using [JSON Server](https://github.com/typicode/json-server) or create a lightweight Express/FastAPI server.

**Example static data model:**

```json
GET /api/incidents
[
  {
    "id": "inc-123",
    "cameraId": "cam-01",
    "type": "Unauthorized Access",
    "thumbnailUrl": "/assets/thumb1.jpg",
    "tsStart": "2025-07-21T08:00:00Z",
    "tsEnd": "2025-07-21T08:02:00Z",
    "resolved": false
  }
]
```

## 🧪 Optional Enhancements

| Feature              | Status | Stack/Details                        |
|----------------------|--------|-------------------------------------|
| Incident Timeline    | ✅     | Horizontal scroll w/ markers       |
| 3D Transform Effect  | ✅     | CSS3 on content hover               |
| Critical Alerts      | ✅     | Pulse animation using `@keyframes` |
| Filter/Sort UI       | ⬜     | Not implemented                    |
| Backend Integration  | ⬜     | Replace simulated data with real   |

## 🎨 Tech Stack

| Category    | Tech                                                     |
|-------------|----------------------------------------------------------|
| HTML/CSS    | HTML5, CSS3, [Tailwind CSS](https://tailwindcss.com)     |
| JavaScript  | Vanilla JS, DOM manipulation                            |
| Video Embed | HTML5 `` player                                   |
| Icons       | [Font Awesome](https://fontawesome.com/) via CDN         |
| Timeline    | Custom CSS & dynamic renders                             |

## 🛠 Screenshots

![Dashboard Overview](assets/screenshot Future Improvements

- Integrate with real backend to fetch incident streams
- WebSocket/live feed updates
- Enable camera feed switching
- Full-screen video support
- Include object detection visualizations (e.g. bounding boxes)

## ✍️ Author

Developed with ❤️ for SecureSight's Technical Assessment  
[Your Name -  GitHub](https://github.com/your-username)

## 📄 License

This project is open source and free to fork. License: MIT

Let me know if you'd like a version with placeholder Markdown image previews or links to actual video demos!
