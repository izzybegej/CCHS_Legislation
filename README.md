# 🐾 Illinois Animal Welfare Bill Tracker

A Python web scraper that monitors Illinois General Assembly bills relevant to
animal welfare, extracts key legislative data, and presents it in a dashboard.

## Desired Outcomes

Watches a list of Illinois House and Senate bills and pulls:
- Bill sponsor and their district
- Assigned committee + committee homepage link
- Current status
- Upcoming scheduled hearings or actions
- Link to full bill text

Initially targeting for organizations in the **52nd Senate / 103rd House districts**.

## Tech Stack

| Tool | Purpose |
|------|---------|
| `requests` | Fetches raw HTML/XML from websites |
| `BeautifulSoup4` | Parses and navigates HTML/XML |
| `pandas` | Stores and manipulates bill data |
| `Streamlit` | Web-based UI dashboard |

## Project Status

🚧 **Phase 1 — In Progress**: XML discovery and site structure research

## Getting Started

### Prerequisites
- Python 3.8+
- pip

### Installation
```bash
git clone https://github.com/YOUR_USERNAME/il-bill-tracker.git
cd il-bill-tracker
pip install -r requirements.txt
python src/scraper.py
```

## Project Structure
```
il-bill-tracker/
├── src/
│   ├── scraper.py       # Fetches and parses bill data
│   ├── bills.py         # Bill list and data management
│   └── app.py           # Streamlit dashboard
├── data/
│   └── bills.csv        # Auto-generated cache
├── tests/
├── requirements.txt
├── README.md
├── PROJECT_PLAN.md
└── CHANGELOG.md
```

## Districts Reference

| Chamber | District | Rep |
|---------|----------|-----|
| Senate  | 52nd     | Paul Faraci (Ours) |
| House   | 103rd    | Carol Ammons (Ours) |
| Senate  | 51st     | Chapin Rose (Neighbor) |
