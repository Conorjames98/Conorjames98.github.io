+++
date = '2025-01-05T21:23:30Z'
draft = false
title = 'Time formatting (Python)'
pin = true
+++

# formatting time in python

Here I simply learnt how to the ge the systems current time format it and display it using the libary 

-datetime-

```py
# import the datetime module
from datetime import datetime

# we assign datetime.now() to the variable current_time
current_time = datetime.now()

# we print the current time using the strftime() method
print("The current time is:", current_time.

# We use strftime to format time so it is human readable
strftime("%H:%M:%S"))
```

in the module datetime we use strftime which stands for (String Format Time) 


