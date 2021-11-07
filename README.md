```python
from earth import Human

class ItMe(Human):
    first_name: str = "ian"
    last_name: str = "whitestone"
    resides_in: str = "🇨🇦"
    enjoys: List[str] = ["🌯", "🏓", "💻", "🐍", "📊", "🏀", "☕️", "🍺", "🍷"]
    speaks: List[str] = ["en-CA", "🐍v3.7"]
    web: str = "https://ianwhitestone.work/"
    social: str = "@ianwhitestone"
    work_where: str = "shopify"
    work_what: str = "data"

    @classmethod
    def hi(cls):
        print(f"hey 👋, i'm {cls.first_name.capitalize()}")
        print(f"currently i work in {cls.work_what} @ {cls.work_where} in {cls.resides_in}")
        print(f"i speak {' and '.join(cls.speaks)}")
        print(f"some things i like: {', '.join(cls.enjoys)}")

>>> ItMe.hi()
hey 👋, i'm Ian
currently i work in data @ shopify in 🇨🇦
i speak en-CA and 🐍v3.7
some things i like: 🌯, 🏓, 💻, 🐍, 📊, 🏀, ☕️, 🍺, 🍷
```
