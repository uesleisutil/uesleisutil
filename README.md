<h5>
    
```python
​
import json
from dataclasses import asdict, dataclass

@dataclass
class Stack:
    languages   : tuple = ("Python", "LaTeX", "Fortran", "SQL", "NCL")
    pronouns    : tuple = ("He", "Him")

    def serialize(self):
        return json.dumps(asdict(self), indent=4)

stack = Stack()
print(stack.serialize())
​
```

</h5>
