# ASM-LaTex-Template
A LaTex Template for Submission to ASM journals to help authors meet our submission guidelines

# Readme for Template Generation

   
1. Unzip the archive to a working folder (say c:\asm)

The folder c:\asm will contain the following files:
	
	- asm-sample.tex (Sample LaTeX File Example)
	- asm.dtx (a bundle of LaTeX and BibTeX files to produce ASM papers)
	- asm.ins (This is file `asm.ins', the installation file for t `asm' distribution)
	- journals_logo_w_asm_logo_stacked.png (ASM Logo)

	Please also add graphics files if any illustrations used in your LaTeX Document file

2. Open Command Prompt and change to c:\asm folder:

       cd c:\asm

3. Run pdflatex on asm.ini file to generate ASM Class file:
       
    c:\asm>c:\texlive\2022\bin\win32\pdflatex.exe asm.ins

       We get the LaTeX class file and .bst file (Bibliography Style file):

       asmarticle.cls
       asm.bst

4. Run asm-sample file to generate Output PDF:

       c:\asm>c:\texlive\2022\bin\win32\pdflatex.exe asm-sample.tex


## Sample PDF Generation (default)


Without using any special option in preamble:

\documentclass{asmarticle} 

## Sample Draft PDF Generation


Use Draft option in preamble:

Example: \documentclass[draft]{asmarticle} 

## Sample Double-Anonymous PDF Generation


Use DoubleBlind option in preamble to subpress author information:

Example: \documentclass[DoubleBlind]{asmarticle}


