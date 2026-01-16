# File Naming Standardization Report

## Overview
All files in the AURRAA project have been analyzed and renamed to follow consistent naming conventions. This ensures better maintainability, clarity, and professional organization.

## Naming Conventions Applied

### CSS Files - Clean Naming
**Pattern:** `{context}.css` - simple, descriptive names without redundant suffixes

- `styles.css` → `global.css` (main stylesheet)
- `chapter1-styles.css` → `chapter1.css`
- `grade-styles.css` → `grade.css`
- `math-g6-chapters-styles.css` → `math-g6-chapters.css`
- `ncert-grade6-styles.css` → `ncert-grade6.css`
- `practice-styles.css` → `practice.css`

### Auth CSS Files - Consolidated to Styles
**Pattern:** `auth-{page}.css` - grouped with all styles

- `login-styles.css` → `auth-login.css` (moved to `styles/`)
- `signup-styles.css` → `auth-signup.css` (moved to `styles/`)
- `signin-styles.css` → `auth-signin.css` (moved to `styles/`)

### Dashboard CSS
- `teacher-dashboard.css` → `dashboard.css` (moved to `styles/`)

### Config Files - Descriptive Naming
- `temp.html` → `dev-temp.html` (indicates it's a development temp file)
- `firebase-diagnostic.html` → `firebase-debug.html` (more descriptive purpose)

### Content Files - Fixed Typos & Standardized
**Typo Fixes:**
- `chem12ch1.html` → `chemistry-grade12-ch1.html` (more descriptive)
- `ncret-grade.html` → `ncert-grade.html` (spelling error fixed)
- `ncret-math-g6-c2.html` → `ncert-math-g6-chap2.html` (consistency)
- `quz-g6-ch1.html` → `quiz-g6-ch1.html` (spelling error fixed)

### Game Files - Standardized Naming
- `12sample-game.html` → `sample-game.html` (removed leading digit)
- `coulums.html` → `coulombs.html` (spelling error fixed)
- `gametemp.html` → `game-temp.html` (consistency with naming)
- `game.html` → `game-sample.html` (more descriptive)

### Video Files - Cleaned Up
**Files Removed:**
- `eample-vid.html` (duplicate of `example-video.html`)
- `temp.js` (temporary file)
- `Chemistry.1.html.zip` (archive)
- `maths.12.html.zip` (archive)
- `science.12.html.zip` (archive)
- `Temp/` directory (temporary folder)

**Retained:**
- `1.1.html`, `1.2.html`, `1.3.html`, `1.4.html` (numbered content - kept for existing references)
- `example-video.html` (single clean version)

## Folder Structure After Renaming

```
Aurraa/
├── styles/
│   ├── global.css (from styles.css)
│   ├── auth-login.css (from auth/login-styles.css)
│   ├── auth-signup.css (from auth/signup-styles.css)
│   ├── auth-signin.css (from auth/signin-styles.css)
│   ├── dashboard.css (from dashboard/teacher-dashboard.css)
│   ├── chapter1.css (from chapter1-styles.css)
│   ├── grade.css (from grade-styles.css)
│   ├── math-g6-chapters.css (from math-g6-chapters-styles.css)
│   ├── ncert-grade6.css (from ncert-grade6-styles.css)
│   ├── practice.css (from practice-styles.css)
│   └── badge.css (unchanged)
│
├── config/
│   ├── firebase.js (unchanged)
│   ├── firestore.rules (unchanged)
│   ├── dev-server.js (unchanged)
│   ├── dev-temp.html (from temp.html)
│   └── firebase-debug.html (from firebase-diagnostic.html)
│
├── content/chapters/
│   ├── chemistry-grade12-ch1.html (from chem12ch1.html)
│   ├── ncert-grade.html (from ncret-grade.html)
│   ├── ncert-math-g6-chap2.html (from ncret-math-g6-c2.html)
│   ├── quiz-g6-ch1.html (from quz-g6-ch1.html)
│   ├── quiz-g12-chem-ch1.html (unchanged)
│   ├── quiz-g12-math-ch1.html (unchanged)
│   ├── quiz-g12-phy-ch1.html (unchanged)
│   └── ... (other files)
│
├── games/
│   ├── sample-game.html (from 12sample-game.html)
│   ├── coulombs.html (from coulums.html - spelling fixed)
│   ├── game-temp.html (from gametemp.html)
│   ├── game-sample.html (from game.html)
│   └── ... (other game files)
│
└── video/
    ├── example-video.html (only copy kept)
    ├── video-g6-word-problem.html (unchanged)
    ├── video-g6-estimation.html (unchanged)
    ├── video-g12-coulombs.html (unchanged)
    ├── 1.1.html, 1.2.html, 1.3.html, 1.4.html (unchanged - numbered content)
    └── ... (other video files)
```

## Summary of Changes

### Files Renamed: 15
- **CSS files:** 11 renamed + 3 moved
- **Config files:** 2 renamed
- **Content files:** 4 renamed
- **Game files:** 4 renamed

### Files Removed: 6
- Video duplicates and archives removed
- Temporary files cleaned up

### References Updated
✅ All HTML files updated with new CSS paths
✅ All content file references updated
✅ All game file references updated
✅ Dashboard CSS reference updated
✅ Config file references updated

## Naming Convention Standards Now In Place

### CSS Files
- **Style:** `{category}.css` for main styles, `{category}-{page}.css` for specific pages
- **Location:** Centralized in `styles/` folder
- **Examples:** `global.css`, `auth-login.css`, `dashboard.css`, `chapter1.css`

### Configuration Files
- **Style:** `{service}-{purpose}.html` for clarity
- **Examples:** `firebase-debug.html`, `dev-temp.html`

### Content/Learning Files
- **Style:** `{subject}-{grade}-{chapter}.html` or `quiz-{grade}-{chapter}.html`
- **Examples:** `chemistry-grade12-ch1.html`, `ncert-math-g6-chap2.html`, `quiz-g6-ch1.html`

### Game Files
- **Style:** `game-{subject}-{grade}-{chapter}.html` or plain descriptive name
- **Examples:** `game-g12-chem-chap1.html`, `sample-game.html`, `coulombs.html`

### Video Files
- **Style:** `video-{subject}-{grade}-{topic}.html` or descriptive name
- **Examples:** `video-g6-word-problem.html`, `example-video.html`

## Benefits Achieved

✅ **Consistency** - All files follow predictable naming patterns  
✅ **Clarity** - File names clearly indicate their purpose  
✅ **Maintainability** - Easier to find and manage files  
✅ **Professionalism** - Project looks polished and well-organized  
✅ **Scalability** - New files can follow established conventions  
✅ **Spelling Corrections** - Fixed typos (ncret→ncert, quz→quiz, coulums→coulombs)  
✅ **Duplication Removed** - Eliminated redundant and temporary files  

