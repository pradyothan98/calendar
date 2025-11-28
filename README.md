# Executive Smart Calendar 🗓️

A Python desktop app that gives business executives a **smart, visual calendar** with:
- A month-view calendar
- Daily task list with **priority, status, owner, and notes**
- Automatic export to **Excel** (`executive_tasks.xlsx`)
- Simple, GUI-based workflow (no need to touch the code once it's running)

---

## 🚀 Features

- **Calendar GUI (Tkinter)**
  - Month view with clickable dates
  - Highlights:
    - **Today** (green)
    - **Selected date** (blue)
    - **Dates with tasks** (yellow)

- **Task management**
  - Add / edit / delete / view tasks for any day
  - Each task includes:
    - Title
    - Start time & end time (`HH:MM`, 24-hour, optional)
    - Priority: `Low`, `Medium`, `High`, `Critical`
    - Status: `Planned`, `In Progress`, `Done`, `Blocked`
    - Owner (responsible person)
    - Notes

- **Executive KPIs**
  - Tasks **today**
  - Tasks in the **next 7 days**
  - Number of **overdue** tasks (past days that are not marked "Done")

- **Excel integration**
  - All tasks exported automatically to **`executive_tasks.xlsx`**
  - Each row = one task, with columns:
    - Date, Title, Start, End, Priority, Status, Owner, Notes  
  - If `executive_tasks.xlsx` is manually deleted, the app **cannot recover it**.  
    It will create a **fresh file** from current tasks the next time you modify tasks.

---

## 🛠️ Tech stack

- **Language:** Python 3.9+  
- **GUI:** Tkinter (built into Python)
- **Excel:** [openpyxl](https://pypi.org/project/openpyxl/)

---

## 📦 Installation

### 1. Clone the repo

```bash
git clone https://github.com/<your-username>/executive-smart-calendar.git
cd executive-smart-calendar
