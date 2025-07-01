#  Suspicious Login Detection System

A simple Python-based tool that detects suspicious login attempts by analyzing IP address geolocation and timestamps. This project helps identify potentially compromised accounts by flagging impossible travel logins 鈥� such as accessing from two countries within a short time frame.

##  Features
- Detects abnormal login behavior based on time and location
- Flags logins from two different countries within 30 minutes
- Uses mock IP-to-country mapping (can be replaced with GeoIP APIs)
- Clean and beginner-friendly Python code

##  Project Structure
```
suspicious-login-detector/   suspicious_login_detector.py
sample_logs.csv
README.md
```

##  Sample Input (Python Dictionary)
```python
login_logs = [
    {"user": "Neves", "ip": "128.101.101.101", "time": "2025-07-01 10:00:00"},
    {"user": "Neves", "ip": "203.0.113.5", "time": "2025-07-01 10:15:00"},
]
```

##  Output
```
Suspicious logins detected:
- User: Neves, Location changed from USA to India within 15.0 minutes
  (2025-07-01 10:00:00  2025-07-01 10:15:00)
```

##  Technologies Used
- Python 3
- datetime module (standard library)

## Future Improvements
- Integrate real-time IP geolocation APIs
- Email/SMS alert integration
- Flask-based dashboard

##  Author
**Prasanth K**  Cybersecurity Enthusiast

##  License
Free to use for learning and personal use.
