# pdflock - Password protect PDF files

Given an input PDF file, output a password protected version.

## Running

Running this is as simple as:

    python3 pdflock.py input.pdf output.pdf
  
To set the password non-interactively, run: 

    pdflock.py input.pdf output.pdf --password="my secret"

## Generating Commands from a Spreadsheet

You can generate commands via a spreadsheet to easily batch password protect PDF documents with different passwords. Assuming that the columns A-C correspond to `Password`, `Input File` and `Output File`. Simply, use the following formula on row 2:

    ="python3 pdflock.py " &  B2 & " " & C2 & " --password="""& A2 &""""

## Installation and Dependencies

This program requires `python3` and the `pyPdf2` module to be installed. 

On a Mac, you can install this with:

    brew install python@3
    pip3 install pyPdf2

## Licensing
It is released under the GNU GPL version 2 license
