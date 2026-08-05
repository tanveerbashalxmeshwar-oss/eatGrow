<img width="1600" height="900" alt="WhatsApp Image 2026-08-05 at 4 22 18 PM" src="https://github.com/user-attachments/assets/c0ac7aac-f454-4344-88a6-1b105632e4f6" />
<img width="1600" height="900" alt="WhatsApp Image 2026-08-05 at 4 22 17 PM" src="https://github.com/user-attachments/assets/1892ea6e-9cf9-4dce-a9e6-3b717db66ce7" />




# 🌱 eatGrow — Fresh, Nutritious Food Near You

> **Eat well without guesswork.**

**eatGrow** is a responsive frontend web prototype that helps users discover fruits and vegetables based on their **city, area, budget, protein, and calorie preferences**.

The application ranks food items according to their **protein value per ₹100**, displays nutritional information, provides nearby shop directions through Google Maps, and allows users to compare two food items side by side.

---

## ✨ Features

### 🥗 Healthy Food Discovery

* Browse fruits and vegetables based on nutritional information.
* View:

  * Protein
  * Calories
  * Fiber
  * Price per kilogram
* Food items are displayed in an easy-to-understand card layout.

### 📍 Location-Based Selection

Users can select:

* City
* Area

Supported cities include:

* Mumbai
* Delhi
* Bangalore
* Hyderabad
* Chennai
* Pune

Each city contains multiple supported areas.

### 💰 Budget Filtering

Users can filter food according to their budget:

| Budget | Price Range          |
| ------ | -------------------- |
| Low    | Under ₹40/kg         |
| Medium | ₹40–₹90/kg           |
| High   | Over ₹90/kg          |
| Any    | No price restriction |

### 💪 Protein Filtering

Users can filter food based on protein content:

* Low
* Medium
* High
* Any

### 🔥 Calorie Filtering

Users can also filter foods based on calorie level:

* Low
* Medium
* High
* Any

### 📊 Smart Food Ranking

Food items are ranked according to:

**Protein per ₹100**

This allows users to quickly identify foods that provide better protein value for their money.

### 🏷️ Food Information Cards

Each food card displays:

* Food name
* Food type
* Emoji/icon
* Protein
* Calories
* Fiber
* Price
* Protein-per-₹100 score
* Suggested alternatives

### 🔄 Try Instead Suggestions

The application automatically recommends alternative food items with similar or better protein values.

### 📍 Shop Directions

Each food listing provides a generated Google Maps search link for the selected area and shop.

Users can click:

> **Get directions**

to open the location search in Google Maps.

### ⚖️ Food Comparison

Users can select up to **two food items** and compare them side by side.

The comparison includes:

* Price
* Protein
* Calories
* Fiber
* Value score
* Shop information

The better value for each comparison category is highlighted.

### 🧹 Clear Filters

Users can reset:

* City
* Area
* Budget
* Protein
* Calories

with a single **Clear Filters** button.

### 📱 Responsive Design

The interface adapts to different screen sizes using CSS media queries and responsive grid layouts.

### ♿ Accessibility Considerations

The project includes:

* Semantic HTML elements
* Keyboard focus styling
* Accessible modal close button
* Reduced-motion support using `prefers-reduced-motion`

---

## 🛠️ Technologies Used

### Frontend

* HTML5
* CSS3
* JavaScript
* CSS Grid
* CSS Flexbox
* Responsive Design

### External Resources

The project uses Google Fonts:

* Space Grotesk
* Inter
* IBM Plex Mono

### Maps

Google Maps search URLs are dynamically generated for shop directions.

---

## 📂 Project Structure

The project is intentionally simple and can run as a single HTML file.

```text
eatgrow/
│
└── eatgrow.html
```

The HTML file contains:

```text
HTML
├── Header
├── Hero Section
├── Food Search / Filter Form
├── Results Section
├── Food Cards
├── Comparison Bar
├── Comparison Modal
├── Toast Notifications
└── Footer

CSS
├── Color Variables
├── Header Styling
├── Hero Styling
├── Search Form
├── Food Cards
├── Comparison UI
├── Modal
├── Toast
└── Responsive Design

JavaScript
├── City & Area Data
├── Food Data
├── Price Calculation
├── Nutrition Filtering
├── Food Ranking
├── Alternative Recommendations
├── Google Maps Links
├── Food Comparison
├── UI Rendering
└── Toast Notifications
```

---

## 🍎 Available Food Data

The prototype contains sample data for various fruits and vegetables.

### Fruits

* Banana
* Apple
* Guava
* Papaya
* Pomegranate
* Orange
* Watermelon
* Mango
* Chikoo
* Grapes

### Vegetables

* Spinach
* Broccoli
* Moringa Leaves
* Green Peas
* Sweet Corn
* Moong Sprouts
* Bottle Gourd
* Okra
* Carrot
* Beetroot
* Cauliflower
* Cabbage
* Sweet Potato
* Potato
* Tomato
* Cucumber
* Capsicum
* Garlic

The project stores nutritional values such as protein, calories, fiber, and base price for these items.

---

## 🚀 How to Run

No backend or package installation is required.

### Step 1 — Download or Clone the Project

Place the project file in a folder:

```text
eatgrow/
└── eatgrow.html
```

### Step 2 — Open the HTML File

Simply double-click:

```text
eatgrow.html
```

or open it using a browser.

### Step 3 — Use the Application

1. Select a **City**
2. Select an **Area**
3. Choose a **Budget**
4. Choose a **Protein level**
5. Choose a **Calorie level**
6. Click **Find healthy food**
7. Browse the recommended foods
8. Open shop directions using Google Maps
9. Select two foods to compare them

