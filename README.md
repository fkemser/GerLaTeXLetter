
<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
<a name="readme-top"></a>
<!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Don't forget to give the project a star!
*** Thanks again! Now go create something AMAZING! :D
-->



<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![GNU GPL v3.0 License][license-shield]][license-url]
<!-- [![LinkedIn][linkedin-shield]][linkedin-url] -->



<!-- PROJECT LOGO -->
<br />
<div align="center">
  <!-- <a href="https://github.com/fkemser/GerLaTeXLetter">
    <img src="images/logo.png" alt="Logo" width="80" height="80">
  </a> -->

<h3 align="center">GerLaTeXLetter</h3>

  <p align="center">
    A LaTeX template for business letters (mostly) following German DIN 5008 standard, based on KOMA-Script class 'scrlttr2'.
    <br />
    <a href="https://github.com/fkemser/GerLaTeXLetter"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/fkemser/GerLaTeXLetter">View Demo</a>
    ·
    <a href="https://github.com/fkemser/GerLaTeXLetter/issues">Report Bug</a>
    ·
    <a href="https://github.com/fkemser/GerLaTeXLetter/issues">Request Feature</a>
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
        <li><a href="#testing-environment">Testing Environment</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li>
          <a href="#prerequisites">Prerequisites</a>
          <ul>
            <li><a href="#debian">Debian</a></li>
            <li><a href="#tex-live-package-manager">TeX Live Package Manager (tlmgr)</a></li>
          </ul>
        </li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li>
      <a href="#customization">Customization</a>
      <ul>
        <li><a href="#headerlco-headerfooterinformation-block-template">header.lco (Header/Footer/Information Block Template)</a></li>
        <li><a href="#lettertex-individual-letter">letter.tex (Individual Letter)</a></li>
        <li><a href="#logopng-sample-logo">logo.png (Sample Logo)</a></li>
        <li><a href="#lettertex-individual-letter">template.lco (General Letter Template)</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

[![Product Name Screen Shot][screenshot1]](res/letter.pdf)
[![Product Name Screen Shot][screenshot2]](res/letter.pdf)

During my research on writing letters with [LaTeX][LaTeX-url] and [KOMA-Script][scrlttr2-url] I encountered many great templates on the web. However, none of them met all my requirements so I decided to create my own one. This template offers

