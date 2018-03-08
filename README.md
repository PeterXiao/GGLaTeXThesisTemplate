# GGLaTeXThesisTemplate
LaTeX templates for theses.

## Compiling

This LaTeX document is tested with the following tools
1. **[ShareLaTeX](https://www.sharelatex.com/)**
2. **[Atom](https://atom.io/)** editor in combination with **[Tex Live](http://www.tug.org/texlive/)** on Debian 9

### ShareLaTeX

* The used compiler is **XeLaTeX**.
* The main document is **main.tex**.

### Atom and TeX Live

#### TeX Live installation

Install TeX Live with the required packages. Therefore execute the below command
```
apt-get install texlive texlive-xetex texlive-lang-german texlive-bibtex-extra biber latexmk
```
#### Atom installation
To build with the [Atom](https://atom.io/) editor on Debian 9 "Stretch" you have to execute the below steps.

1. Download the .deb package from https://atom.io/
2. Install Atom with the command
```
dpkg -i /path/to/deb/file/atom-amd64.deb
```
3. Run Atom and install the packages
    * `atom-latex`
        * v0.8.2: There is a known issue on UNIX systems https://github.com/James-Yu/Atom-LaTeX/issues/110. (Fixed in version v0.8.3)<br>
        Therefore you have to edit the file `/home/<user>/.atom/packages/atom-latex/lib/builder.coffee` in line 66 from `@buildErrs += data` to `@buildErrs[@buildErrs.length - 1] += data`
    * `language-latex`
4. Open the `atom-latex` package settings and change
    * `LaTeX compiler to use` to `xelatex`
    * `BibTex compiler to use` to `biber`
    * Add to the default values of `Files to clean` the file extensions `*.xml, *.gz, *.atfi, *.bcf, *.maf, *mtc*, *.ilg, *.lol`
    * make sure that `Clean LaTeX auxiliary files after building process` is enabled.

## 3rd Party

### Fonts

* Arial
* Times New Roman

### Images

* images/content/nate-grant-346782.jpg
    * Source: [Unsplash](https://unsplash.com/photos/QQ9LainS6tI)
    * License: [do whatever you want](https://unsplash.com/license)
* images/content/ben-kolde-367194.jpg
    * Source: [Unsplash](https://unsplash.com/photos/lqZPleZ4ERA)
    * License: [do whatever you want](https://unsplash.com/license)
