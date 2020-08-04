```python
>>> from typing import List
>>> from earth import Human

>>> class ItMe(Human):

        first_name: str = "ian"
        last_name: str = "whitestone"
        resides_in: str = "🇨🇦"
        enjoys: List[str] = [
            "🌯", "🏓", "💻", "🐍", "🏀", "☕️", "🍺", "🍷"
        ]
        speaks: List[str] = ['en-CA', "🐍"]    
        web: str = "https://ianwhitestone.work/"
        social: str = "@ianwhitestone"    
        work_where: str = "shopify"
        work_what: str = "data"
    
        @classmethod
        def intro(cls):
            print(f"hey 👋, i'm {cls.first_name.capitalize()}")
            print(f"currently i'm doing {cls.work_what} @ {cls.work_where} in {cls.resides_in}")
            print(f"i speak {' and '.join(cls.speaks)}")
            print("some things i like:")
            print(*cls.enjoys, sep=",\n")

>>> ItMe.intro()

hey 👋, i'm Ian
currently i'm doing data @ shopify in 🇨🇦
i speak en-CA and 🐍
some things i like:
🌯,
🏓,
💻,
🐍,
🏀,
☕️,
🍺,
🍷
```