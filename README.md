```python
from typing import List
from earth import Human

class ItMe(Human):

    first_name: str = "ian"
    last_name: str = "whitestone"
    resides_in: str = "🇨🇦"
    enjoys: List[str] = [
        "🌯", "🏓", "💻", "🐍", "🏀", "☕️",
    ]
    speaks: List[str] = ['en-CA', "🐍"]    
    web: str = "https://ianwhitestone.work/"
    social: str = "@ianwhitestone"    
    work: str = "data @ shopify"

    @classmethod
    def intro(cls):
        print(f"Hey 👋, I'm {cls.first_name.capitalize()}.")
        print(f"Currently I'm doing {cls.work} in {cls.resides_in}.")
        print("Some things I like to do:")
        print(*cls.enjoys, sep=",\n")

ItMe.intro()
```