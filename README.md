# pub_mplstyle
A simple matplotlib style sheet with serif fonts and minor ticks.

![example plot](/examples/example.png)

## Usage
The style sheet can be called using the github URL or a local path.

```python
import matplotlib.style as style
style.use('https://raw.githubusercontent.com/ad3ller/pub_mplstyle/master/pub.mplstyle')
```

## Notes

The style sheet changes the default output to 150 dpi pdf with bbox='tight'.

The style sheet uses TrueType fonts.  To switch to tex fonts (slower),

```python
import matplotlib.pyplot as plt
plt.rcParams['text.usetex'] = True
```

Using ``` %matplotlib inline ```  in Jupyter apparently overrides font.size to 10.  Call the style sheet after setting inline. Or reset  manually

```python
plt.rcParams['font.size'] = 14
```

For further information on matplotlib style sheets see [http://matplotlib.org/users/style_sheets.html](http://matplotlib.org/users/style_sheets.html)