* a structured layout, mostly following German [DIN 5008][din5008] standard,
* a customizable logo placeholder, information block, and footer
* an automatically created vCard QR code with your (company's) contact details, allowing the recipient to store them in their smartphone, and
* code snippets allowing you to
  * include OS environmental variables in your letter, e.g. as used in the [TeXLetterCreator](https://github.com/fkemser/TeXLetterCreator) project,
  * create multi-lingual documents.

<p align="right">(<a href="#readme-top">back to top</a>)</p>



### Built With

[![LaTeX][LaTeX-shield]][LaTeX-url]
[![Shell Script][Shell Script-shield]][Shell Script-url]

<p align="right">(<a href="#readme-top">back to top</a>)</p>



### Testing Environment

The project has been developed and tested on the following system:

| Info | Description
---: | ---
OS | Debian GNU/Linux 12 (bookworm)
Kernel | 5.15.90.1-microsoft-standard-WSL2
Packages | [texlive-latex-recommended (2022.20230122-3)](https://packages.debian.org/bookworm/texlive-latex-recommended)
|| [texlive-luatex (2022.20230122-3)](https://packages.debian.org/bookworm/texlive-luatex)
|| [xz-utils (5.4.1-0.2)](https://packages.debian.org/bookworm/xz-utils)

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- PREREQUISITES -->
## Prerequisites

Please make sure that the following dependencies are installed:

* [XZ Utils](https://xz.tukaani.org/xz-utils/)
* TeX distribution of your choice, e.g. [TeX Live](https://www.tug.org/texlive/)
* [LuaTeX](https://www.luatex.org/) engine
* Packages (CTAN)
  [afterpage](https://www.ctan.org/pkg/afterpage), [babel](https://www.ctan.org/pkg/babel), [babel-english](https://www.ctan.org/pkg/babel-english), [babel-german](https://www.ctan.org/pkg/babel-german), [catchfile](https://www.ctan.org/pkg/catchfile), [enumitem](https://www.ctan.org/pkg/enumitem), [etoolbox](https://www.ctan.org/pkg/etoolbox), [fontawesome5](https://www.ctan.org/pkg/fontawesome5), [graphicx](https://www.ctan.org/pkg/graphicx), [iflang](https://www.ctan.org/pkg/iflang), [ifthen](https://www.ctan.org/pkg/ifthen), [qrcode](https://www.ctan.org/pkg/qrcode),  [scrlayer-scrpage](https://www.ctan.org/pkg/scrlayer-scrpage), [scrlttr2](https://www.ctan.org/pkg/scrlttr2), [sourcesanspro](https://www.ctan.org/pkg/sourcesanspro), [tabularx](https://www.ctan.org/pkg/tabularx), [xstring](https://www.ctan.org/pkg/xstring)

Below you can find distribution-specific installation instructions.

> :exclamation: Please **do not forget to install the [additional CTAN packages](#tex-live-package-manager)** after (!) the distribution-specific package installation.

### Debian

```sh
> sudo apt install texlive-latex-recommended texlive-luatex xz-utils
```

### TeX Live Package Manager (tlmgr)

**Some CTAN packages listed above are not included in the distributions' packages**. However, they can be manually installed by using the **TeX Live package manager** `tlmgr`.

Before continuing please make sure that `tlmgr`'s **user mode has been initialized** by running the following command:

```sh
> tlmgr init-usertree
```

In case you skip this step you may get an error during installation:

> (running on Debian, switching to user mode!)  
> (see /usr/share/doc/texlive-base/README.tlmgr-on-Debian.md)  
> TLPDB: not a directory, not loading: /home/user/texmf  
> tlmgr: **user mode not initialized**, please read the documentation!

Now you can **install the required CTAN packages**:

```sh
> tlmgr install babel-english babel-german blindtext catchfile enumitem fontawesome5 qrcode sourcesanspro xstring
```

In some cases the **installation may fail** with a message similar to the following one:

> tlmgr: **Local TeX Live (2022) is older than remote repository (2023)**.  
> Cross release updates are only supported with  
>   update-tlmgr-latest(.sh/.exe) --update  
> See https://tug.org/texlive/upgrade.html for details.

In those cases the version of the TeX Live system installed via your distribution's package manager does not match the version of `tldr`'s default repository. **To fix this problem:**

1. **Figure out the year of your local TeX Live system** by running the following command:

    ```sh
    > tex --version
    ```
   The output may look like this:

    > TeX 3.141592653 (TeX Live **2022**/Debian)  
    > kpathsea version 6.3.4  
    > Copyright 2022 D.E. Knuth.  
    > ...

2. **Add the repository** while replacing `<year>` by the year from step 1 (**2022** here).

    ```sh
    > tlmgr option repository ftp://tug.org/historic/systems/texlive/<year>/tlnet-final
    ```

    In case you would like to use another mirror please have a look at: https://tug.org/historic/

Next we will **install the necessary hyphenation pattern packages**.
In case you skip this step you may get a warning message when compiling your letter and your LaTeX compiler may use the wrong hyphenation patterns:

```
> Package babel Warning: No hyphenation patterns were preloaded for
> (babel)                the language 'German (new orthography)' into the format.
> 
> (babel)                Please, configure your TeX system to add them and
> (babel)                rebuild the format. Now I will use the patterns
> (babel)                preloaded for \language=0 instead on input line 48.
```

Before continuing please **make sure that the following files can be modified by your current user**:

```sh
> sudo touch                                        \
    /var/lib/texmf/tex/generic/config/language.dat  \
    /var/lib/texmf/tex/generic/config/language.dat.backup
> sudo chown $(id -u):$(id -g)                      \
    /var/lib/texmf/tex/generic/config/language.dat  \
    /var/lib/texmf/tex/generic/config/language.dat.backup
```

Then **install the hyphenation pattern packages** by running:

```sh
> tlmgr install hyphen-german
```

Afterwards, **do not forget to revert the file permission changes**:

```sh
> sudo chown root:root                              \
    /var/lib/texmf/tex/generic/config/language.dat  \
    /var/lib/texmf/tex/generic/config/language.dat.backup
```

> :warning:  The installation process modifies the system-wide `Babel` configuration file `language.dat` (see above). Your (Linux) distribution's package manager may also modify this file in the future, e.g. when updating your TeX base installation. This may result in configuration issues so it is **recommended to backup this file every time you update your TeX distribution packages**.

Optional: In case you have modified the template (and therefore need additional CTAN packages) **you may find the following `tlmgr` commands useful**

```sh
# Search for a package that contains a certain file, e.g. 'loadhyph-de-1996.tex'
> tlmgr search --global --file loadhyph-de-1996.tex

# Show which files belong to a certain package, e.g. 'hyphen-german'
> tlmgr info hyphen-german --list

# List installed packages
> tlmgr list --only-installed
```

**Done!** You can continue with [Installation](#installation).

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- INSTALLATION-->
## Installation

1. Clone the repo
  ```sh
   > git clone https://github.com/fkemser/GerLaTeXLetter.git
   ```
2. Customize the template, see [Customization](#customization).

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- CUSTOMIZATION -->
## Customization

Before writing your first letter you should customize the template. To do so, please have a look at the following repository files:

```
.
├── src
│   ├── header.lco    Header/Footer/Information Block Template
│   ├── letter.tex    Individual Letter
│   ├── logo.png      Sample Logo
│   └── template.lco  General Letter Template
...
```

> :information_source: For more information please also have a look at the comments within the files, the [KOMA-Script documentation][scrlttr2-doc-url] and the [KOMA-Script Wiki][koma-wiki-url].

<p align="right">(<a href="#readme-top">back to top</a>)</p>



### `header.lco` (Header/Footer/Information Block Template)

Open `header.lco` with your favourite editor and replace the example values by your own ones. Generally speaking it is always about the last `{}` of each line.

```latex
\renewcommand{\fromgivennames}{Max}
```

With some variables you are able to not only change their values but also their field descriptor, indicated by `[]`.

```latex
\setkomavar{frombushours1}[Mo - Mi]{08:00 - 17:00}
```

There are also some variables that allow you to set multi-line text:

```latex
\setkomavar{fromroutebus}{%
  11 Musterstraße\newline
  22 Musterplatz%
}
```
> :exclamation:  Please use `\newline` instead of `\\` to set a linebreak.

#### vCard QR Code

By default, a vCard will be generated from the sender's information and printed as a QR code within the information block. To disable this behaviour, simply comment each of the following lines with a `%` at the beginning.

```latex
\newplength{fromvcardheight}
\setplength{fromvcardheight}{1.5cm}
```
#### Logo

To replace the sample logo with your own one, simply replace `logo.png` by your own file. To use a different file name simply replace `{logo}` by your own filename, without any extension. The file must be located in the `src` folder. 

```latex
\setkomavar{fromlogo}{\includegraphics[height=1.25cm]{logo}}
```

To disable the logo just comment the above line with a `%` at the beginning.

<p align="right">(<a href="#readme-top">back to top</a>)</p>



### `letter.tex` (Individual Letter)

> :question:But this is the file to write my individual letter, why should I store anything template-related here?

Well, for writing just one single letter you may skip this section. But in case of form letters you need a template which  `letter.tex` will be the base for.

#### Change language

Edit the following line to change the letter's language: 

```latex
\usepackage[ngerman]{babel}
```
> :warning: At the moment, only `ngerman`, `english`, `USenglish`, and `UKenglish` (all case-sensitive) are supported.

This will not only change the information block's descriptors but also any text within the letter for which you have defined language-dependent variables. It also loads language-specific hyphenation patterns.

#### Variables

You can define your own variables by using the following command, where `varname` is the variable's name and `description` its (optional) description.
```latex
\newkomavar[description]{varname}
```

To use the variable or its description (`*`) within the letter just use:
```latex
\usekomavar{varname}  % Variable
\usekomavar*{varname} % Descriptor
```

For multi-lingual documents you can define language-dependent values:

```latex
% Default
\setkomavar{varname}{value_default}

% ngerman
\IfLanguagePatterns{ngerman}{%
  \setkomavar{varname}{value_ngerman}
}{}
```

The same applies to descriptions:

```latex
% Default
\setkomavar*{varname}{description_default}

% ngerman
\IfLanguagePatterns{ngerman}{%
  \setkomavar*{varname}{description_ngerman}
}{}
```

#### Environmental variables

To use your system's environmental variables within your letter:

1. Define a new variable where `envvarname` is the environmental variable's name (within your system) and `macroname` the macro (variable) name that you will use within your letter.

  ```latex
  \getenv[\macroname]{envvarname}
  ```
2. In your letter simply use `\macroname` wherever you would like to use the variable's value.

#### Addressee-independent variables

When writing form letters there may be some addressee-related parts that do not change, e.g. subject, closing, etc. You can set them within the `Addressee-independent` section.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

### `logo.png` (Sample Logo)

See [Logo](#logo) section above.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

### `template.lco` (General Letter Template)

To change the letter's general appearance please edit `template.lco`. However, this is only recommended for experienced users.

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- USAGE-->
## Usage

To write your individual letter, open `letter.tex` and edit the following two sections:

| Section | Description |
---: | ---
`ADDRESSEE` | Recipient-related information, e.g. name, address, etc.
`BODY` | Letter body (text)

> :exclamation:A manual `\pagebreak`  has to be set after each page, otherwise the textwdith will not be calculated correctly.

To create the final PDF of your letter, change into the `src` directory and run the following command:

```sh
> lualatex letter
```

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- ROADMAP -->
## Roadmap

See the [open issues](https://github.com/fkemser/GerLaTeXLetter/issues) for a full list of proposed features (and known issues).

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- LICENSE -->
## License

Distributed under the **MIT License**. See [`LICENSE`][license-url] for more information.

> :warning: The license above does not apply to the sample logo file `/src/logo.png`. For more information please have a look at [Logoipsum's terms of license](https://logoipsum.com/license).

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- CONTACT -->
## Contact

Project Link: [https://github.com/fkemser/GerLaTeXLetter](https://github.com/fkemser/GerLaTeXLetter)

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

###
* [KOMA-Script](https://komascript.de/)
* [Logoipsum](https://logoipsum.com/) (`src/logo.png`)

###
* [The LaTeX Project](https://www.latex-project.org/)
* [TeX Live - TeX Users Group (tug.org)](https://www.tug.org/texlive/)
* [LuaTeX](https://www.luatex.org/)

###
* [afterpage (CTAN)](https://www.ctan.org/pkg/afterpage)
* [babel (CTAN)](https://www.ctan.org/pkg/babel)
* [catchfile (CTAN)](https://www.ctan.org/pkg/catchfile)
* [enumitem (CTAN)](https://www.ctan.org/pkg/enumitem)
* [etoolbox (CTAN)](https://www.ctan.org/pkg/etoolbox)
* [fontawesome5 (CTAN)](https://www.ctan.org/pkg/fontawesome5)
* [graphicx (CTAN)](https://www.ctan.org/pkg/graphicx)
* [iflang (CTAN)](https://www.ctan.org/pkg/iflang)
* [ifthen (CTAN)](https://www.ctan.org/pkg/ifthen)
* [qrcode (CTAN)](https://www.ctan.org/pkg/qrcode)
* [scrlayer-scrpage (CTAN)](https://www.ctan.org/pkg/scrlayer-scrpage)
* [sourcesanspro (CTAN)](https://www.ctan.org/pkg/sourcesanspro)
* [scrlttr2 (CTAN)](https://www.ctan.org/pkg/scrlttr2)
* [tabularx (CTAN)](https://www.ctan.org/pkg/tabularx)
* [xstring (CTAN)](https://www.ctan.org/pkg/xstring)
###
* [othneildrew/Best-README-Template](https://github.com/othneildrew/Best-README-Template)
* [Ileriayo/markdown-badges](https://github.com/Ileriayo/markdown-badges)

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/fkemser/GerLaTeXLetter.svg?style=for-the-badge
[contributors-url]: https://github.com/fkemser/GerLaTeXLetter/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/fkemser/GerLaTeXLetter.svg?style=for-the-badge
[forks-url]: https://github.com/fkemser/GerLaTeXLetter/network/members
[stars-shield]: https://img.shields.io/github/stars/fkemser/GerLaTeXLetter.svg?style=for-the-badge
[stars-url]: https://github.com/fkemser/GerLaTeXLetter/stargazers
[issues-shield]: https://img.shields.io/github/issues/fkemser/GerLaTeXLetter.svg?style=for-the-badge
[issues-url]: https://github.com/fkemser/GerLaTeXLetter/issues
[license-shield]: https://img.shields.io/github/license/fkemser/GerLaTeXLetter.svg?style=for-the-badge
[license-url]: https://github.com/fkemser/GerLaTeXLetter/blob/master/LICENSE
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/linkedin_username
[screenshot1]: res/letter-1.png
[screenshot2]: res/letter-2.png

[LaTeX-shield]: https://img.shields.io/badge/latex-%23008080.svg?style=for-the-badge&logo=latex&logoColor=white
[LaTeX-url]: https://www.latex-project.org/
[Shell Script-shield]: https://img.shields.io/badge/shell_script-%23121011.svg?style=for-the-badge&logo=gnu-bash&logoColor=white
[Shell Script-url]: https://pubs.opengroup.org/onlinepubs/9699919799/

[din5008]:https://de.wikipedia.org/wiki/DIN_5008
[koma-wiki-url]:https://sourceforge.net/p/koma-script/_list/wiki
[scrlttr2-doc-url]:http://mirrors.ctan.org/macros/latex/contrib/koma-script/doc/scrguide-en.pdf
[scrlttr2-url]:https://www.ctan.org/pkg/scrlttr2