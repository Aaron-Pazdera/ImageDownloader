# ImageDownloader
A simple python script that downloads all the URLs in a text file into a folder.

# Usage Examples:
 
**Linux example:**
```
mkdir ~/Downloads/DownloadedURLs

python ~/Downloads/ImageDownloader-master/DownloadImages.py ~/Downloads/URLs.txt ~/Downloads/DownloadedURLs
```
**Windows example:**
Windows stands out as the only modern operating system which does not actually come with a Python interpreter. Install one, then for the first argument of running the script, use the path to the python executable. The easiest way to do so is through the Windows 10 app store. If you do it that way, you can use just the `python` command, instead of a path to the python executable.
```
REM Make sure that teh 
mkdir C:\Users\%username%\Downloads\DownloadedURLs

REM The path to the python executable that you're using, or python for windows 10 app store version
REM Additionally, the default Windows .zip extractor creates an additional intermediate folder, whereas most others do not.
C:\python27\python.exe C:\Users\PazderaAaron\Downloads\ImageDownloader-master\ImageDownloader-master\DownloadImages.py C:\Users\%username%\Downloads\URLs.txt C:\Users\%username%\Downloads\DownloadedURLs
```



The URLs in the source file should be separated with a newline character.

If you leave the arguments blank, they should default to "URLs.txt" and your default Downloads folder (Should work on at least Windows and most all Linux distros, Mac is untested) respectively. But, if your file is not in fact named URLs.txt, and

If the name of a folder contains a space in it, you may have to escape that space with \\.
