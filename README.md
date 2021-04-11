# Windows Desktop Notification In Python

This Post will give you a very easy way to create desktop notifications in Windows using Python.

To install the dependency , Use the code below
```python
python -m pip install win10toast
```
Now use the code below to make a notification alert.

```python
from win10toast import ToastNotifier
# One-time initialization
toaster = ToastNotifier()

# Show notification whenever needed
toaster.show_toast("Notification! From Tech CVR", "Alert!", threaded=True, icon_path=None, duration=5)

import time
while toaster.notification_active():
    time.sleep(0.1)
```
Enjoy : )
