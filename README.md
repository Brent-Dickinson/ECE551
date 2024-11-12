# ECE551 Term Paper Repository

This repository contains our ECE551 term paper, written in LaTeX using the IEEE template.

## Initial Setup

### 1. Installing LaTeX and TeXstudio

#### Windows
1. Download and install MiKTeX from [https://miktex.org/download](https://miktex.org/download)
2. Download and install TeXstudio from [https://www.texstudio.org](https://www.texstudio.org)

#### macOS
1. Download and install MacTeX from [https://www.tug.org/mactex/](https://www.tug.org/mactex/)
2. Download and install TeXstudio from [https://www.texstudio.org](https://www.texstudio.org)

#### Linux
```bash
# For Ubuntu/Debian
sudo apt-get update
sudo apt-get install texlive-full texstudio

# For Fedora
sudo dnf install texlive-scheme-full texstudio
```

### 2. Testing Your LaTeX Installation

1. Open TeXstudio
2. First, open and compile the IEEE template file (`IEEE template.tex`)
   - This file contains important formatting instructions and examples
   - Keep this file as a reference for LaTeX commands and styling
   - A successful compilation confirms your LaTeX setup is working
3. Then, open the paper file (`paper.tex`)
   - This is where we'll write our actual term paper
   - It's based on the IEEE template but stripped down to essentials
4. Click the "Build & View" button (green play button) or press F5 to compile

## GitHub Workflow

### Initial Repository Setup

```bash
# Clone the repository
git clone https://github.com/Brent-Dickinson/ECE551.git
cd ECE551
```

### Regular Workflow

Always follow these steps when working on the paper:

1. Before starting work:
```bash
# Get the latest changes
git pull origin main
```

2. While working:
```bash
# Check status of your changes
git status

# Add your changes
git add .

# Commit your changes with a descriptive message
git commit -m "Description of your changes"
```

3. After completing work:
```bash
# Push your changes
git push origin main
```

### Best Practices

1. Pull before starting any new work
2. Commit frequently with clear messages
3. Push your changes at the end of each working session
4. Communicate with your partner about major changes
5. Keep backup copies of important files

## Repository Structure

```
├── IEEE template.tex  # Original IEEE template with formatting instructions
├── paper.tex         # Our term paper
└── figures/          # Directory for images and figures
```

## Bibliography Notes

The bibliography will be written directly in the paper.tex file using the IEEE format:

```latex
\begin{thebibliography}{00}
\bibitem{ref1} Author(s), "Title of paper," Journal Name, vol. x, no. x, pp. xxx-xxx, Month Year.
\bibitem{ref2} Author(s), "Title of book," Publisher, Year.
\end{thebibliography}
```

To cite references in the text, use the `\cite{ref1}` command.

## Common Issues and Solutions

1. **LaTeX compilation errors**
   - Check the log file for specific error messages
   - Ensure all required packages are installed
   - Verify syntax in recent changes
   - Refer to `IEEE template.tex` for correct formatting examples

2. **Git merge conflicts**
   - Communicate with your partner before making major changes
   - Resolve conflicts by carefully reviewing both versions
   - When in doubt, make a backup before attempting to resolve

## Additional Resources

- [LaTeX Tutorial](https://www.latex-tutorial.com)
- [IEEE Template Documentation](https://www.ieee.org/conferences/publishing/templates.html)
- [Git Documentation](https://git-scm.com/doc)
