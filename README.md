Trumpia API
==========================
A simple Python wrapper for Trumpia's messaging API.

Features
--------

* An object oriented interface for Trumpia's API
* Will eventually support all of Trumpia's API calls


Installation
-------------
     pip install trumpia 
     
Usage
-----
```python
from trumpia import TrumpiaAPI
    
    
api = TrumpiaAPI(your_username, your_api_key)
campaign_lists = api.get_lists()
for i, trumpia_list in enumerate(campaign_lists):
    list_details = api.get_list_details(trumpia_list)
    # Print the list details as a dictionary
    print(list_details.__dict__)
```

License
-------

See LICENSE for details.
