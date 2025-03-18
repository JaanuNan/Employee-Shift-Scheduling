# Shift Scheduling Application

This project is a **Shift Scheduling Application** designed to simplify the process of creating, optimizing, and managing work schedules for a team. The application uses a combination of front-end technologies (HTML, JavaScript, FullCalendar) and back-end logic (Python with DEAP for optimization) to generate efficient and fair work schedules.

---

## Features 

- **Add Team Members**: Dynamically add or remove team members from the scheduling pool.
- **Generate Optimized Schedules**: Automatically create schedules that adhere to predefined rules using optimization algorithms.
- **Interactive Calendar**: View, load, and save schedules using an interactive calendar interface powered by FullCalendar.
- **Shift Types**:
  - **Day Shift**: Monday to Thursday (9:00 AM - 6:00 PM), Friday (9:00 AM - 4:00 PM).
  - **Night Shift**: Monday to Thursday (6:01 PM - 8:59 AM next day).
  - **Weekend Shift**: Friday (4:00 PM) to Monday (9:00 AM).
- **Metrics Dashboard**:
  - View annual and monthly shift distribution for each employee.
- **Save and Load Schedules**: Persist schedules for future use.

---

## Table of Contents

1. [Technologies Used](#technologies-used)
2. [Setup Instructions](#setup-instructions)
3. [Usage Guide](#usage-guide)
4. [Optimization Rules](#optimization-rules)
5. [Screenshots](#screenshots)

---

## Technologies Used 

### Front-End
- HTML5
- CSS3 (Bootstrap for styling)
- JavaScript:
  - FullCalendar.js
  - jQuery
  - Plotly.js for data visualization

### Back-End
- Python:
  - DEAP library for genetic algorithm-based optimization
  - Flask (or similar framework) for handling API requests
- Other Libraries:
  - Calendar module for date calculations

---

## Setup Instructions 

### Prerequisites
1. Install Python (>=3.7).
2. Install required Python libraries:
   ```bash
   pip install flask deap
   ```
3. Ensure you have internet access for external libraries like Bootstrap, FullCalendar, and Plotly.

### Steps to Run the Project
1. Clone the repository:
   ```bash
   git repo clone JaanuNan/Employee-Shift-Scheduling
   cd shift-scheduling
   ```
2. Start the back-end server:
   ```bash
   python app.py
   ```
3. Open `index.html` in your browser to access the front-end interface.

---

## Usage Guide 

1. **Add Team Members**:
   - Enter team member names in the input fields provided.
   - Use the "Add Name" button to add more fields or "X" buttons to remove names.

2. **Generate Schedule**:
   - Click on "Create Calendar" to generate an optimized schedule.
   - The schedule will appear on the interactive calendar.

3. **Save or Load Schedules**:
   - Save generated schedules using the "Save Calendar" button.
   - Load previously saved schedules by selecting from the dropdown and clicking "Load Schedule."

4. **View Metrics**:
   - Scroll down to view annual and monthly shift distribution metrics.

---

## Optimization Rules 

The scheduling algorithm ensures compliance with the following rules:

1. A worker cannot work two shifts in the same week.
2. The day worker of the current week must be the night worker of the next week.
3. The night worker of the current week cannot work in the next week.

The algorithm uses a genetic approach to find an optimal solution that satisfies these constraints while distributing shifts fairly among all workers.

---

## Screenshots 

![image](https://github.com/user-attachments/assets/e3b366f4-c284-4a29-bc63-741babcb316f)
![image](https://github.com/user-attachments/assets/86aeca7b-4aee-4412-9577-81e6f341b603)
![image](https://github.com/user-attachments/assets/1b3f94b7-694f-47f4-bac4-864ae19c9730)






---





