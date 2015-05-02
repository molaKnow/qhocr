The application qhocr is a free Hebrew OCR (optical character recognition) application based on the [hebocr c/c++](http://code.google.com/p/hebocr/) library originally written by Dr. by Kobi Zamir. The aim of this project is to develop a fully open-source and free OCR application, aimed for an end-user. The GUI is written in Nokia's Qt4. the application has been currently tested on win32 and Linux, but other platforms should be supported as well.


http://cucomania.dyndns.info/he/qhocr דף זה בעברית:

‫התוכנה qhocr היא תוכנה לזהוי תווים אופטים המבוססת על הספרייה [hebocr ](http://code.google.com/p/hebocr) במקור של ד"ר קובי זמיר. המטרה של הפרוייקט הזה היא לפתח תוכנת פתוחת־קוד וחופשית לזהוי תווים, המיועדת למשתמשי קצה. ממשק המשתמש כתוב ב־Qt4 של נוקיה. התוכנה נבדקה על חלונות ועל לינוקס, אבל תמיכה בפלטפורמות אחרות יתתווספו לפי הצורך.‬

‫הורדות מסודרות של התוכנה נמצאות באתר: http://code.google.com/p/qhocr/downloads/list . כדי להוריד את קוד המקור ולקבל את גרסאות הפיתוח האחרונות יש לעקוב אחרי ההוראות שיש באתר http://code.google.com/p/qhocr. ‬
לפרטים נוספים, אנא פנה אל דיאגו בכתובת
**diegoiast _at_ gmail.com**

![http://qhocr.googlecode.com/svn/tests/qhocr-0.10.16-svn.jpeg](http://qhocr.googlecode.com/svn/tests/qhocr-0.10.16-svn.jpeg)
‬
## Build on Windows ##
To build the application on windows:
  1. Download the Qt4 SDK from Nokia/QtSoftware - http://qt.nokia.com/downloads/sdk-windows-cpp
  1. Download TortoiseHG - http://tortoisehg.bitbucket.org/
  1. After a reboot, create a new directory "c:\source\qhocr" (you may choose another name, but it cannot contain spaces)
  1. Right click on the new qhocr directory, and choose the new item "TortoiseHg -> Clone.."
  1. Use this as the source path: https://qhocr.googlecode.com/hg/

## Build on Linux ##
You need to install the Qt4 development packages and Mercurial
```
# Fedroa, be sure that you have the Qt4 versions
yum install qt-devel
# Debian/Ubuntu
aptitude install libqt4-dev qt4-dev-tools
```

Then you need to checkout the source from Subversion, run qmake and make to compile the application:
```
hg clone https://qhocr.googlecode.com/hg/  qhocr
cd qhocr
# note this directory will have 2 *.pro files, one is for the CLI version, 
qmake qhocr.pro
make
ls -lh bin/qhocr

```

Please note that this procedure will create a nested Mercurial repository. The directory qhocr/src/hebocr actually points to https://hebocr.googlecode.com/hg

For more details, please contact Diego, at this email:
**diegoiast _at_ gmail.com**