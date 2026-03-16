# IOE Internal Marks Predictor

A web tool for IOE (Institute of Engineering, Tribhuvan University) students to predict internal assessment marks and reverse-calculate teacher-given marks from published grade sheets.

## Live

**[ioe.bibeksubedi0001.com.np](https://ioe.bibeksubedi0001.com.np)**

## Features

- **Predict Mode** — Enter marks given by your teacher (Asst.) and your external score (Final) to see the predicted marksheet internal marks and grade.
- **Reverse Mode** — Enter your actual marksheet Asst. & Final marks to find out what your teacher originally gave you.
- GPA calculation with overall grade
- Print-friendly marksheet layout
- Supports multiple faculties: BCE, BCT, BEI, BME, BAR, BAM, BIE
- Semester selection (I/I through III/I)

## How It Works

IOE applies an internal moderation rule:

| Condition                   | Effect                                |
| --------------------------- | ------------------------------------- |
| External ≥ 80%              | No change to internal marks           |
| Internal–External gap > 20% | Reduction = (gap − 20) × 2            |
| External > pass mark        | Internal guaranteed ≥ 40% of Asst. FM |

This tool applies those rules to predict or reverse-engineer the marks.

## Project Structure

```
├── index.html       # Entry point (auto-redirects to app)
├── app.html         # Main application
├── assets/
│   └── logo.svg     # TU logo
├── data/
│   ├── subject-data.js   # Subject data (JS bundle)
│   └── subject.json      # Raw subject data source
├── CNAME            # Custom domain for GitHub Pages
└── README.md
```

## Setup

No build step required — just open `internal-marks-predictor.html` in a browser, or visit the live site.

## Author

**Bibek Subedi** — [bibeksubedi0001.com.np](https://bibeksubedi0001.com.np)
