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
        cls.hello()
        cls.sup_right_now()
        cls.things_i_like_to_do()

    @classmethod
    def hello(cls):
        print(f"Hey 👋, I'm {cls.first_name.capitalize()}.")

    @classmethod
    def sup_right_now(cls):
        print(f"Currently I'm doing {cls.work} in {cls.resides_in}.")

    @classmethod
    def things_i_like_to_do(cls):
        print("Some things I like to do:")
        print(*cls.enjoys, sep=",\n")

ItMe.intro()
```