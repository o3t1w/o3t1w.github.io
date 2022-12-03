
# ➕ Add your resources to [O3T1W's OSINT Tools Map](https://o3t1w.github.io/tree/)

- **Go in `/database.json`**
- **Edit the file** then **save it**.
  - _If you want your project to be merged, follow the rules and tutorial following this part._

## 🖌 Syntax
1. Resources names:
    - For the legend, specify **one** or **many emoji(s) from [this legend](https://github.com/o3t1w/o3t1w.github.io/tree/main/tree#-legend)**. _If there are many emojis, do not add space between them._
    - Add a space.
    - Add the name of your resource. It can contain spaces.
2. Branch names:
    - You can put spaces in it, but **no emoji at the start** of the string.
## 🛠 Tutorial:
If you don't understand how the JSON file works, the following lines are for you !
### 📂 To add a new branch:
Let's say I want to open in the `Usernames` branch a new one called `Alpha`, containing itself an empty branch `Beta`.
```python
# Before
{
    "OSINT Map": {
        "Usernames": {
            "📦 maigret": "https://github.com/soxoj/maigret"
        }
    }
}

# After
{
    "OSINT Map": {
        "Usernames": {
            "📦 maigret": "https://github.com/soxoj/maigret",
            "Alpha": {
                "Beta": {}
            }
        }
    }
}
```
### ♟ To add a new tool
Now, let's say I want to add a tool to my brand new branch `Beta`:
```python
# Before
{
    "OSINT Map": {
        "Usernames": {
            "📦 maigret": "https://github.com/soxoj/maigret",
            "Alpha": {
                "Beta": {}
            }
        }
    }
}

# After
{
    "OSINT Map": {
        "Usernames": {
            "📦 maigret": "https://github.com/soxoj/maigret",
            "Alpha": {
                "Beta": {
                    "<CATEGORY EMOJI (check the rules)> <CATEGORY NAME>": "url://to.my.awesome/tool"
                }
            }
        }
    }
}
```
