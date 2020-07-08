# pdflock - Password protect PDF files

Given an input PDF file, output a password protected version.

## Running

Running this is as simple as:

    $ python3 pdflock.py input.pdf output.pdf
  
To set the password non-interactively, run: 

    $ pdflock.py input.pdf output.pdf --password="my secret"
 

## Installation and Dependencies
This program requires `python3` and the `pyPdf2` module to be installed. 

On a Mac, you can install this with `brew install python@3; pip3 install pyPdf2`

## Licensing
It is released under the GNU GPL version 2 license