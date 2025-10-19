# MS Thesis LaTeX Template: Quantum Steering in RDQBL

## Overview
This is a comprehensive LaTeX template for your Master of Science thesis on **Continuous-Variable Quantum Steering in a Raman-Driven Quantum Beat Laser (RDQBL)**.

**Author:** [Your Name]
**Supervisor:** Dr. Shakir Ullah
**Department:** Physics, Quaid-i-Azam University, Islamabad
**Year:** 2025-2026

---

## 📁 File Structure

```
Thesis/
├── MS_Thesis_Steering.tex          # Main thesis file (COMPILE THIS)
├── Chapter_1_Introduction.tex       # Chapter 1: Introduction
├── Chapter_2_Theory.tex             # Chapter 2: Theory & Literature Review
├── Chapter_3_Model.tex              # Chapter 3: Model & Methodology
├── Chapter_4_Results.tex            # Chapter 4: Results & Analysis
├── Chapter_5_Discussion.tex         # Chapter 5: Discussion
├── Chapter_6_Conclusions.tex        # Chapter 6: Conclusions
├── Chapter_7_References.tex         # Chapter 7: References
├── Sample.bib                       # Bibliography database
├── README.md                        # This file
└── QAU_enhanced_Logo.jpg            # University logo (update filename if needed)
```

---

## 🚀 Quick Start

### Prerequisites
You need the following installed:
- **LaTeX Distribution:** MiKTeX (Windows), TeX Live (Linux), MacTeX (Mac)
- **LaTeX Editor:** TeXstudio, Overleaf (online), VS Code (with LaTeX extension)
- **BibTeX:** Usually included with LaTeX distribution

### Compilation Instructions

#### Option 1: Using TeXstudio (Recommended)
1. Open `MS_Thesis_Steering.tex`
2. Click **Build & View** (or press F5)
3. PDF will be generated automatically

#### Option 2: Command Line
```bash
cd "C:\Users\quanta\Documents\MS Research\Thesis"

# Full compilation cycle
pdflatex MS_Thesis_Steering.tex
bibtex MS_Thesis_Steering
pdflatex MS_Thesis_Steering.tex
pdflatex MS_Thesis_Steering.tex
```