---

## 🔍 How the Application Works

The basic workflow is:

```text
User
 │
 ▼
Select City
 │
 ▼
Select Area
 │
 ▼
Choose Filters
 │
 ├── Budget
 ├── Protein
 └── Calories
 │
 ▼
Generate Food Listings
 │
 ▼
Apply Filters
 │
 ▼
Calculate Protein-per-₹100 Score
 │
 ▼
Sort Food Items
 │
 ▼
Display Results
 │
 ├── Nutrition Information
 ├── Price
 ├── Shop
 ├── Alternatives
 └── Compare Option
```

---

## 🧠 Ranking Logic

eatGrow calculates a value score based on protein and price.

The project uses the concept:

```text
Protein Value Score =
Protein × 10 / Price × 100
```

The resulting value represents approximately:

```text
grams of protein per ₹100
```

Foods with higher scores are displayed first.

The actual implementation creates listings, calculates the score, applies filters, and sorts results from highest to lowest score.

---

## 💡 Example Usage

Suppose a user selects:

```text
City: Bangalore
Area: Indiranagar
Budget: Medium
Protein: High
Calories: Any
```

eatGrow will:

1. Generate food listings for Bangalore → Indiranagar.
2. Calculate prices using the prototype's city and location data.
3. Filter foods according to the selected criteria.
4. Calculate protein-per-₹100 value.
5. Sort the results.
6. Display suitable food cards.
7. Provide alternative food suggestions.
8. Provide shop directions.

---

## ⚖️ Comparison System

Users can select a maximum of two food items.

The comparison system evaluates:

```text
Price
Protein
Calories
Fiber
Value Score
Shop
```

For nutritional values, higher values are treated as better where appropriate, while lower price and calories are treated as better for comparison purposes.

---

## 📍 Google Maps Integration

The project generates a Google Maps search URL using:

```text
Shop + Area + City
```

This allows users to open a Google Maps search for the selected shop and location.

The project does **not** use a backend or Google Maps API key for this feature. It creates a regular Google Maps search URL in the browser.

---

## 🎨 UI / Design

The interface uses a fresh, nature-inspired design.

### Design Characteristics

* Forest green theme
* Citrus yellow accents
* Berry-colored links
* White content cards
* Rounded corners
* Soft shadows
* Responsive grid
* Nutrition-focused cards
* Tag/order-slip visual style

### Fonts

```text
Space Grotesk
Inter
IBM Plex Mono
```

The project imports these fonts from Google Fonts.

---

## 📱 Responsive Behavior

The application uses CSS responsive layouts.

For example:

```text
Desktop
┌────────┬────────┬────────┬────────┐
│ Food 1 │ Food 2 │ Food 3 │ Food 4 │
└────────┴────────┴────────┴────────┘

Mobile
┌──────────────┐
│    Food 1    │
├──────────────┤
│    Food 2    │
├──────────────┤
│    Food 3    │
└──────────────┘
```

The food cards automatically adapt using a responsive CSS grid.

---

## 🔐 Data & Privacy

This prototype operates entirely in the browser.

There is:

* No login system
* No database
* No backend server
* No user account system
* No API authentication
* No personal data storage

The food, city, area, shop, and nutrition information is stored directly in the JavaScript source.

---

## ⚠️ Important Disclaimer

**eatGrow is a prototype.**

The prices and stock information shown in the application are **illustrative sample data and are not live market listings**.

The application should not be considered a live food marketplace or a professional medical/nutritional recommendation system.

---

## 🔮 Future Improvements

The current prototype can be extended with:

* 🗺️ Real-time map integration
* 📍 GPS-based location detection
* 🏪 Real grocery/market listings
* 💰 Live food prices
* 🛒 Online grocery ordering
* 🥗 Personalized diet recommendations
* 👤 User accounts
* ❤️ Favorite foods
* 📈 Nutrition tracking
* 📊 Daily nutrition dashboard
* 🔔 Price alerts
* 🧠 AI-powered food recommendations
* 🌐 Backend API
* 🗄️ Database integration
* 📱 Progressive Web App support

---

## 🏗️ Possible Future Architecture

A production version could use:

```text
Frontend
│
├── HTML / CSS / JavaScript
│
▼
Backend API
│
├── Authentication
├── Food API
├── Nutrition Service
├── Location Service
└── Recommendation Engine
│
▼
Database
│
├── Users
├── Foods
├── Nutrition
├── Shops
├── Prices
└── User Preferences
```

---

## 📌 Current Project Scope

| Component               | Status |
| ----------------------- | ------ |
| Responsive UI           | ✅      |
| City Selection          | ✅      |
| Area Selection          | ✅      |
| Budget Filter           | ✅      |
| Protein Filter          | ✅      |
| Calorie Filter          | ✅      |
| Food Ranking            | ✅      |
| Nutrition Information   | ✅      |
| Alternative Suggestions | ✅      |
| Google Maps Search      | ✅      |
| Food Comparison         | ✅      |
| Backend                 | ❌      |
| Database                | ❌      |
| Live Prices             | ❌      |
| Real-Time Stock         | ❌      |
| User Authentication     | ❌      |

---

## 📄 License

This project is a prototype created for learning, demonstration, and project presentation purposes.

You can modify and extend the project according to your requirements.

---

## 👨‍💻 Project

**Project Name:** eatGrow
**Type:** Frontend Web Prototype
**Category:** Healthy Food Discovery & Nutrition
**Technology:** HTML, CSS & JavaScript

---

## 🌱 eatGrow

**Fresh produce. Better nutrition. Smarter choices.**
