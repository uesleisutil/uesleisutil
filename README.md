<h2> Hey, I'm Ueslei. Welcome to my Github page!</h2>

<h5>
    
```python
​
import json
from dataclasses import asdict, dataclass

@dataclass
class Stack:
    languages   : tuple = ("Python", "Django", "Flask", "LaTeX", "Fortran", "NCL", "HTML", "CSS", "JavaScript", "NodeJS")
    misc        : tuple = ("Tensorflow")
    ongoing     : tuple = ("VueJS", "R", "Kubernetes", "Tensorflow")
    pronouns    : tuple = ("He", "Him")

    def serialize(self):
        return json.dumps(asdict(self), indent=4)

stack = Stack()
print(stack.serialize())
​
```

</h5>
