# LaTeX-Packages-Ubuntu

Installing packages for LaTeX:

1. Download the package file from ctan website, by searching on google for '<package_name>.sty ctan'.

2. Extract the files from the package downloaded.

  2.1. If there is no <package_name>.sty file found and <package_name>.ins file is present, run the following command in terminal after changing to the folder of downloaded package.
       latex <package_name>.ins

3. Make a new folder inside the package directory of LaTeX software using the following command:
   sudo mkdir /usr/share/texlive/texmf-dist/tex/latex/<package_name>

4. Now move the <package_name>.sty to the LaTeX software using the command:
   sudo mv <package_name>.sty /usr/share/texlive/texmf-dist/tex/latex/<package_name>/

5. After moving, update the package repository of LaTeX using the command:
   sudo texhash

6. Reopen the TexStudio or any IDE to use the newly added package.
