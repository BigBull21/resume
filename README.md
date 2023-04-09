# 📋 Résumé + CV + Coverletter
A repository containing the LaTeX source of Aaron Rinehart's résumé, curriculum vitae, and coverletter matter. Tested and deployed with GitHub Actions.

---
[![résumé last release](https://img.shields.io/github/release-date/bigbull21/resume?logo=github&label=Last%20Release)](https://github.com/bigbull21/resume/releases)
[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/bigbull21/resume/ci.yml?logo=github&label=CI)](https://github.com/bigbull21/resume/actions/workflows/ci.yml)

# 🤖 Deployment
Deployment is automated by [GitHub Actions](https://github.com/bigbull21/resume/actions).
- Pushes to `main` trigger a new release of the [latest résumé, cv, and cover letter](https://github.com/bigbull21/resume/releases/tag/latest), available in several formats.
  | Artifact               | Link                                                                          | Mirror                                         |
  | ---------------------- | ----------------------------------------------------------------------------- | ---------------------------------------------- |
  | Résumé                 | <https://bigbull21.github.io/resume/resume.html>                               | <https://bigbull21.github.io/resume/>           |
  | Résumé, Embedded       | <https://bigbull21.github.io/resume/resume-embed.html>                         | <https://bigbull21.github.io/resume/embed.html> |
  | Résumé, Download       | <https://github.com/bigbull21/resume/releases/download/latest/resume.pdf>      |                                                |
  | CV                     | <https://bigbull21.github.io/resume/cv.html>                                   |                                                |
  | CV, Embedded           | <https://bigbull21.github.io/resume/cv-embed.html>                             |                                                |
  | CV, Download           | <https://github.com/bigbull21/resume/releases/download/latest/cv.pdf>          |                                                |
  | Cover letter           | <https://bigbull21.github.io/resume/coverletter.html>                          |                                                |
  | Cover letter, Embedded | <https://bigbull21.github.io/resume/coverletter-embed.html>                    |                                                |
  | Cover letter, Download | <https://github.com/bigbull21/resume/releases/download/latest/coverletter.pdf> |                                                |
- Manually pushed [releases](https://github.com/bigbull21/resume/releases) also trigger workflows to upload artifacts.

# 🔧 Building
## Dependencies
- [TeXLive, full](https://www.tug.org/texlive/)
- [Make](https://www.gnu.org/software/make/)
- [j2cli](https://github.com/kolypto/j2cli)
## Commands
- **Build the résumé**:
  ```bash
  make resume
  ```
- **Build the cirriculum vitae**:
  ```bash
  make cv
  ```
- **Build the cover letter**:
  ```bash
  make coverletter
  ```
- **Build all**:
  ```bash
  make all
  ```
- **Purge all**:
  ```bash
  make clean
  ```
- **Open PDFs**:
  ```bash
  make open
  ```

# 🔏 License
This project is [MIT](./LICENSE) licensed. You are within your rights to fork my résumé and use it as your own, although you should probably change my name to yours.
