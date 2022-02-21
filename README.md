[![Hits](https://hits.sh/github.com/xncbf.svg?view=today-total)](https://hits.sh/github.com/xncbf/)
```python
from earth import Human

class ItMe(Human):
    first_name: str = "joon hwan"
    last_name: str = "kim"
    resides_in: str = "🇰🇷"
    enjoys: List[str] = ["🍔", "💻", "🐍", "🐶", "🐈", "☕️", "🍺", "🍷"]
    speaks: List[str] = ["ko-KR", "🐍v3.10"]
    web: str = "https://pypy.dev/"
    work_where: str = "FreeD Soft"
    work_what: str = "backend-engineer"

    @classmethod
    def hi(cls):
        print(f"hey 👋, i'm {cls.first_name.capitalize()}")
        print(f"currently i work in {cls.work_what} @ {cls.work_where} in {cls.resides_in}")
        print(f"i speak {' and '.join(cls.speaks)}")
        print(f"some things i like: {', '.join(cls.enjoys)}")

>>> ItMe.hi()
hey 👋, i'm Joon Hwan
currently i work in backend-engineer @ FreeD Soft in 🇰🇷
i speak ko-KR and 🐍v3.10
some things i like: 🍔, 💻, 🐍, 🐶, 🐈, ☕️, 🍺, 🍷
```
