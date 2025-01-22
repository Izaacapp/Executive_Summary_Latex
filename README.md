<a name="readme-top"></a>

<div align="center">
  
  [![Contributors][contributors-shield]][contributors-url]
  [![Forks][forks-shield]][forks-url]
  [![Stargazers][stars-shield]][stars-url]
  [![Issues][issues-shield]][issues-url]
  [![LinkedIn][linkedin-shield]][linkedin-url]
</div>

<br />
<div align="center">
  <a href="https://github.com/Izaacapp/Executive_Summary_Latex">
    <img src="binary.png" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">Executive Summary LaTeX Template</h3>

  <p align="center">
    A customizable LaTeX template for professional executive summaries, with support for LuaLaTeX and XeLaTeX.
    <br />
    <a href="https://github.com/Izaacapp/Executive_Summary_Latex"><strong>Explore the docs »</strong></a>
    <br />
    <br />
  </p>
</div>



<details>
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#about-the-project">About The Project</a></li>
    <li><a href="#features">Features</a></li>
    <li><a href="#installation-and-setup">Installation and Setup</a></li>
    <li><a href="#configuration">Configuration</a></li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>



## About The Project

This project is a LaTeX-based executive summary template. It was initially developed in Overleaf but later adapted for local compilation using **LuaLaTeX** and **XeLaTeX** to avoid Overleaf's timeout limitations. The template supports custom fonts and styles, ensuring professional-quality output.




## Features

- Support for **LuaLaTeX** and **XeLaTeX** for extended font compatibility.
- Customizable `.tex` and `.bib` files.
- Visual Studio Code integration via the `latex-workshop` extension.
- Easy configuration for local compilation.




## Installation and Setup

### Prerequisites

1. **LaTeX Distribution**: Install [TeX Live](https://www.tug.org/texlive/) or [MacTeX](https://www.tug.org/mactex/) for Mac users.  
2. **Fonts**: Install the required fonts locally for accurate rendering.
3. **Visual Studio Code**: Install [Visual Studio Code](https://code.visualstudio.com/).
4. **VS Code Extensions**: Install the [LaTeX Workshop](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop) extension.



### Installation Steps

#### For UNIX-based Systems

1. Download and extract the TeX Live installer:
   ```bash
   tar -xvzf install-tl-unx.tar.gz
   cd install-tl-<version>
   ```
2. Run the installer with permissions:
   ```bash
   sudo perl install-tl -v -gui text
   ```
3. Configure the installer with your preferences (default settings are recommended).
4. Add TeX Live binaries to your `PATH`:
   ```bash
   export PATH=/path/to/texlive/bin:$PATH
   ```
5. Verify the installation:
   ```bash
   which kpsewhich
   which lualatex
   ```
   Both should point to your TeX Live installation.

#### For Mac M1 Users

1. Download [MacTeX](https://www.tug.org/mactex/).
2. Run the installer and follow the instructions.
3. Verify the installation:
   ```bash
   which lualatex
   lualatex --version
   ```





## Configuration

### LaTeX Workshop Settings

Update the `settings.json` file in Visual Studio Code with the following configuration:

```json
"latex-workshop.latex.recipe.default": "latexmk (lualatex)",
"latex-workshop.latex.recipes": [
    {
        "name": "latexmk (lualatex)",
        "tools": ["lualatex"]
    },
    {
        "name": "latexmk (xelatex)",
        "tools": ["xelatex"]
    }
],
"latex-workshop.latex.tools": [
    {
        "name": "lualatex",
        "command": "lualatex",
        "args": [
            "-synctex=1",
            "-interaction=nonstopmode",
            "-file-line-error",
            "%DOC%"
        ]
    },
    {
        "name": "xelatex",
        "command": "xelatex",
        "args": [
            "-synctex=1",
            "-interaction=nonstopmode",
            "-file-line-error",
            "%DOC%"
        ]
    }
]
```





## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/Izaacapp/Executive_Summary_Latex.git
   cd Executive_Summary_Latex
   ```
2. Open the project in Visual Studio Code.
3. Edit `executive_summary.tex` and `bibliography.bib` to customize the template.
4. Compile the project using `LuaLaTeX` or `XeLaTeX`.



## Contributing

Contributions are welcome! Fork the repository, create a feature branch, and submit a pull request.





## License

Distributed under the MIT License. See `MIT-LICENSE.txt` for details.





## Contact

Izaac Plambeck  
[Tweet me](https://x.com/Izaacapp)  
[Email me](mailto:izaacap@gmail.com)





## Acknowledgments

- [Overleaf](https://www.overleaf.com)
- [LaTeX Workshop](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop)
- [TeX Live](https://www.tug.org/texlive/)
- [MacTeX](https://www.tug.org/mactex/)



<!-- MARKDOWN LINKS & IMAGES -->
[contributors-shield]: https://img.shields.io/badge/Contributors-violet?style=for-the-badge
[contributors-url]: https://github.com/Izaacapp/Executive_Summary_Latex/graphs/contributors
[forks-shield]: https://img.shields.io/badge/Forks-green?style=for-the-badge
[forks-url]: https://github.com/Izaacapp/Executive_Summary_Latex/network/members
[stars-shield]: https://img.shields.io/badge/Stars-gold?style=for-the-badge
[stars-url]: https://github.com/Izaacapp/Executive_Summary_Latex/stargazers
[issues-shield]: https://img.shields.io/badge/Issues-red?style=for-the-badge
[issues-url]: https://github.com/Izaacapp/Executive_Summary_Latex/issues
[license-shield]: https://img.shields.io/github/license/Izaacapp/Executive_Summary_Latex.svg?style=for-the-badge
[license-url]: https://github.com/Izaacapp/Executive_Summary_Latex/blob/main/LICENSE
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/izaac-plambeck/

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<p align="right"> <a href="https://github.com/Izaacapp/Executive_Summary_Latex/issues/new?labels=bug&template=bug-report---.md">Report Bug</a>

<p align="right"> <a href="https://github.com/Izaacapp/Executive_Summary_Latex/issues/new?labels=enhancement&template=feature-request---.md">Request Feature</a>