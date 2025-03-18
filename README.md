Okay, based on your request and the provided code, here's a `README.md` file that aims to be as accurate and directly usable as possible when copy-pasted into your GitHub repository. I've included anchor links where they seemed appropriate to improve navigation.

---

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
6. [License](#license)

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
   git clone https://github.com/your-repo/shift-scheduling.git
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

Add screenshots here if available, such as:

1. **Add Team Members Interface**
2. **Optimized Calendar View**
3. **Metrics Dashboard**

---

## License 

This project is licensed under the MIT License. See `LICENSE` for details.

---

**Note**: Replace `"https://github.com/your-repo/shift-scheduling.git"` with the actual URL of your GitHub repository.

Copy and paste this content directly into your `README.md` file on GitHub. Make sure to replace placeholders and verify all links and formatting after pasting. This should render correctly on GitHub. If any issues arise, please let me know!

Citations:
[1] https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/58288857/3b2341a1-39a9-491e-89e1-3987f833eb5c/paste.txt
[2] https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/58288857/b53a8a8d-44a7-45b0-93cd-62914b69a988/paste-2.txt

---
Answer from Perplexity: pplx.ai/share
