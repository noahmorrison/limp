# limp
Lazy imports in python

Just add ```import limp``` to the top of your imports and they'll only be imported when you use the module
```python
#!/usr/bin/python

import limp  # Lazy imports begin now

import json
import sys

print('json' in sys.modules)  # False
print(', '.join(json.loads('["Hello", "World!"]')))
print('json' in sys.modules)  # True
```
