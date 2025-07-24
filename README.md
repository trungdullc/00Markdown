# Header 1

<h2> Header 2: Note: <font color = "red">html tags</font> <font color = "green">also work</font> in Markdown</h2>

###### Header 6

Note: Under is Horizontal Line
***
Note: Under is Horizontal Line
---
Note: Under is Horizontal Line
<hr>

<p>Html style paragraph.  This text is <strong>strong</strong> and <b>bold</b> while this text is <i>italic</i> this is <em>emphasized</em> and <del>strikethrough</del>.  Here is a Link to <a href="https://www.google.com" target="_blank" alt="Google Link">Google</a></p>

<center><img src ="https://www.google.com/images/logo.gif" alt="Google Image Here" title="Google Image"></center>

Markdown style paragraph.  This text is **strong** and __bold__ while this is _italic1_ or *italic2*.  Here is a Link to [Google](https://www.google.com)

<!-- 
Note: Putting Markdown inside html tag not work, becomes raw text
Note: Can't center Markdown, use html instead
<p align="center"></p>
<div style="text-align:center;"></div>
-->
![alt text](https://www.google.com/images/logo.gif "Google Image")

```python
class Solution:
    def output(self) -> None:
        print("Hi Hackers")

def main() -> None:
    sol: Solution = Solution()
    sol.output()

if __name__ == "__main__":
    main()
```

<pre><code>
#include <iostream>

int main() {
    std::cout << "Hello" << "\n";
    return 0;    
}
</code></pre>

<code>Inline Code</code>

<blockquote>BlockQuote HTML</blockquote><br>

> BlockQuote Markdown

Unordered List HTML
<ul>
  <li>Apple</li>
  <li>Banana</li>
</ul>

Unordered List Markdown
* Apple
- Banana

Ordered List HTML
<ol>
  <li>Apple 4</li>
  <li>Banana 3</li>
</ol>

Ordered List Markdown
1. Apple 4
2. Banana 3

<table style="border: 1px solid black; border-collapse: collapse; color: black; background-color: white;">
  <caption style="font-weight: bold; background-color: lightpink;">Fruit and Their Colors</caption>
  <tr>
    <th style="border: 2px solid black; background-color: white;">Fruit</th>
    <th style="border: 2px dotted red; background-color: green; color: white;">Color</th>
  </tr>
  <tr>
    <td style="border: 2px dashed blue; background-color: lightyellow;">Apple</td>
    <td style="border: 2px double purple; background-color: lavender;">Red</td>
  </tr>
  <tr>
    <td style="border: 2px groove orange; background-color: #f0f8ff;">Banana</td>
    <td style="border: 2px ridge teal; background-color: #e6ffe6;">Yellow</td>
  </tr>
  <tr>
    <td style="border: 2px inset gray; background-color: #fff0f5;">Grapes</td>
    <td style="border: 2px outset brown; background-color: #f5f5dc;">Purple</td>
  </tr>
</table>
