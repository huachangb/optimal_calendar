# Planner for finding the optimal schedule
To-do:
- Make a to-do list

## Format of dates 
```json
[
    {
        "description": str,
        "start_date": datetime,
        "duration": int,
        "location": str
    }
]
```

# Usage
```python
from calendar_planner import Calendar

# dictionary of subjects and path to file
course_paths = {
    "path-to-excel-file": "course-name"
}

# create calendar
cal = Calendar()
cal.add_courses_from_excel(course_paths)

# get all possible combinations
cal.find_all_schedules()
```
