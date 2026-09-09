# Student Information App

## Project Title
Student Information System

## Team Members
| Name | Register Number | Role | GitHub Username |
|------|------------------|------|------------------|
| TR Vithun | 2547163 | Team Lead / Developer | (add) |
| Amogh Sahore | 2547108 | UI Developer | (add) |
| Baghyasree Roy | 2547118 | JavaScript Developer | (add) |

## Project Description
A simple static web app that displays student information, built as a lab
exercise to practice a collaborative Git workflow (branching, pull requests,
and merge conflict resolution).

## Technologies Used
- HTML
- CSS
- JavaScript

## Git Branching Strategy
- `main` — stable, always deployable
- `feature/ui` — UI/CSS improvements
- `feature/javascript` — "Show Details" button functionality
- `feature/contact` — adds contact information section
- `feature/student-name` / `feature/app-title` — heading text changes (used
  to intentionally create and resolve a merge conflict)

## Pull Requests Created
1. `feature/ui` → `main`
2. `feature/javascript` → `main`
3. `feature/contact` → `main`
4. `feature/student-name` → `main`
5. `feature/app-title` → `main`

## Merge Conflict
**What caused the conflict?**
`feature/student-name` and `feature/app-title` were both branched from the
same commit and both changed the same `<h1>` line in `index.html` to
different text. When `feature/app-title` was merged after
`feature/student-name` was already merged into `main`, Git could not
automatically decide which version of that line to keep.

**How was it resolved?**
The conflict markers (`<<<<<<<`, `=======`, `>>>>>>>`) were opened in
`index.html`, the two versions were manually compared, and a combined
heading was chosen to keep. The markers were removed, the file was staged
with `git add`, and the resolution was committed and pushed.

## How to Run the Application
1. Clone the repository.
2. Open `index.html` in any web browser.
3. No build steps, server, or database are required.
