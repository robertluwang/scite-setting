## Scite
Scite is most lightweight editor and portable by nature, it is my favorite quick note and code for long time, less than 3MB.

Here show you how to use scite as lightweight python IDE.

## scite + python dark theme
You can download from my [github](https://github.com/robertluwang/scite-setting) and quick replaces your scite theme. Please backup your SciTEGlobal.properties if you have some change on it.

```
git clone git@github.com:robertluwang/scite-setting.git
cd scite
cp SciTEGlobal.properties <scite path>/
```

## what changed to python.properties
scite already supports python, here just some small changes to make it more nice.
- string in red or pink, not comfortable for me so changed to #246161, you can pick up one from [HTML Color Picker](http://www.rapidtables.com/web/color/color-picker.htm)
- python path, you need to setup own portable path if it is not standard installation in windows
- append below setting to end of SciTEGlobal.properties or SciTEUser.properties

```
# Python

# Keyword
style.python.5=fore:#3060A0,bold

# String
style.python.3=fore:#246161,$(font.monospace)
# Single quoted string
style.python.4=fore:#246161,$(font.monospace)

# Triple quotes
style.python.6=fore:#246161
# Triple double quotes
style.python.7=fore:#246161

# python path sample, change to your own python path and uncomment below lines; otherwise assume it is standard installation on Windons
#command.go.*.py=C:\oldhorse\portableapps\python\PortablePython2.7.5.1\App\pythonw -u "$(FileNameExt)"
#command.go.*.pyw=C:\oldhorse\portableapps\python\PortablePython2.7.5.1\App\pythonw -u "$(FileNameExt)"
#command.1.$(file.patterns.py)=C:\oldhorse\portableapps\python\PortablePython2.7.5.1\App\python -c "import py_compile; py_compile.compile(r'$(FilePath)')"

```
