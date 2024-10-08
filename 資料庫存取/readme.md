# sqlite 3 介紹 
# Python版本已經預裝了 sqlite3 模組 
# python存取 sqlite3 的套件安裝 ==> !pip install pysqlite3
# 
- [sqlite3 — DB-API 2.0 interface for SQLite databases](https://docs.python.org/3/library/sqlite3.html)
- https://shengyu7697.github.io/python-sqlite/
```python
import sqlite3
con = sqlite3.connect("tutorial.db")

cur = con.cursor()

cur.execute("CREATE TABLE movie(title, year, score)")


```
