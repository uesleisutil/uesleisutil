<h5>
    
```python
​
import json
from dataclasses import asdict, dataclass

@dataclass
class Stack:
    languages   : tuple = ("Python", "Django", "Flask", "LaTeX", "Fortran", "SQL", "NCL", "HTML", "CSS", "JS")
    misc        : tuple = ("Tensorflow")
    ongoing     : tuple = ("R", "ECL")
    pronouns    : tuple = ("He", "Him")

    def serialize(self):
        return json.dumps(asdict(self), indent=4)

stack = Stack()
print(stack.serialize())
​
```

</h5>
