| 🔢 | Method                | Description                              | Example                     | Output            |
| -- | --------------------- | ---------------------------------------- | --------------------------- | ----------------- |
| 1  | `str.upper()`         | Convert to uppercase                     | `"hi".upper()`              | `'HI'`            |
| 2  | `str.lower()`         | Convert to lowercase                     | `"Hi".lower()`              | `'hi'`            |
| 3  | `str.title()`         | Title case (capitalize each word)        | `"hello world".title()`     | `'Hello World'`   |
| 4  | `str.capitalize()`    | Capitalize first character only          | `"hello".capitalize()`      | `'Hello'`         |
| 5  | `str.strip()`         | Remove leading/trailing spaces           | `"  hi  ".strip()`          | `'hi'`            |
| 6  | `str.lstrip()`        | Remove leading spaces                    | `"  hi".lstrip()`           | `'hi'`            |
| 7  | `str.rstrip()`        | Remove trailing spaces                   | `"hi  ".rstrip()`           | `'hi'`            |
| 8  | `str.find(sub)`       | Find substring index                     | `"hello".find("e")`         | `1`               |
| 9  | `str.index(sub)`      | Like find(), but error if not found      | `"hello".index("e")`        | `1`               |
| 10 | `str.count(sub)`      | Count occurrences of substring           | `"banana".count("a")`       | `3`               |
| 11 | `str.replace(a, b)`   | Replace all `a` with `b`                 | `"a-b-c".replace("-", ":")` | `'a:b:c'`         |
| 12 | `str.split(sep)`      | Split string into list                   | `"a,b,c".split(",")`        | `['a', 'b', 'c']` |
| 13 | `str.join(list)`      | Join list into string                    | `".".join(["a","b"])`       | `'a.b'`           |
| 14 | `str.startswith(sub)` | Check if string starts with `sub`        | `"hello".startswith("he")`  | `True`            |
| 15 | `str.endswith(sub)`   | Check if string ends with `sub`          | `"hello".endswith("lo")`    | `True`            |
| 16 | `str.isdigit()`       | Check if all chars are digits            | `"123".isdigit()`           | `True`            |
| 17 | `str.isalpha()`       | Check if all chars are letters           | `"abc".isalpha()`           | `True`            |
| 18 | `str.isalnum()`       | Check if all chars are letters or digits | `"abc123".isalnum()`        | `True`            |
| 19 | `str.isspace()`       | Check if all chars are whitespace        | `"   ".isspace()`           | `True`            |
| 20 | `str.istitle()`       | Check if title case                      | `"Hello World".istitle()`   | `True`            |
| 21 | `str.isupper()`       | Check if all chars are uppercase         | `"HELLO".isupper()`         | `True`            |
| 22 | `str.islower()`       | Check if all chars are lowercase         | `"hello".islower()`         | `True`            |
| 23 | `str.zfill(n)`        | Pad with leading zeros to length `n`     | `"42".zfill(5)`             | `'00042'`         |
| 24 | `str.center(w)`       | Center string within width `w`           | `"hi".center(6, '-')`       | `'--hi--'`        |
| 25 | `str.ljust(w)`        | Left-justify within width `w`            | `"hi".ljust(6, '-')`        | `'hi----'`        |
| 26 | `str.rjust(w)`        | Right-justify within width `w`           | `"hi".rjust(6, '-')`        | `'----hi'`        |
| 27 | `str.swapcase()`      | Swap case                                | `"Hello".swapcase()`        | `'hELLO'`         |
| 28 | `str.encode()`        | Encode to bytes                          | `"hi".encode()`             | `b'hi'`           |
| 29 | `str.format()`        | Format string                            | `"Hi {}".format("Tim")`     | `'Hi Tim'`        |
| 30 | `f"{}"` (f-string)    | Modern formatting                        | `f"Hi {name}"`              | `'Hi Tim'`        |

---
## 🧾 list

| 🔢  | Method          | Description                      | Example              | Output           |
| --- | --------------- | -------------------------------- | -------------------- | ---------------- |
| 1️⃣ | `append(x)`     | ➕ Add item to end                | `lst.append(4)`      | `[1, 2, 3, 4]`   |
| 2️⃣ | `extend([...])` | 📌 Extend list with iterable     | `lst.extend([4,5])`  | `[1,2,3,4,5]`    |
| 3️⃣ | `insert(i, x)`  | 🧷 Insert item at index          | `lst.insert(1, 100)` | `[1, 100, 2, 3]` |
| 4️⃣ | `pop(i)`        | 🚪 Remove & return item at index | `lst.pop(1)`         | `2`              |
| 5️⃣ | `remove(x)`     | ❌ Remove first match             | `lst.remove(3)`      | `[1, 2, 4]`      |
| 6️⃣ | `clear()`       | 🧹 Remove all items              | `lst.clear()`        | `[]`             |
| 7️⃣ | `index(x)`      | 🔍 First index of value          | `lst.index(2)`       | `1`              |
| 8️⃣ | `count(x)`      | 🔢 Count occurrences             | `lst.count(3)`       | `1`              |
| 9️⃣ | `sort()`        | 🔼 In-place sort                 | `lst.sort()`         | `[1,2,3]`        |
| 🔟  | `reverse()`     | 🔁 Reverse order in-place        | `lst.reverse()`      | `[3,2,1]`        |
| 🔟  | `copy()`        | 📋 Shallow copy                  | `lst.copy()`         | `[1,2,3]`        |

