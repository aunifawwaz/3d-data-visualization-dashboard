# 3D Data Visualization Dashboard

An interactive 3D data visualization web application built with **Three.js** and **JavaScript**. This project displays 200+ user profiles parsed from an external dataset, rendered as interactive CSS3D objects that can transition between four distinct spatial layouts.

### 🚀 Live Demo
https://3dvisualisationaunifawwaz.netlify.app/

### ✨ Key Features & Technical Implementations

* **Google Authentication (OAuth 2.0):** Integrated Google Identity Services (GIS) to create a secure, full-screen login portal. The 3D scene remains locked until the user successfully authenticates.
* **External Data Fetching:** Utilized `PapaParse` to asynchronously fetch and parse CSV data directly from a published Google Sheet API endpoint.
* **Dynamic Conditional Styling:** Programmed logic to parse financial data strings (Net Worth) and dynamically assign background colors to the 3D cards based on specific thresholds (Red < $100k, Orange $100k-$200k, Green > $200k).
* **Custom Layout Algorithms:** Re-engineered the default Three.js periodic table math to create four completely different layouts for over 200 data points:
  1. **Table:** A flat 20x10 grid.
  2. **Sphere:** A Fibonacci sphere distribution.
  3. **Double Helix:** Custom trigonometry to create a two-strand DNA-style spiral.
  4. **3D Grid:** A volumetric 5x4x10 grid.
* **Smooth Animations:** Used `TWEEN.js` to interpolate camera and object positions, allowing data cards to fluidly morph between layouts.
* **Deployment:** Hosted and deployed via Netlify.

### 🛠️ Tech Stack
* **Frontend:** HTML5, CSS3, Vanilla JavaScript
* **3D Engine:** Three.js (CSS3DRenderer)
* **Authentication:** Google Identity Services (GIS)
* **Data Parsing:** PapaParse
* **Animation:** TWEEN.js

### ⚙️ How to Run Locally
1. Clone this repository.
2. Open the `index.html` file in your code editor and replace the `data-client_id` in the Google login div with your own Google Cloud OAuth Client ID.
3. Run the project using a local server (like VS Code's **Live Server** extension).

*Note: The base 3D rendering architecture was inspired by the official Three.js CSS3D Periodic Table demo. The data integration, OAuth, layout mathematics, and UI styling were custom-built for this project.*