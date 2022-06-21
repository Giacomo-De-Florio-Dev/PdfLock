
# Welcome to PDF Lock - by Giacomo-De-Florio-Dev
The script and its various versions contained in the repository provide a full support for protecting your PDF files with a password.

# System requirements
## Supported Operanting Systems
- Microsoft Windows
- Linux and Distros. 
- Mac Os X [Unstable].

## Required programs and libraries.
- Latest version of Python installed on your device.
- PyPDF2 (Python Lib).

# Usage
Download the latest release of PdfLock from [here](https://github.com/Giacomo-De-Florio-Dev/PdfLock/releases/latest), and unzip the archive.zip.
Then, put the `pdflock.py` file into your python project folder.
After that, you have to write in one of your scripts:

	import pdflock

Using `import pdflock` also perform some other functions such as checking the pypdf2 library and its installer if it is not available.

You can also directly import the function that crypt the PDFs:

	from pdflock import protect

Once you imported the pdflock library, to DIRECTLY lock a PDF use:

	pdflock.protect(YourPDFfilePath, YourPasswordToUnlockThePDF)

Using that format, the program will encrypt the PDF located in the path entered.
If you want to protect a copy of a PDF file, use:

	pdflock.protect(YourPDFfilePath, YourPasswordToUnlockThePDF, YourProtectedPDFDestination)

Using this format, the program will create a copy of your PDF file and encrypt it.

## Examples
example number 1:

	import pdflock

	pdf_path = input("insert your pdf file path here: ")
	pdf_password = input("insert a password to use to unlock yout pdf file: ")
	
	pdflock.protect(pdf_path, pdf_password)

example number 2:

	import pdflock

	pdf_path = input("insert your pdf file path here: ")
	pdf_password = input("insert a password to use to unlock yout pdf file: ")
	pdf_dext = input("insert here the destination path of your protected pdf file: ")

	pdflock.protect(pdf_path, pdf_password, pdf_dext)
	
## Credits
Program developed by [@Giacomo-De-Florio-Dev](https://github.com/giacomo-de-florio-dev/)

## [**DOWNLOAD HERE THE LATEST VERSION OF PDFLOCK**](https://github.com/Giacomo-De-Florio-Dev/PdfLock/releases/latest)
