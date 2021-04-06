### 🍻 Hey! Nice to see you!

<!-- Zero width character is used to put extra blank lines before and after code -->

<h1>
    
```python
​
import json
from dataclasses import asdict, dataclass


@dataclass
class Stack:
    languages   : tuple = ("Python", "JS", "Rust")
    databases   : tuple = ("PostgreSQL", "Mongo", "Redis")
    misc        : tuple = ("Docker", "ZMQ", "RabbitMQ")
    ongoing     : tuple = ("FastAPI", "Trio")

    def serialize(self):
        return json.dumps(asdict(self), indent=4)


stack = Stack()
print(stack.serialize())
​
```
</h1>
