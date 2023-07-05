```python
from powerbiclient.authentication import DeviceCodeLoginAuthentication
from powerbiclient import Report, models
from io import StringIO
from ipywidgets import interact
import requests
import pandas as pd
import matplotlib
```


```python
from powerbiclient.authentication import InteractiveLoginAuthentication
interactive_auth = InteractiveLoginAuthentication()
```

    A local browser window will open for interactive sign in.
    
    Interactive authentication successfully completed.
    You are now logged in.
    
    The result should be passed only to trusted code in your notebook.
    


```python
auth = DeviceCodeLoginAuthentication()
```

    Performing device flow authentication. Please follow the instructions below.
    To sign in, use a web browser to open the page https://microsoft.com/devicelogin and enter the code EJ27JYKHV to authenticate.
    
    Device flow authentication successfully completed.
    You are now logged in .
    
    The result should be passed only to trusted code in your notebook.
    


```python
from IPython.display import IFrame

url = "https://app.powerbi.com/view?r=eyJrIjoiMzc5NmJlNGItNmE3ZC00ZTlmLWI0N2MtYzJmM2RmNzIxYWQ4IiwidCI6ImQ1N2QzMmNjLWMxMjEtNDg4Zi1iMDdiLWRmZTcwNTY4MGM3MSIsImMiOjN9"
iframe = IFrame(url, width="600", height="373.5")
display(iframe)

```



<iframe
    width="600"
    height="373.5"
    src="https://app.powerbi.com/view?r=eyJrIjoiMzc5NmJlNGItNmE3ZC00ZTlmLWI0N2MtYzJmM2RmNzIxYWQ4IiwidCI6ImQ1N2QzMmNjLWMxMjEtNDg4Zi1iMDdiLWRmZTcwNTY4MGM3MSIsImMiOjN9"
    frameborder="0"
    allowfullscreen

></iframe>




```python
from IPython.display import display, HTML

url = "https://app.powerbi.com/view?r=eyJrIjoiM2QzMTgxNDEtN2IwZS00M2RjLTlkODYtZjEwYTIxNzBmZTU5IiwidCI6ImQ1N2QzMmNjLWMxMjEtNDg4Zi1iMDdiLWRmZTcwNTY4MGM3MSIsImMiOjN9"

html_code = f'<div style="display: flex; justify-content: center;"><iframe title="General PowerBI Dashboard" src="{url}" width="600" height="373.5" frameborder="0" allowfullscreen="true"></iframe></div>'

display(HTML(html_code))

```


<div style="display: flex; justify-content: center;"><iframe title="General PowerBI Dashboard" src="https://app.powerbi.com/view?r=eyJrIjoiM2QzMTgxNDEtN2IwZS00M2RjLTlkODYtZjEwYTIxNzBmZTU5IiwidCI6ImQ1N2QzMmNjLWMxMjEtNDg4Zi1iMDdiLWRmZTcwNTY4MGM3MSIsImMiOjN9" width="600" height="373.5" frameborder="0" allowfullscreen="true"></iframe></div>



```python

```
