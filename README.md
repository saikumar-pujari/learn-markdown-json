# learn-markdown-json

* **important**:about json its below the markdown on line 156

>## markdown
## Headings

Use `#` for headings. More `#` means a smaller heading:

```markdown
# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5
```

## Paragraphs

Just write your text as normal.  
A line break is made by ending a line with two spaces.

Example:

This is a paragraph.  
This is another line in the same paragraph.

## Emphasis

- *Italic*: `*text*` → *text*
- **Bold**: `**text**` → **text**
- ***Bold & Italic***: `***text***` → ***text***
- ~~Strikethrough~~: `~~text~~` → ~~text~~

> Note: Highlighting with `==text==` is not standard in Markdown.

## Code

Inline code: `` `code` `` → `code`

Code block:

<pre>
```cpp
#include &lt;iostream&gt;
int main() {}
```
</pre>

## Links & Images

- [Link text](https://example.com): `[Link text](https://example.com)`
- Image: `![alt text](image_url)`

Example:  
[saikumar](saikumar.me)  
![image]()

## Blockquotes

Use `>` for blockquotes:

```markdown
> This is a quote
>> Nested quote
>>> More nested
```

## Horizontal Line

Use `---` for a horizontal rule:

---

## Lists

**Ordered list:**

```markdown
1. First item
    2. Subitem
2. Second item
3. Third item
```

**Unordered list:**

```markdown
- Item
    - Subitem
* Item
+ Item
```

## Task Lists/checkbox

```markdown
- [ ] Task not done
- [x] Task done
```

- [ ] Task not done
- [x] Task done

## Tables

Basic table:

```markdown
| Column 1 | Column 2 |
|----------|----------|
| Row 1    | Data 1   |
| Row 2    | Data 2   |
```

| Column 1 | Column 2 |
|----------|----------|
| Row 1    | Data 1   |
| Row 2    | Data 2   |

**Center align:**

```markdown
| Column 1 | Column 2 |
|:--------:|:--------:|
|  Row 1   |  Data 1  |
|  Row 2   |  Data 2  |
```

| Column 1 | Column 2 |
|:--------:|:--------:|
|  Row 1   |  Data 1  |
|  Row 2   |  Data 2  |

**Align left/right:**

```markdown
| Column 1 | Column 2 |
|-------:|:--------|
| right  | left    |
| Row 2  | Data 2  |
```

| Column 1 | Column 2 |
|-------:|:--------|
| right  | left    |
| Row 2  | Data 2  |

---
here ends the markdown  
This guide covers the basics of Markdown formatting for easy reference!

---


> ## JSON (JavaScript Object Notation)

JSON is a lightweight data format used for storing and exchanging data. It's easy for humans to read and write, and easy for machines to parse and generate.

### Basic Structure

A JSON object is made up of key-value pairs, surrounded by curly braces `{}`. Keys are strings, and values can be strings, numbers, arrays, objects, `true`, `false`, or `null`.

Example:

```json
{
    "name": "Alice",
    "age": 25,
    "isStudent": false,
    "skills": ["Python", "JavaScript"],
    "address": {
        "city": "Wonderland",
        "zip": "12345"
    }
}
```

### Rules

- Keys and string values must be in double quotes `"`.
- Data is separated by commas.
- Arrays use square brackets `[]`.
- No comments allowed in JSON.

### Using JSON in JavaScript

Parse JSON string to object:

```js
const jsonString = '{"name":"Alice","age":25}';
const obj = JSON.parse(jsonString);
console.log(obj.name); // Alice
```

Convert object to JSON string:

```js
const obj = { name: "Alice", age: 25 };
const jsonString = JSON.stringify(obj);
console.log(jsonString); // {"name":"Alice","age":25}
```

### Using JSON in Python

Parse JSON string to dictionary:

```python
import json

json_string = '{"name": "Alice", "age": 25}'
data = json.loads(json_string)
print(data["name"])  # Alice
```

Convert dictionary to JSON string:

```python
import json

data = { "name": "Alice", "age": 25 }
json_string = json.dumps(data)
print(json_string)  # {"name": "Alice", "age": 25}
```

---

JSON is widely used for APIs, configuration files, and data exchange between applications.
