# AR Marker Detector 🟦

A lightweight, production-ready WebXR application that detects a custom physical marker and renders a 3D overlay in real-time. Built with **AR.js** and **A-Frame**, this project runs entirely in the browser without any backend server requirements.

## 🚀 Features

- **Instant AR Detection:** Recognizes the custom `pattern-nielit.patt` marker.
- **Production UX:**
  - **Loading Screen:** Elegant spinner while the camera initializes.
  - **Status Badge:** Real-time feedback ("Searching..." vs "Marker Detected!").
  - **Error Handling:** Friendly messages if camera access is denied.
- **Visuals:** Renders a high-fidelity **Blue 3D Box** with smooth rotation animation.
- **Mobile Optimized:** Full-screen experience with VR mode disabled (no goggles button).

## 🛠️ Tech Stack

- **Frontend:** HTML5, CSS3
- **AR Engine:** [AR.js](https://github.com/AR-js-org/AR.js) (Marker Tracking)
- **3D Engine:** [A-Frame](https://aframe.io/) (Rendering)

## 📂 Project Structure

```text
📦 avr_custom_marker
 ┣ 📜 index.html           # Main AR application
 ┣ 📜 pattern-nielit.patt  # The custom marker file (Binary pattern)
 ┗ 📜 README.md            # Documentation

```

## ⚙️ Setup & Deployment

**Note:** This application requires **HTTPS** to access the device camera. It will not work on `http://` or if you simply open the file on your desktop.

### 1. Prerequisites

* A GitHub account.
* The `pattern-nielit.patt` file (included in this repo).
* A printer (to print the physical marker).

### 2. Deployment (GitHub Pages)

1. Upload `index.html` and `pattern-nielit.patt` to your GitHub repository.
2. Go to **Settings** > **Pages**.
3. Under **Branch**, select `main` (or `master`) and `/root`.
4. Click **Save**.
5. Wait ~2 minutes for the site to go live at `https://yourusername.github.io/repo-name`.

## 📱 How to Use

1. **Print the Marker:** Ensure you have the NIELIT pattern printed (black square with custom inner design).
* *Tip: Ensure there is a white border around the black square.*


2. **Open the App:** Visit your GitHub Pages URL on a smartphone.
3. **Grant Permissions:** Allow camera access when prompted.
4. **Scan:** Point your camera at the paper marker.
* **Success:** The status badge turns **Green**, and a floating Blue Box appears over the paper!



## 🐛 Troubleshooting

| Issue | Cause | Fix |
| --- | --- | --- |
| **Camera won't open** | Insecure Context | Ensure URL starts with `https://`. |
| **Stuck on Loading** | Camera Permission | Check browser settings to allow camera access. |
| **Marker not detected** | Bad Lighting | Move to a brighter area. Avoid glare on the paper. |
| **Box is flickering** | Stability | Keep the camera steady; the app uses smoothing to help. |
| **404 Not Found** | Missing File | Ensure `pattern-nielit.patt` is in the exact same folder as `index.html`. |

## 📄 License

This project is licensed under the MIT License.

---

*Built with ❤️ using WebXR*
