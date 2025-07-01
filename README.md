# 馃攼 Suspicious Login Detection System

A simple Python-based tool that detects suspicious login attempts by analyzing IP address geolocation and timestamps. This project helps identify potentially compromised accounts by flagging impossible travel logins 鈥� such as accessing from two countries within a short time frame.

## 馃殌 Features
- Detects abnormal login behavior based on time and location
- Flags logins from two different countries within 30 minutes
- Uses mock IP-to-country mapping (can be replaced with GeoIP APIs)
- Clean and beginner-friendly Python code

## 馃搧 Project Structure
```
suspicious-login-detector/
鈹溾攢鈹€ suspicious_login_detector.py
鈹溾攢鈹€ sample_logs.csv
鈹溾攢鈹€ README.md
```

## 馃И Sample Input (Python Dictionary)
```python
login_logs = [
    {"user": "alice", "ip": "128.101.101.101", "time": "2025-07-01 10:00:00"},
    {"user": "alice", "ip": "203.0.113.5", "time": "2025-07-01 10:15:00"},
]
```

## 鉁� Output
```
Suspicious logins detected:
- User: alice, Location changed from USA to India within 15.0 minutes
  (2025-07-01 10:00:00 鈫� 2025-07-01 10:15:00)
```

## 馃洜锔� Technologies Used
- Python 3
- datetime module (standard library)

## 馃挕 Future Improvements
- Integrate real-time IP geolocation APIs
- Email/SMS alert integration
- Flask-based dashboard

## 馃懆鈥嶐煉� Author
**Prasanth K** 鈥� Cybersecurity Enthusiast

## 馃摐 License
Free to use for learning and personal use.
