# 📅 Mini Calendar Using JavaScript

A sleek and minimalist **mini calendar application** that dynamically displays the current date, day, month, and year using JavaScript. This project is perfect for learning and showcasing real-time date manipulation and formatting.

---

## Features
- 📆 **Dynamic Date Display:** Automatically updates to display the current date, day, month, and year.
- 🎨 **Modern UI:** A visually appealing and responsive design with a gradient background and rounded calendar card.
- 💻 **Lightweight:** Built with pure HTML, CSS, and JavaScript for optimal performance.
- 🖥️ **Responsive:** Adapts seamlessly to all screen sizes for an excellent user experience.

---

## Technologies Used
- 🎨 **HTML:** Provides the structure for the calendar layout.
- 🎨 **CSS:** Styles the calendar, including the gradient background and rounded borders.
- ✨ **JavaScript:** Implements real-time date fetching and dynamic updates.

---

## How to Use

1. **View the Calendar:**
   - Open the `index.html` file in your browser to view the mini calendar.

2. **Real-Time Updates:**
   - The calendar dynamically displays the current:
     - **Date**
     - **Day**
     - **Month**
     - **Year**

3. **Responsive Design:**
   - Enjoy a seamless experience on any device, from desktop to mobile.

---

## How It Works

### Key JavaScript Logic:
- The `Date` object is used to fetch the current date and time.
- Arrays are utilized to map the day (`weekDays`) and month (`allMonths`) indices to their respective names.
- The `innerHTML` property updates the calendar elements dynamically.

```javascript
const date = document.getElementById("date");
const day = document.getElementById("day");
const month = document.getElementById("month");
const year = document.getElementById("year");

const today = new Date();

const weekDays = ["Sunday","Monday","Tuesday","Wednesday","Thursday","Friday","Saturday"];
const allMonths = ["January","February","March","April","May","June","July","August","September","October","November","December"];

date.innerHTML = (today.getDate()<10?"0":"") + today.getDate();
day.innerHTML = weekDays[today.getDay()];
month.innerHTML = allMonths[today.getMonth()];
year.innerHTML = today.getFullYear();
```

![Image](https://github.com/user-attachments/assets/9d1225c1-4c78-4382-8841-9c26858a4189)
