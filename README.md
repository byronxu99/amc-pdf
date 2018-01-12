# amc-pdf
ugly script, nice PDFs

## About
**amc-pdf** is a bash shell script that I wrote several years ago. Its purpose is to generate nice-looking PDF files of past exams in the AMC series of mathematics contests, including the AMC 8, AMC 10, AMC 12, AIME, and USA(J)MO. The script downloads data from the Art of Problem Solving Wiki and uses LaTeX to create a problems PDF and an answer key/solutions PDF.

Sample output:

<img src="https://i.imgur.com/k03j08K.png" width="400" align="middle"><img src="https://i.imgur.com/ADQfY5y.png" width="400" align="middle">

## Usage
The script's dependecies are
* bash
* curl
* A LaTeX distribution
* Asymptote
* latexmk

and optionally, these Asymptote packages (the script will have to download them each time if they are missing)
* [olympiad.asy](https://math.berkeley.edu/~monks/images/olympiad.asy)
* [cse5.asy](https://raw.githubusercontent.com/vEnhance/dotfiles/master/asy/cse5.asy)

Running **amc-pdf** is simple -- Just call with the year and the test type.
* `./amc-pdf 2008 amc 8`
* `./amc-pdf 2013 amc 10a`
* `./amc-pdf 2016 amc 12b`
* `./amc-pdf 2011 aime i`
* `./amc-pdf 2010 usamo`


