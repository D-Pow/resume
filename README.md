# [My resume](https://docs.google.com/viewer?url=https://github.com/D-Pow/resume/raw/master/Resume%20-%20Devon%20Powell.pdf)

## Build

Written in `.sublime-build` syntax for ease of use:

* Compile
    - `pdflatex "$file" && pdflatex "$file"`
* Remove intermediate files
    - `rm -f "${file_base_name}.log" "${file_base_name}.aux" "${file_base_name}.out" "${file_base_name}.bbl" "${file_base_name}.blg" "${file_base_name}.toc" "${file_base_name}.up*"`
* Opening after build
    - Linux: `xdg-open "${file_base_name}.pdf`
    - Windows: `start /B "" "${file_base_name}.pdf"`
    - Mac: `open "${file_base_name}.pdf`
