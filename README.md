<div style="text-align: center;">

Portable Python
===============

</div>

<hr>

- A portable distribution of the Python programming language
		
- Provides a lightweight, self-contained Python environment that you can use from a usb , network share , folder.
 
- It includes all the most commonly used Python modules and allows you to run Python programs without needing to install Python globally or require admin privileges.


## 🛠️ Key Features

- **Easy to use** – Just unzip the archive and start coding with Python right away!

- **Pre-configured environment** – Most commonly used Python modules are already included. `requests` `beautifulsoup4` `psutil` `pillow` `...`

- **Pip support** – You can install additional Python modules as needed with pip.

- **No admin privileges required** – You can unzip and use the distribution anywhere.

Usage
------------

* Extract ppy.zip

powershell
```
Expand-Archive ppy.zip

portable-python\python.exe -c "print('Hello World')"
```
#### OR
```
Expand-Archive -Path ppy.zip -DestinationPath XYZ

XYZ\python.exe test.py
```

### python.ps1

```
iwr "https://github.com/portable-python/portable-python/ppy.zip" -o ppy.zip

Expand-Archive ppy.zip

cd ppy.zip

python.exe -c "print('Hello World')"

```




### Installing libraries

```
python.exe -m pip install <module>
```

### Importing libraries

```
import os,sys

try:
    import colorama
except:
    os.system(f"{sys.executable} -m pip install colorama")
    import colorama
```            
More informations
-----------------


* Development, bug reports and feature requests: https://github.com/portable-python/portable-python
