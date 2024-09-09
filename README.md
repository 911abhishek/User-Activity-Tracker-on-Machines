
# User Activity Tracker on Machines

## Overview
This script is designed to track login and logout events of users on different machines and generate a report showing which users are currently logged into which machines.

The script processes a series of events and outputs the current status of users logged into specific machines.

## Features
- Track user login and logout events.
- Generate a report of current users logged into each machine.
- Class-based event structure for easy extension.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/user-activity-tracker.git
   ```

2. Navigate to the project directory:
   ```bash
   cd user-activity-tracker
   ```

3. Run the script:
   ```bash
   python script.py
   ```

## Usage
You can add or modify the `events` list in the script to simulate different login/logout events.

### Example Event List:
```python
events = [
    Event('2020-01-21 12:45:46', 'login', 'myworkstation.local', 'jordan'),
    Event('2020-01-22 15:53:42', 'logout', 'webserver.local', 'jordan'),
    Event('2020-01-21 18:53:21', 'login', 'webserver.local', 'lane'),
    Event('2020-01-22 10:25:34', 'logout', 'myworkstation.local', 'jordan'),
    Event('2020-01-21 08:20:01', 'login', 'webserver.local', 'jordan'),
    Event('2020-01-23 11:24:35', 'login', 'mailserver.local', 'chris'),
]
```

## How It Works
1. **get_event_date(event)**: Used to sort events by date.
2. **current_users(events)**: Loops through the events and keeps track of users logged into each machine.
3. **generate_report(machines)**: Generates and prints a report of the current users on each machine.

## Contributing
Feel free to submit pull requests or report any issues.

## License
This project is licensed under the MIT License.
