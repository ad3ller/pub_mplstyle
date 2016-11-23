# pub_mplstyle
A simple matplotlib style sheet for creating plots to be published in two-column articles.

## Usage
The style sheet can be called using the github URL or a local path.

```python
import matplotlib.style as style
style.use('https://raw.githubusercontent.com/ad3ller/pub_mplstyle/master/pub.mplstyle')
```

## Notes

The style sheet changes the default output to 150 dpi pdf with bbox='tight'.

Using ``` %matplotlib inline ```  in Jupyter apparently overrides font.size.  To fix, simply run

```python
import matplotlib.pyplot as plt
plt.rcParams['font.size'] = 14
```

For further information on matplotlib style sheets see [http://matplotlib.org/users/style_sheets.html](http://matplotlib.org/users/style_sheets.html)