#### Option 3: Overleaf (Online)
1. Create new project on [Overleaf.com](https://www.overleaf.com)
2. Upload all `.tex` and `.bib` files
3. Click **Recompile** to generate PDF

---

## ✏️ How to Edit Your Thesis

### 1. Update Personal Information
**File:** `MS_Thesis_Steering.tex`

Find and replace:
```latex
{\Large \textbf{[Your Name]} \par}           % Line ~65
{\centering\large (Reg. \# [Your Registration Number])}  % Line ~94
```

### 2. Update Logo
If your logo filename is different:
```latex
\includegraphics[width=7.7cm]{QAU_enhanced_Logo}  % Update filename
```

### 3. Edit Chapter Content
Each chapter is in a separate file. Example:

**File:** `Chapter_1_Introduction.tex`

The chapter structure is already provided with sections and subsections. You can:
- Add your content under existing sections
- Modify section headers
- Add new sections as needed

### 4. Add/Modify Bibliography

**File:** `Sample.bib`

Add new references in BibTeX format:
```bibtex
@article{AuthorYear,
  author = {Author, A. and Other, B.},
  title = {Title of Article},
  journal = {Journal Name},
  volume = {10},
  pages = {123--145},
  year = {2024}
}
```

Then cite in your text:
```latex
\cite{AuthorYear}
```

---

## 📝 Writing Guidelines

### Chapter Templates
Each chapter follows this structure:

```latex
\chapter{Chapter Title}
\label{chpX}

\section{Section 1}
Your content here...

\subsection{Subsection}
More content...
```

### Formatting Text
- **Bold:** `\textbf{text}`
- **Italic:** `\textit{text}`
- **Bold + Italic:** `\textbf{\textit{text}}`
- **Monospace:** `\texttt{text}`

### Equations
Inline equation: `$E = mc^2$`

Display equation:
```latex
\begin{equation}
E = mc^2
\label{eq:einstein}
\end{equation}
```

Reference equation: `Equation \ref{eq:einstein}`

### Lists
Bullet list:
```latex
\begin{itemize}
  \item First point
  \item Second point
\end{itemize}
```

Numbered list:
```latex
\begin{enumerate}
  \item First point
  \item Second point
\end{enumerate}
```

### Figures
```latex
\begin{figure}[h]
  \centering
  \includegraphics[width=0.8\textwidth]{figure_name.pdf}
  \caption{Figure description}
  \label{fig:label}
\end{figure}
```

Reference figure: `Figure \ref{fig:label}`

### Tables
```latex
\begin{table}[h]
  \centering
  \begin{tabular}{ll}
    \hline
    Column 1 & Column 2 \\
    \hline
    Data 1 & Data 2 \\
    \hline
  \end{tabular}
  \caption{Table description}
  \label{tab:label}
\end{table}
```

---

## 🎨 Document Features

### Automatically Generated
- ✅ Title pages (3 pages)
- ✅ Certification page
- ✅ Dedication page
- ✅ Table of Contents
- ✅ List of Figures
- ✅ List of Tables
- ✅ Page numbering (Roman for front matter, Arabic for main content)
- ✅ Hyperlinks (clickable in PDF)

### Formatting Applied
- ✅ 1.4x line spacing (adjustable in line 6)
- ✅ Professional fonts (Times New Roman)
- ✅ Proper margins (1.5" left, 1.0" others)
- ✅ Chapter formatting with centering and spacing
- ✅ Blue hyperlinks for references and TOC

---

## 🔧 Customization

### Change Title
**File:** `MS_Thesis_Steering.tex` (Lines ~53, ~85)
```latex
{\LARGE \textbf{Your New Title} \par}
```

### Change Supervisor Name
**File:** `MS_Thesis_Steering.tex` (Lines ~69, ~99)
```latex
{\Large \textbf{Dr. New Supervisor Name} \par}
```

### Change Line Spacing
**File:** `MS_Thesis_Steering.tex` (Line 6)
```latex
\renewcommand{\baselinestretch}{1.5}  % Change 1.4 to desired value
```

### Change Colors
**File:** `MS_Thesis_Steering.tex` (Line 55)
```latex
\usepackage[colorlinks=true, allcolors=blue]{hyperref}
% Change 'blue' to red, black, etc.
```

---

## ⚠️ Common Issues & Solutions

### Issue: "pdfinclude.sty not found"
✅ **Solution:** Already fixed in this template. The invalid package has been removed.

### Issue: "Package xcolor Warning"
✅ **Solution:** This is just a warning, not an error. Your PDF will still compile.

### Issue: Bibliography not appearing
✅ **Solution:**
1. Make sure `Sample.bib` is in same directory
2. Run: `pdflatex → bibtex → pdflatex → pdflatex`
3. Don't forget the middle `bibtex` step!

### Issue: Figures not showing
✅ **Solution:**
- Ensure image files are in thesis folder
- Use `.pdf`, `.jpg`, or `.png` format
- Check filename spelling in `\includegraphics{}`

### Issue: Table of Contents not updating
✅ **Solution:** Recompile twice (LaTeX needs two passes to update TOC)

---

## 📚 Chapter Descriptions

### Chapter 1: Introduction
- Background and motivation
- Problem statement
- Research objectives
- Thesis layout

### Chapter 2: Theory & Literature Review
- Quantum correlations hierarchy
- Continuous-variable systems
- Quantum steering theory
- Previous work review
- Motivation for this work

### Chapter 3: Model & Methodology
- RDQBL physical system
- Hamiltonian formulation
- Master equations
- Covariance matrix formalism
- Steering quantification

### Chapter 4: Results & Analysis
- Steering generation
- Parameter effects
- Robustness analysis
- Experimental validation

### Chapter 5: Discussion
- Physical interpretation
- Robustness mechanisms
- Quantum correlation hierarchy
- Comparison with prior work
- Experimental feasibility

### Chapter 6: Conclusions
- Summary of findings
- Significance and impact
- Limitations
- Recommendations for future work

### Chapter 7: References
- Bibliography database
- All cited sources

---

## 📊 Thesis Statistics Template

After completion, your thesis will have approximately:
- **Page count:** 100-150 pages
- **Figures:** 8-12 research figures
- **Tables:** 5-8 data/comparison tables
- **References:** 60-80 citations
- **Equations:** 200+ mathematical expressions

---

## 🎓 Before Submission

### Checklist
- [ ] All chapters completed and proofread
- [ ] All figures inserted with proper captions
- [ ] All citations formatted correctly
- [ ] Bibliography compiled with BibTeX
- [ ] Page numbers correct (Roman front matter, Arabic main)
- [ ] Table of Contents updated
- [ ] Dedication page completed
- [ ] Acknowledgments written
- [ ] Abstract finalized
- [ ] Supervisor certification page signed

### Final PDF Generation
```bash
pdflatex MS_Thesis_Steering.tex
bibtex MS_Thesis_Steering
pdflatex MS_Thesis_Steering.tex
pdflatex MS_Thesis_Steering.tex
```

Save the final `MS_Thesis_Steering.pdf` for submission.

---

## 📞 Support & Resources

### LaTeX Learning
- [Overleaf Learn LaTeX](https://www.overleaf.com/learn)
- [ShareLaTeX Documentation](https://www.sharelatex.com/learn/Learn_LaTeX_in_30_minutes)
- [The Not So Short Introduction to LaTeX](https://tobi.oetiker.ch/lshort/)

### Packages Used
- `geometry` - Page margins
- `graphicx` - Graphics inclusion
- `amsmath` - Advanced mathematics
- `hyperref` - Hyperlinks
- `natbib` - Bibliography styling
- `titlesec` - Section formatting

---

## ✨ Notes

- **Template Created:** October 2025
- **Last Updated:** October 18, 2025
- **Compatible with:** MiKTeX, TeX Live, Overleaf
- **Main Document:** `MS_Thesis_Steering.tex`

**Remember:** Always backup your work! Keep copies in multiple locations.

---

**Good luck with your thesis! 🎓**

