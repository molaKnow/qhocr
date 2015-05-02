# Introduction #

The code is handled using Mercurial. You you are running linux, you can install it with one of these commands:

```
# debian, ubuntu
aptitude install mercurial

# redhat, fedora
yum install 
```

If you are running Windows, please download TortoiseHG from here: http://mercurial.selenic.com/downloads/

You will also need Qt4:
  * Linux users can install it from their package managers,
  * Or download it from Nokia as windows users
  * Windows users need to download the qtsdk from here: http://qt.nokia.com/downloads/sdk-windows-cpp . The sdk comes with Qt4 (the libraries) QtCreator (an IDE) mingw (a compiler + debugger). And many other goodies.

The most important thing to remember here, is that this project is actually a mix of two: the GUI and the base library. The base library has it's own project - http://code.google.com/p/hebocr/ and this is the reason for the repositories nesting

# Download the code on Linux #

Execute these two commands
```
hg clone https://qhocr.googlecode.com/hg/  qhocr
hg clone https://hebocr.googlecode.com/hg/ qhocr/src/hebocr
```

**TODO** how to save credentials? I read the manuals, but still it does not work for me.

# Download the code on windows #

**Note**

> You need to create the first create a new repository clone on a directory without spaces. On windows XP, your home directory is not good (`c:\document and settings\use\my documents`) so you will need to create a new one. For example `c:\source`. Under Windows 7, your home directory does not contain spaces (`c:\users\user\documents`). For simplicity, the examples will use `c:\source\qhocr` as the directory to which the code will be downloaded to.

After you installed ToroiseHg, right click on a directory, and choose "Clone". In the source type `https://qhocr.googlecode.com/hg/`, and in the target type "c:\source\qhocr".

Then click again on a directory, and choose "TortoiseHg->Clone".  This time as the source type `https://hebocr.googlecode.com/hg/`  and target choose `c:\source\qhocr\src\hebocr`