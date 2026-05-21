# Common Markdown Syntax
This document gathers all the Markdown syntax that are supported by both GitHub and GitLab. This is very useful for creating documentation for those platforms simultaneously.

Only the Markdown syntax that are common between the documentations below are highlighted here.
- GitHub
  - [GitHub Docs - Basic Writing and Formatting Syntax](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).
  - [GitHub Docs - Working with Advanced Formatting](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting).
  - [GitHub Flavored Markdown Spec](https://github.github.com/gfm/).
- GitLab
  - [GitLab Flavored Markdown](https://docs.gitlab.com/user/markdown/).
  - [GitLab Syntax Rendered](https://gitlab.com/gitlab-org/gitlab/-/blob/master/doc/user/markdown.md).

This is meant for personal use to ease writing documentation on both GitHub and GitLab for the same project/repository.

I might add other platforms here, but I don't plan to seriously maintain any of this. However, feel free to fork and create your documentation from this.

---

## Headings
> <ins>**Syntax**</ins>  
> ```
> # Heading 1
> ## Heading 2
> ### Heading 3
> #### Heading 4
> ##### Heading 5
> ###### Heading 6
> ```

> <ins>**Output**</ins>  
> # Heading 1
> ## Heading 2
> ### Heading 3
> #### Heading 4
> ##### Heading 5
> ###### Heading 6

---

## Line Breaks

### Paragraphs
> <ins>**Syntax**</ins>  
> ```
> This is the first paragraph.
> This will not be counted as a new line.
> 
> However, an empty line will create a paragraph. So, this is the second paragraph.
> ```

> <ins>**Output**</ins>  
> This is the first paragraph.
> This will not be counted as a new line.
> 
> However, an empty line will create a paragraph. So, this is the second paragraph.

### New Line
> <ins>**Sytnax**</ins>  
> ```
> This is line 1.
> But this won't be next line.\
> This, however, is the line 2, because of the backslash (`\`) in previous line.  
> And this is also in next line, because of double-space (`  `).
> ```

> <ins>**Output**</ins>  
> This is line 1.
> But this won't be next line.\
> This, however, is the line 2, because of the backslash (`\`) in previous line.  
> And this is also in next line, because of double-space (`  `).

---

## Emphasis / Styling
|Style                 |Syntax            |Example                                 |Output                                |
|----------------------|------------------|----------------------------------------|--------------------------------------|
|Bold                  |`** **` or `__ __`|`**This is bold text**`                 |**This is bold text**                 |
|Italic                |`* *` or `_ _`    |`_This text is italicized_`             |_This text is italicized_             |
|Strikethrough         |`~~ ~~` or `~ ~`  |`~~This was mistaken text~~`            |~~This was mistaken text~~            |
|Bold and nested italic|`** **` and `_ _` |`**This text is _extremely_ important**`|**This text is _extremely_ important**|
|All bold and italic   |`*** ***`         |`***All this text is important***`      |_**All this text is important**_      |
|Subscript             |`<sub> </sub>`    |`This is a <sub>subscript</sub> text`   |This is a <sub>subscript</sub> text   |
|Superscript           |`<sup> </sup>`    |`This is a <sup>superscript</sup> text` |This is a <sup>superscript</sup> text |
|Underline             |`<ins> </ins>`    |`This is an <ins>underlined</ins> text` |This is an <ins>underlined</ins> text |

---

## Horizontal Line
> [!NOTE]
> - GitHub automatically adds a horizontal line when rendering headings, but it doesn't modify the text.
> - Horizontal lines turn the respective lines above into a Heading. See the renderings in **Output** section below.

> <ins>**Syntax**</ins>  
> ```
> Option 1: using Hyphens (-)
> ---
> 
> Option 2: using Asterisks (*)
> ***
> 
> Option 3: using Underscores (_)
> ___
> ```

> <ins>**Output**</ins>  
> 
> Option 1: using Hyphens (-)
> ---
> 
> Option 2: using Asterisks (*)
> ***
> 
> Option 3: using Underscores (_)
> ___

---

## Lists
### Unordered Lists
> <ins>**Syntax**</ins>  
> ```
> - Option 1: using Hyphen / Minus (-)
>   - Sub-item with indentation.
>     - Nesting with more indentation.
> + Option 2: using Plus (+)
>   + Sub-item with indentation.
>     + More indentation.
> * Option 3: using Asterisk (*)
>   * Sub-item with indentation.
>     * More indentation.
> ```

> <ins>**Output**</ins>  
> - Option 1: using Hyphen / Minus (-)
>   - Sub-item with indentation.
>     - Nesting with more indentation.
> + Option 2: using Plus (+)
>   + Sub-item with indentation.
>     + More indentation.
> * Option 3: using Asterisk (*)
>   * Sub-item with indentation.
>     * More indentation.

### Ordered Lists
> <ins>**Syntax**</ins>  
> ```
> 1. Type "1." and a Space to create first item.
> 2. Continue the numbering to add more items.
>    1. Indent to create sub-item.
>       1. Nesting is also supported.
> ```

> <ins>**Output**</ins>  
> 1. Type "1." and a Space to create first item.
> 2. Continue the numbering to add more items.
>    1. Indent to create sub-item.
>       1. Nesting is also supported.

### Mixing List Types
> <ins>**Syntax**</ins>  
> ```
> 1. Unordered List
>    - Item 1
>      1. Ordered sub-list.
>      2. Continuing the order.
> 
> - Ordered List
>   1. Starting here.
>   2. Continuing.
>      - No order in sub-items.
>      - No order here too!
> ```

> <ins>**Output**</ins>  
> 1. Unordered List
>    - Item 1
>      1. Ordered sub-list.
>      2. Continuing the order.
> 
> - Ordered List
>   1. Starting here.
>   2. Continuing.
>      - No order in sub-items.
>      - No order here too!

---

## Task Lists
> <ins>**Syntax**</ins>  
> ```
> - [ ] Unchecked item.
> - [x] Checked item.
>   - [ ] Sub-tasks with indentation.
> ```

> <ins>**Output**</ins>  
> - [ ] Unchecked item.
> - [x] Checked item.
>   - [ ] Sub-tasks with indentation.

---

## Links
> <ins>**Syntax**</ins>  
> ```
> - Inline-style link: [Example Domain](https://example.com/)
> - File in _same directory_: [Example Text File](example.txt)
> - Relative link: [File inside a sub-directory](ExampleDirectory/Example2.txt)
> - Link to a Section: [This goes to the top Heading](#common-markdown-syntax)
> - Link to Section in another Markdown file: [Example.md Link](example.md#example-heading-1)
> - URL Auto-linking:
>   - https://www.google.com
>   - ftp://ftp.us.debian.org/debian/
>   - smb://foo/bar/baz
>   - irc://irc.freenode.net/
>   - http://localhost:3000
> ```

> <ins>**Output**</ins>  
> - Inline-style link: [Example Domain](https://example.com/)
> - File in _same directory_: [Example Text File](example.txt)
> - Relative link: [File inside a sub-directory](ExampleDirectory/Example2.txt)
> - Link to a Section: [This goes to the top Heading](#common-markdown-syntax)
> - Link to Section in another Markdown file: [Example.md Link](example.md#example-heading-1)
> - URL Auto-linking (some might not work in GitHub):
>   - https://www.google.com
>   - ftp://ftp.us.debian.org/debian/
>   - smb://foo/bar/baz
>   - irc://irc.freenode.net/
>   - http://localhost:3000

---

## Quote Blocks
> <ins>**Syntax**</ins>  
> ```
> > This is a Block Quote.  
> > This is another line in the Block Quote.  
> > This is how the "Syntax" and "Output" sections are written here.  
> > > They can also be nested like this.
> ```

> <ins>**Output**</ins>  
> > This is a Block Quote.  
> > This is another line in the Block Quote.  
> > This is how the "Syntax" and "Output" sections are written here.  
> > > They can also be nested like this.

---

## Alert Blocks
> <ins>**Syntax**</ins>  
> ```
> > [!NOTE]  
> > Highlights information that users should take into account, even when skimming.
> 
> > [!TIP]  
> > Optional information to help a user be more successful.
> 
> > [!IMPORTANT]  
> > Crucial information necessary for users to succeed.
> 
> > [!WARNING]  
> > Critical content demanding immediate user attention due to potential risks.
> 
> > [!CAUTION]  
> > Negative potential consequences of an action.
> ```

> <ins>**Output**</ins>  

> [!NOTE]  
> Highlights information that users should take into account, even when skimming.

> [!TIP]  
> Optional information to help a user be more successful.

> [!IMPORTANT]  
> Crucial information necessary for users to succeed.

> [!WARNING]  
> Critical content demanding immediate user attention due to potential risks.

> [!CAUTION]  
> Negative potential consequences of an action.

> [!NOTE]  
> <ins>**Nesting and Indentation**</ins>
> 
> GitLab Flavored Markdown supports nesting and indentation alignment of the Alert Blocks, but GitHub Flavored Markdown doesn't support it.
> 
> The block below will be rendered as intended in GitLab, but _not in GitHub_.
> > <ins>**Syntax**</ins>  
> > ```
> > - This is a Note block
> > 	> [!NOTE]
> > 	> Highlights information that users should take into account, even when skimming.
> > - This is a Tip block
> > 	> [!TIP]
> > 	> Optional information to help a user be more successful.
> > - This is an Important block
> > 	> [!IMPORTANT]
> > 	> Crucial information necessary for users to succeed.
> > - This is a Warning block
> > 	> [!WARNING]
> > 	> Critical content demanding immediate user attention due to potential risks.
> > - This is a Caution block
> > 	> [!CAUTION]
> > 	> Negative potential consequences of an action.
> > ```
> 
> > <ins>**Output**</ins>  
> > - This is a Note block
> > 	> [!NOTE]
> > 	> Highlights information that users should take into account, even when skimming.
> > - This is a Tip block
> > 	> [!TIP]
> > 	> Optional information to help a user be more successful.
> > - This is an Important block
> > 	> [!IMPORTANT]
> > 	> Crucial information necessary for users to succeed.
> > - This is a Warning block
> > 	> [!WARNING]
> > 	> Critical content demanding immediate user attention due to potential risks.
> > - This is a Caution block
> > 	> [!CAUTION]
> > 	> Negative potential consequences of an action.

---

## Code Blocks
### Basic Code Block  
> <ins>**Syntax**</ins>  
> ````
> ```
> checkEvenOdd(number){
> 	if number is divisble by 2,
> 		return "Even"
> 	else, return "Odd"
> }
> ```
> ````

> <ins>**Output**</ins>  
> ```
> checkEvenOdd(number){
> 	if number is divisble by 2,
> 		return "Even"
> 	else, return "Odd"
> }
> ```

### Syntax Highlighting
> [!NOTE]  
> - [**GitHub's supported languages and keywords**](https://github.com/github-linguist/linguist/blob/main/lib/linguist/languages.yml) ("`name`" and "`aliases`" fields in the YAML file). GitHub uses [Linguist](https://github.com/github-linguist/linguist).
> - [**GitLab's supported languages and keywords**](https://github.com/rouge-ruby/rouge/wiki/List-of-supported-languages-and-lexers). GitLab uses [Rogue Ruby library](https://github.com/rouge-ruby/rouge).

> <ins>**Syntax**</ins>  
> Written in _Bash_  
> ````
> ```bash
> checkEvenOdd() {
> 	local number=$1
> 	
> 	if (( number % 2 == 0 )); then
> 		printf "Even"
> 	else
> 		printf "Odd"
> 	fi
> }
> ```
> ````
>   
> Written in _Markdown_  
> ````
> ```md
> ## This is a Markdown Syntax
> 1. All Markdown syntax are _highlighted_ here.
> - But, they're **not rendered**
> ```
> ````
>   
> Written in _XML_  
> ````
> ```xml
> <?xml version="1.0" encoding="UTF-8"?>
> <library>
>     <book id="b1">
>         <title>The Adventures of Sherlock Holmes</title>
>         <author>Arthur Conan Doyle</author>
>         <year>1892</year>
>     </book>
> 
>     <book id="b2">
>         <title>Pride and Prejudice</title>
>         <author>Jane Austen</author>
>         <year>1813</year>
>     </book>
> </library>
> ```
> ````

> <ins>**Output**</ins>  
> Written in _Bash_  
> ```bash
> checkEvenOdd() {
> 	local number=$1
> 	
> 	if (( number % 2 == 0 )); then
> 		printf "Even"
> 	else
> 		printf "Odd"
> 	fi
> }
> ```
>   
> Written in _Markdown_  
> ```md
> ## This is a Markdown Syntax
> 1. All Markdown syntax are _highlighted_ here.
> - But, they're **not rendered**
> ```
>   
> Written in _XML_  
> ```xml
> <?xml version="1.0" encoding="UTF-8"?>
> <library>
>     <book id="b1">
>         <title>The Adventures of Sherlock Holmes</title>
>         <author>Arthur Conan Doyle</author>
>         <year>1892</year>
>     </book>
> 
>     <book id="b2">
>         <title>Pride and Prejudice</title>
>         <author>Jane Austen</author>
>         <year>1813</year>
>     </book>
> </library>
> ```

### Backtick Fencing  
- Minimum _3 backticks_ are required for a **code block**, _less_ will render as **inline code**.
- Number of backticks **ending a section** <ins>_must match_</ins> the number of backticks **starting i**.
- Closest pair of matching backticks are considered a block. Meaning that a line of `N` backticks will create a block with the latest line before it that has `N` backticks.
- Sections created with different number of backticks can be nested. A block marked with _3 backticks_ can be nested inside a block marked with _4 backticks_.

The rules above are used to to write this entire [Code Blocks](#code-blocks) section.  

> <ins>**Syntax**</ins>
> - Using **2 backticks**.  
> 	```
> 	``
> 	Line 1
> 	`Line 2`
> 	``
> 	```
> - Using nested backtick blocks.  
> 	`````
> 	````yaml
> 	name: Test YAML
> 	  vars:
> 	    foo: 1
> 	    bar: hello
> 	    baz:
> 	      - item1
> 	      - item2
> 	```sh
> 	echo "Hello, World!"
> 	```
> 	````
> 	`````

> <ins>**Output**</ins>
> - Using **2 backticks**.  
> 	``
> 	Line 1
> 	`Line 2`
> 	``
> - Using nested backtick blocks.  
> 	````yaml
> 	name: Test YAML
> 	  vars:
> 	    foo: 1
> 	    bar: hello
> 	    baz:
> 	      - item1
> 	      - item2
> 	```sh
> 	echo "Hello, World!"
> 	```
> 	````

---

## Tables
> <ins>**Syntax**</ins>
> - Bare minimum syntax. Table renders as expected.
> 	```
> 	|Left aligned|Centre aligned|Right aligned|
> 	|:---|:------:|--------:|
> 	|cell 1|Writing '\|' and '\-' using escape character `\`|cell 3|
> 	|cell 4|cell 5 is longer|cell 6 is much longer than the others, but that's ok. It eventually wraps the text when the cell is too large for the display size.|
> 	|cell 7|This item has:<br>- Multiple items<br>- That we want listed separately.|cell 9|
> 	```
> 
> - Cleaner plain-text for visual clarity. Table rendering unaffected.
> 	```
> 	| Left aligned     | Centre aligned                                                          | Right aligned                                                                                                                       |
> 	| :--------------- | :---------------------------------------------------------------------: | ----------------------------------------------------------------------------------------------------------------------------------: |
> 	| cell 1           | Writing '\|' and '\-' using escape character `\`                        | cell 3                                                                                                                              |
> 	| cell 4 is longer.| cell 5                                                                  | cell 6 is much longer than the others, but that's ok. It eventually wraps the text when the cell is too large for the display size. |
> 	| cell 7           | This item has:<br>- Multiple items<br>- That we want listed separately. | cell 9                                                                                                                              |
> 	```

> <ins>**Syntax**</ins>
> - Bare minimum syntax. Table renders as expected.
> 	|Left aligned|Centre aligned|Right aligned|
> 	|:---|:------:|--------:|
> 	|cell 1|Writing '\|' and '\-' using escape character `\`|cell 3|
> 	|cell 4|cell 5 is longer|cell 6 is much longer than the others, but that's ok. It eventually wraps the text when the cell is too large for the display size.|
> 	|cell 7|This item has:<br>- Multiple items<br>- That we want listed separately.|cell 9|
> 
> - Cleaner plain-text for visual clarity. Table rendering unaffected.
> 	| Left aligned     | Centre aligned                                                          | Right aligned                                                                                                                       |
> 	| :--------------- | :---------------------------------------------------------------------: | ----------------------------------------------------------------------------------------------------------------------------------: |
> 	| cell 1           | Writing '\|' and '\-' using escape character `\`                        | cell 3                                                                                                                              |
> 	| cell 4 is longer.| cell 5                                                                  | cell 6 is much longer than the others, but that's ok. It eventually wraps the text when the cell is too large for the display size. |
> 	| cell 7           | This item has:<br>- Multiple items<br>- That we want listed separately. | cell 9                                                                                                                              |