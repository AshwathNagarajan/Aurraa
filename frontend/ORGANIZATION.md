# AURRAA Project - Folder Organization

## Overview
The AURRAA project has been reorganized by feature to improve maintainability and clarity. All files are now organized into logical feature-based directories.

## Directory Structure

```
Aurraa/
├── index.html                  # Main landing page
├── auth/                       # Authentication & Login/Signup
│   ├── login.html
│   ├── login.js
│   ├── login-handler.js
│   ├── login-styles.css
│   ├── signup.html
│   ├── signup-styles.css
│   ├── teacher-login.html
│   ├── teacher-signup.html
│   ├── teacher-auth.js
│   ├── teacher-login-handler.js
│   ├── student-auth.js
│   ├── signin.html
│   ├── signin-styles.css
│   └── enhanced-login.js
├── dashboard/                  # Teacher Dashboard
│   ├── teacher-dashboard.html
│   └── app.js
├── styles/                     # All CSS stylesheets
│   ├── badge.css
│   ├── teacher-dashboard.css
│   ├── chapter1-styles.css
│   ├── grade-styles.css
│   ├── math-g6-chapters-styles.css
│   ├── ncert-grade6-styles.css
│   └── practice-styles.css
├── utils/                      # Utility functions
│   └── badge.js                # Badge/reward system
├── config/                     # Configuration & Setup
│   ├── firebase.js
│   ├── firestore.rules
│   ├── dev-server.js
│   ├── firebase-diagnostic.html
│   └── temp.html
├── content/                    # Learning Content
│   ├── syllabus/               # Syllabus pages
│   │   ├── ncert-grade6.html
│   │   ├── ncert-grade12-syllabus.html
│   │   ├── ncert-g12-math-syallabus.html
│   │   ├── ncert-g12-physics-syllabus.html
│   │   ├── ncert-g12-chem-syllabus.html
│   │   ├── ncert-g12-biology.html
│   │   ├── ncert-g12-chem-syllabus.html
│   │   ├── ncert-g10-syllabus.html
│   │   ├── ncert-g6-science-chapter.html
│   │   ├── ncert-math-g6-chap*.html
│   │   └── ... (other syllabus files)
│   └── chapters/               # Chapter & Quiz content
│       ├── chapter1-numbers.html
│       ├── math-g6-chapters.html
│       ├── practice.html
│       ├── ncret-grade.html
│       ├── ncret-math-g6-c2.html
│       ├── scert-grade.html
│       ├── scert-grade6.html
│       ├── gr12-ncert-*.html
│       ├── quz-g6-ch1.html
│       ├── quiz-g12-chem-ch1.html
│       ├── quiz-g12-math-ch1.html
│       ├── quiz-g12-phy-ch1.html
│       └── ... (other chapter files)
├── video/                      # Video content
│   ├── video-g6-word-problem.html
│   ├── video-g6-estimation.html
│   ├── video-g6-factors-multiples.html
│   ├── video-g6-comparing-ordering-large-numbers.html
│   ├── video-g6-india-and-inter.html
│   ├── video-g6-math-*.html
│   ├── video-g6-natural-wholenumber.html
│   ├── video-g12-*.html
│   ├── example-video.html
│   ├── eample-vid.html
│   └── ... (other video files)
├── games/                      # Game content
│   ├── game-g6-rounding.html
│   ├── game-g6-word.html
│   ├── game-g6-math-indian.html
│   ├── game-g12-math-chap1.html
│   ├── game-g12-coulumns.html
│   ├── game-g12-gauss.html
│   ├── game-g12-chem-chap1.html
│   ├── math-g6-ch1-game.html
│   ├── 12sample-game.html
│   ├── gametemp.html
│   └── ... (other game files)
├── scripts/                    # Scripts & utilities (pre-existing)
├── aura/                       # Aurora/AURA related files (pre-existing)
├── flutter/                    # Flutter related files (pre-existing)
└── .badge-backups/             # Badge backup files

```

## File Mapping

### HTML Files by Category

#### Authentication Pages
- **login.html** → `auth/login.html`
- **signup.html** → `auth/signup.html`
- **teacher-login.html** → `auth/teacher-login.html`
- **teacher-signup.html** → `auth/teacher-signup.html`
- **signin.html** → `auth/signin.html`

#### Dashboard
- **teacher-dashboard.html** → `dashboard/teacher-dashboard.html`
- **app.js** → `dashboard/app.js`

#### Content/Learning Pages
- **Syllabus files** → `content/syllabus/`
- **Chapter files** → `content/chapters/`
- **Video files** → `video/`
- **Game files** → `games/`

### CSS Files
All CSS files have been moved to `styles/`:
- `badge.css` - Badge styling
- `teacher-dashboard.css` - Dashboard styling
- `chapter1-styles.css` - Chapter content styling
- `grade-styles.css` - Grade selection styling
- `math-g6-chapters-styles.css` - Math chapter styling
- `ncert-grade6-styles.css` - NCERT Grade 6 styling
- `practice-styles.css` - Practice content styling

### JavaScript Files
All JS files have been organized:
- **Authentication** → `auth/` (login.js, student-auth.js, teacher-auth.js, etc.)
- **Utils** → `utils/` (badge.js)
- **Config** → `config/` (firebase.js, dev-server.js)
- **Dashboard** → `dashboard/` (app.js)

## Path Updates Summary

### Updated File References
All HTML files have been updated to reference moved files with correct relative paths:

1. **In auth/ files:**
   - `badge.css` → `../styles/badge.css`
   - `badge.js` → `../utils/badge.js`
   - `firebase.js` → `../config/firebase.js`

2. **In content/ files:**
   - `badge.css` → `../../styles/badge.css`
   - `badge.js` → `../../utils/badge.js`
   - `video-*.html` → `../../video/video-*.html`
   - `game-*.html` → `../../games/game-*.html`
   - `quiz/` → `../../quiz/`

3. **In video/ files:**
   - `badge.css` → `../styles/badge.css`
   - `badge.js` → `../utils/badge.js`

4. **In games/ files:**
   - `badge.css` → `../styles/badge.css`
   - `badge.js` → `../utils/badge.js`

5. **In dashboard/ files:**
   - `teacher-dashboard.css` → `../styles/teacher-dashboard.css`

6. **In index.html:**
   - `teacher-auth.js` → `auth/teacher-auth.js`
   - `student-auth.js` → `auth/student-auth.js`
   - `badge.js` → `utils/badge.js`

## Benefits of This Organization

✅ **Clear Feature Separation** - Each feature has its own directory
✅ **Easier Navigation** - Developers can quickly find related files
✅ **Scalability** - New features can be added in parallel directories
✅ **Maintainability** - CSS and JS files are centralized by type
✅ **Reduced Clutter** - Root directory now only contains landing page
✅ **Better Git History** - Feature branches can modify entire directories

## Notes

- Content files within the same subdirectory (e.g., all files in `content/chapters/`) maintain relative links without path prefixes
- External resources (CDN links, APIs) remain unchanged
- Pre-existing folders (`aura/`, `flutter/`, `quiz/`, `scripts/`) were left in place
- File permissions preserved during migration

