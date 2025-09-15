# Ashley Mathews Resume (LaTeX)

This repository contains the LaTeX source code for Ashley Mathews' professional resume. The project is designed for easy editing, modularity, and compatibility with modern applicant tracking systems (ATS).

## Features
- **Modular LaTeX Structure:** Each resume section (header, experience, education, etc.) is in its own `.tex` file for easy editing and maintenance.
- **Modern Font:** Uses Arial via XeLaTeX for ATS compatibility and a clean, professional look.
- **Colorful Section Headings:** Section titles are styled in a custom blue for visual appeal.
- **Clickable Links:** Email and LinkedIn are clickable in the PDF.
- **Minimal Dependencies:** Designed to work with [BasicTeX](https://www.tug.org/mactex/morepackages.html) (a minimal TeX Live distribution for macOS).

## Requirements
- **macOS** (or any OS with TeX Live)
- [BasicTeX](https://www.tug.org/mactex/morepackages.html) (or full MacTeX/TeX Live)
- `tlmgr` (TeX Live Manager, for installing extra packages)
- **XeLaTeX** (Unicode-aware LaTeX engine)

## Setup Instructions

1. **Install BasicTeX** (if not already installed):
   - Download and install from [here](https://www.tug.org/mactex/morepackages.html)

2. **Install Required LaTeX Packages:**
   - Open Terminal and run:
     ```sh
     sudo tlmgr update --self
     sudo tlmgr install xcolor fontspec enumitem titlesec marvosym fullpage tabularx fontawesome5 multicol graphicx hyperref babel
     ```

3. **Clone this Repository:**
   ```sh
   git clone https://github.com/rishabhmalhotra/ashley_resume_latex.git
   cd ashley_resume_latex
   ```

4. **Build the Resume PDF:**
   - Use XeLaTeX to compile:
     ```sh
     xelatex main.tex
     ```
   - Or use a LaTeX editor (e.g., VS Code with LaTeX Workshop) and select XeLaTeX as the compiler.

5. **Output:**
   - The compiled PDF will be `main.pdf` in the project directory.

## File Structure

- `main.tex` — Main entry point, includes all sections
- `preamble.tex` — Packages, color definitions, and custom commands
- `header.tex` — Name, contact info, and links
- `experience.tex` — Employment experience
- `volunteer.tex` — Volunteer work
- `education.tex` — Education history
- `achievements.tex` — Awards and achievements
- `skills.tex` — Technical skills

## Notes
- **Font:** Arial is set via `fontspec` and XeLaTeX for maximum ATS compatibility.
- **PDF Links:** Email and LinkedIn are clickable in the output PDF.
- **Customization:** Edit the section `.tex` files to update your information.

## License
MIT License. See `LICENSE` file for details.

---

For any issues or suggestions, please open an issue or pull request on GitHub.
