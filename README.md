# Extended Word Count

**Options**
  * w - counts the words
  * W - gets word usage
  * c - counts all chars (no whitespaces)
  * C - get char usage
  * b - counts all bytes (with whitespaces)
  * f - sets file to load (or dir to start if '--graphical')
  * E - set filename for exported json file (see JSON)
  
  (string flags (--))
  * hell      - graphical tkinter dialog (no specification of options)
  * graphical - ANSI Graphic selection   (no specification of options)
  * words - same as 'w'
  * chars - same as 'c'

**JSON**
  * Format:
    * words      - number of words
    * chars      - number of chars
    * kbd\_hits   - number of keyboard hits
    * stat\_bytes - dict of statistics of bytes
    * stat\_words - dict of statistics of words
    * avg\_word\_len - average word length

  * How to load:
    ```python3
    import json
    
    f = open("example.json", 'r')
    data = json.load(f)
    f.close()

    print(data["words"])
    ```
