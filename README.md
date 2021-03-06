# oTree Documentation

[otree.readthedocs.io](http://otree.readthedocs.io/)

If you know Chinese, please help contribute a translation!

1.   Clone this repo
1.   `pip install -r requirements.txt`
1.   Go to locales/ and edit the .po files using [poedit](http://poedit.net) or simply using a text editor
1.   To preview your changes: `sphinx-build -b html -D language=zh_CN source build/html/zh_CN`
1.   Open the HTML files in your browser and check that they look OK
1.   Commit your changes to the .po files & make a pull request.

Then, your changes will be visible at:

[https://otree.readthedocs.io/zh_CN/latest/index.html](https://otree.readthedocs.io/zh_CN/latest/index.html)

To generate new .po files after an update to the English version, run:
		
```
sphinx-build -b gettext source build/gettext
sphinx-intl update -p build/gettext -l zh_CN
```