# Header 1

<h2> Header 2: Note: <font color = "red">html tags</font> <font color = "green">also work</font> in Markdown</h2>

###### Header 6

Note: Under is Horizontal Line
***
Note: Under is Horizontal Line
---
Note: Under is Horizontal Line
<hr>

<p>Html style paragraph.  This text is <strong>strong</strong> and <b>bold</b> while this text is <i>italic</i> this is <em>emphasized</em> and <del>strikethrough</del> and <mark>highlighted</mark> and <span style="background-color: green;">custom highlighted</span>.  Here is a Link to <a href="https://www.google.com" target="_blank" alt="Google Link">Google</a></p>

<center><img src ="https://www.google.com/images/logo.gif" alt="Google Image Here" title="Google Image"></center>

Markdown style paragraph.  This text is **strong** and __bold__ while this is _italic1_ or *italic2* and ~~strikethrough~~.  Here is a Link to [Google](https://www.google.com)

HTML Math x<sup>2</sup>y<sub>3</sub>

[Emojis](https://emojipedia.org/)✔️✅⭐❤️🧧💳

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
    <ul>
      <li>Granny</li>
      <li>Fuji</li>
    </ul>
  <li>Banana</li>
  <li>Carrot</li>
</ul>

Unordered List Markdown
* Apple
   * Granny
   * Fuji
- Banana
+ Carrot

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

|Table|Name|
|:---:|---:|
|0|Pokemons|
|1|Fruits|
|2|Vegetables|

HTML TaskList are inline
<form>
<input type="checkbox" id="trash" name="trash">
<label for="trash">Throw out Trash</label><br>
<input type="checkbox" id="dish" name="dish" checked>
<label for="dish">Clean Dishes</label>
</form>

## <font color = "yellow">Pre-Installation</font>

### Check current Git username and email
git config user.name
git config user.email

### Set globally (for all repos)(preferred)
git config --global user.name "Your Name"
git config --global user.email "your@email.com"

### Optional: Set for just this repo
git config user.name "Project Name"
git config user.email "project@email.com"

### Check if You Already Have SSH Keys
ls -la ~/.ssh

| <font color = "red">(private key)</font> | <font color = "red">id_rsa</font>  | <font color = "red">id_ed25519</font>  |
| --- | --- | --- |
| <font color = "green">(public key)</font> | <font color = "green">id_rsa.pub</font> | <font color = "green">id_ed25519.pub</font> |

### Pick: Generate SSH Key w/ ed25519 algorithm (more secure than RSA)
ssh-keygen -t ed25519 -C "your@email.com"

### Pick: Generate SSH Key w/ RSA algorithm
ssh-keygen -t rsa -b 4096 -C "your@email.com"

### Add SSH Key to GitHub/GitLab
cat ~/.ssh/id_ed25519.pub
cat ~/.ssh/id_rsa.pub

## <font color = "yellow">Installation</font>

1. Clone the repository
```bash
git clone git@github.com:trungdullc/00Markdown.git
```

2. Navigate to the project directory
```bash
cd 00Markdown/
```

3. Install dependencies
```bash
npm install
```

4. Create environment variable file
```bash
touch .env.local
```

5. Add the following environment variables to the .env.local file
```
FIREBASE_API_KEY=<your-firebase-api-key>
FIREBASE_AUTH_DOMAIN=<your-firebase-auth-domain>
FIREBASE_PROJECT_ID=<your-firebase-project-id>
FIREBASE_STORAGE_BUCKET=<your-firebase-storage-bucket>
FIREBASE_MESSAGING_SENDER_ID=<your-firebase-messaging-sender-id>
FIREBASE_APP_ID=<your-firebase-app-id>
FIREBASE_MEASUREMENT_ID=<your-firebase-measurement-id>
GOOGLE_MAPS_API_KEY=<your-google-maps-api-key>
IPGEOLOCATION_API_KEY=<your-ipgeolocation-api-key>
```

6. Deploy and set up Firebase Cloud Functions
```bash
cd functions
npm install
firebase deploy --only functions
```

7. Return to project root and start the development server
```bash
cd ..
npm run dev
```