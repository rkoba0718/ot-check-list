[日本語](docs/README.ja.md)

# Overseas Travel Packing Checklist

A simple web app to manage your packing checklist for overseas travel.

## Application

https://rkoba0718.github.io/ot-check-list/

https://github.com/user-attachments/assets/2832888a-aa15-438e-8727-a686d7200e3c

Demonstrates the full workflow: adding items, checking off, editing, and marking as complete.

| Top Page | In Use |
|:---:|:---:|
| <img src="image/top.png" width="300"> | <img src="image/usage.png" width="300"> |

## Features

- **Add Items** - Add packing items via text input
- **Check Management** - Toggle prepared/unprepared status with checkboxes
- **Inline Editing** - Edit item names in place using the pencil icon
- **Delete** - Remove items with the × icon
- **Progress Display** - Visualize preparation status with a count and progress bar
- **Data Persistence** - Data is retained even after closing the browser via localStorage

## Usage

1. Access the [Checklist App](https://rkoba0718.github.io/ot-check-list/) (supports both PC and smartphones)
2. Enter an item name in the input field and press the "追加" (Add) button
3. Tap the checkbox to mark prepared items as complete
4. Use the pencil icon to edit or the × icon to delete items

## Tech Stack

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-222222?style=for-the-badge&logo=githubpages&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)

| Category | Technology |
|----------|------------|
| Frontend | HTML / CSS / Vanilla JavaScript |
| Data Storage | localStorage (browser-side storage) |
| Hosting | GitHub Pages |
| CI/CD | GitHub Actions |

## Project Structure

```
ot-check-list/
├── index.html                 # App (HTML/CSS/JS all-in-one)
├── image/
│   ├── intro.mp4              # Demo video
│   ├── top.png                # Top page screenshot
│   └── usage.png              # In-use screenshot
├── .github/workflows/
│   └── deploy.yml             # GitHub Pages deploy workflow
├── README.md                  # English README
└── README.ja.md               # Japanese README
```

## Run Locally

```bash
# Clone the repository
git clone https://github.com/rkoba0718/ot-check-list.git
cd ot-check-list

# Start a local server
python3 -m http.server 8080

# Open http://localhost:8080 in your browser
```

## Notes

- Data is stored in each device's browser (localStorage), so it cannot be shared across devices
- Clearing browser data will reset the checklist