---

## tuple

| 🔢  | Method        | Description               | Example      | Output  |
| --- | ------------- | ------------------------- | ------------ | ------- |
| 1️⃣ | `count(x)`    | 🔢 Count occurrences of x | `t.count(3)` | `1`     |
| 2️⃣ | `index(x)`    | 🔍 First index of x       | `t.index(2)` | `1`     |
| ⚠️  | *No mutation* | ✅ Tuples are immutable    | `t[0] = 10`  | ❌ Error |

---

## Set

| 🔢  | Method                   | Description                   | Example           | Output              |
| --- | ------------------------ | ----------------------------- | ----------------- | ------------------- |
| 1️⃣ | `add(x)`                 | ➕ Add element                 | `s.add(5)`        | `{1, 2, 3, 5}`      |
| 2️⃣ | `update([...])`          | 📌 Add multiple elements      | `s.update([6,7])` | `{1,2,3,6,7}`       |
| 3️⃣ | `remove(x)`              | ❌ Remove (error if not found) | `s.remove(3)`     | `{1,2}`             |
| 4️⃣ | `discard(x)`             | ❌ Safe remove (no error)      | `s.discard(10)`   | ✅ (no error)        |
| 5️⃣ | `pop()`                  | 🚪 Remove random element      | `s.pop()`         | Random item removed |
| 6️⃣ | `clear()`                | 🧹 Empty the set              | `s.clear()`       | `set()`             |
| 7️⃣ | `union()`                | ➕ Combine sets                | `s1.union(s2)`    | `s1 ∪ s2`           |
| 8️⃣ | `intersection()`         | 🔁 Common items               | `s1 & s2`         | `s1 ∩ s2`           |
| 9️⃣ | `difference()`           | ➖ Unique to first set         | `s1 - s2`         | `s1 \ s2`           |
| 🔟  | `symmetric_difference()` | 🔄 Non-common items           | `s1 ^ s2`         | `(A ∪ B) - (A ∩ B)` |

---

## Dict

| 🔢  | Method             | Description                         | Example                | Output               |
| --- | ------------------ | ----------------------------------- | ---------------------- | -------------------- |
| 1️⃣ | `get(k, default)`  | 🔍 Safe fetch                       | `d.get("a", 0)`        | `value or 0`         |
| 2️⃣ | `keys()`           | 🔑 All keys                         | `d.keys()`             | `dict_keys([...])`   |
| 3️⃣ | `values()`         | 📦 All values                       | `d.values()`           | `dict_values([...])` |
| 4️⃣ | `items()`          | 🧩 Key-value pairs                  | `d.items()`            | `dict_items([...])`  |
| 5️⃣ | `pop(k)`           | ❌ Remove key & return value         | `d.pop("a")`           | `value`              |
| 6️⃣ | `popitem()`        | 🧹 Remove last inserted item (3.7+) | `d.popitem()`          | `(key, value)`       |
| 7️⃣ | `update({...})`    | 🔁 Merge/update values              | `d.update({"a": 10})`  | updated `d`          |
| 8️⃣ | `setdefault(k, v)` | 🆕 Set value if key missing         | `d.setdefault("c", 3)` | `3`                  |
| 9️⃣ | `clear()`          | 🧼 Empty dictionary                 | `d.clear()`            | `{}`                 |
| 🔟  | `copy()`           | 📋 Shallow copy                     | `d.copy()`             | copy of `d`          |


---

## Summary

| Data Type | Mutable | Ordered | Allows Duplicates | Key Characteristics                   |
| --------- | ------- | ------- | ----------------- | ------------------------------------- |
| `list`    | ✅       | ✅       | ✅                 | Dynamic array, preserves order        |
| `tuple`   | ❌       | ✅       | ✅                 | Immutable, used for fixed collections |
| `set`     | ✅       | ❌       | ❌                 | Unique items, supports set math ops   |
| `dict`    | ✅       | ✅(3.7+) | ❌ (keys)          | Key-value pairs, fast lookup          |
