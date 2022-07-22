# Contributing

There are many ways to help out this project. Some require programming skills, but others don't. *Here topics are ordered by their required skill level.*

---

<?>
@ToC
<?/?>

## Purpose of this Repo

<?>
This is a general purpose template repo, with potential customization capabilities (customization not implemented yet).
<?/?>

<?>
@Purpose
<?/?>

## Community Standards

See the [community standards](https://github.com/nighterrors/_REPO-56A4F_General_/blob/main/CODE_OF_CONDUCT.md)!

<?>
Spoiler: Tere are none:( - This is just a template, after all.
<?/?>

## Forum

*Doesn't require coding skills, just an understanding how it works is enough to help others how to use it.*

- [Help out by answering questions](https://github.com/nighterrors/_REPO-56A4F_General_/discussions/categories/q-a).
- *[Especially if you are bilingual](https://github.com/nighterrors/_REPO-56A4F_General_/discussions/categories/foreign-help)!*

## Documentation

*Under the hood documentation requires understanding the code, but usage instructions don't necessarily.*

- [Help out by writing documentation](https://github.com/nighterrors/_REPO-56A4F_General_/wiki).

## Codebase

*This definitely requires coding skills.*

Before contributing to the codebase, please read our [coding guidelines](#Coding-Style)!

- See if there are [open issues](https://github.com/nighterrors/_REPO-56A4F_General_/issues?q=is%3Aopen+is%3Aissue), you can help with.
	- Start with [something easy](https://github.com/nighterrors/_REPO-56A4F_General_/labels/good%20first%20issue), just to see how you like it!
	- Help us with our most [pressing issues](https://github.com/nighterrors/_REPO-56A4F_General_/labels/help%20wanted)!
	- [Bug fixes](https://github.com/nighterrors/_REPO-56A4F_General_/labels/bug) are allways wellcome!
	- Or maybe you'd like to [implement new features](https://github.com/nighterrors/_REPO-56A4F_General_/labels/enhancement)?

*At any rate, please start by replying to the issue, **letting everyone know what you're working on, and planning to do**. Especially if you're new here!*

### Pull Requests

PRs are allways wellcome as long as they adhere to the [coding guidelines](#Coding-Style)!

<?>
1. Development happens on the [`dev-`](https://github.com/nighterrors/_REPO-56A4F_General_/tree/dev-) branch. And occasionally on separate `Feature` branches.
2. Once a phase is complete, it's merged into [`test`](https://github.com/nighterrors/_REPO-56A4F_General_/tree/test), where the testing takes place.
3. Once all tests are passed, it's merged into the default branch: [`main`](https://github.com/nighterrors/_REPO-56A4F_General_/tree/main), thus concluding that phase.
<?/?>

---

## Coding Style

### Based on

- [WordPress Coding Standards](https://codex.wordpress.org/WordPress_Coding_Standards#Indentation)

#### See also

- [Clean Code Explained](https://www.freecodecamp.org/news/clean-coding-for-beginners/)
- [I Shall Call It.. SomethingManager](https://blog.codinghorror.com/i-shall-call-it-somethingmanager/)

### Key rules

#### General

0. *Indentation should reflect logical structure.*<sup id="AgStructure"><a title="Duh." onclick="document.getElementsByTagName('article')[0].getElementsByTagName('details')[0].open=true" href="#FgStructure">[0]</a></sup>

0. ***Use <kbd>tab</kbd> characters to indent lines!*** <sup id="AgTabs"><a title="Tabs are flexible. Either you prefer 2 or 4 spaces per indention level(, or any other uncommon number), using tabs lets you set up your editor to render them as short or as long as you like it. And it doesn't matter if your friends / colleagues prefer it differently, y'all can allways collaborate on the same file and still have it rendered the way you like it. Using tabs saves you at least 1 B per character;) I haven't found any -good- reason not to." onclick="document.getElementsByTagName('article')[0].getElementsByTagName('details')[0].open=true" href="#FgTabs">[1]</a></sup>

0. **Comments should start at the same indent as the line they belong to.**<sup id="AgCommentAtSameIndent"><a title="It looks nice and structured." onclick="document.getElementsByTagName('article')[0].getElementsByTagName('details')[0].open=true" href="#FgCommentAtSameIndent">[2]</a></sup>

0. *Prefer descriptive names over explanations.*<sup id="AgDescriptiveNames"><a title="It'll help remebering what it does, without having to find where it was explained. It'll also help others better understand the code." onclick="document.getElementsByTagName('article')[0].getElementsByTagName('details')[0].open=true" href="#FgDescriptiveNames">[3]</a></sup>

0. *But describe what needs to be in comments.*<sup id="AgAddDescriptions"><a title="This helps understand the code that was written a long time ago. But also helps others, who would like to collaborate or just having issues with the code. Especially if they aren't programmers. Also quite invaluable in debugging. So please explain what each block of code supposed to do!" onclick="document.getElementsByTagName('article')[0].getElementsByTagName('details')[0].open=true" href="#FgAddDescriptions">[4]</a><sup>

0. *Use comments to further structure your code* by adding titles to sections.<sup id="AgSections"><a title="Helps readability and finding relevant parts of the code." onclick="document.getElementsByTagName('article')[0].getElementsByTagName('details')[0].open=true" href="#FgSections">[5]</a></sup>

#### HTML

6. **Close self-closing elements with ` /&gt;`.**<sup id="AhSpaceSlashCloseEmptyElements"><a title="For XML compatibility." onclick="document.getElementsByTagName('article')[0].getElementsByTagName('details')[0].open=true" href="#FhSpaceSlashCloseEmptyElements">[6]</a></sup><br /><aside>As per W3C recommendation, these tags should be closed with exactly one space followed by a forward slash.</aside>

6. **Booleans in HTML should be in short form.**<sup id="AhBooleanAttributes"><a title="To improve readability." onclick="document.getElementsByTagName('article')[0].getElementsByTagName('details')[0].open=true" href="#FhBooleanAttributes">[7]</a></sup><br /><aside>E.g.: ✅`defer` instead of ❌`defer=true`.</aside>

6. **Attribute values should always be quoted.**<sup id="AhStringAttributeValues"><a title="For XML compatibility. And to avoid errors." onclick="document.getElementsByTagName('article')[0].getElementsByTagName('details')[0].open=true" href="#FhStringAttributeValues">[8]</a></sup>

6. **Use single quote `'` for well known keywords.**<sup id="AhSingleQuoteKeyWords"><a title="To help distinguish them." onclick="document.getElementsByTagName('article')[0].getElementsByTagName('details')[0].open=true" href="#FhSingleQuoteKeyWords">[9]</a></sup><br /><aside>E.g.: `&lt;html lang='en' &gt;`.</aside>

6. **But double quotes `"` for arbitrary strings.**<sup id="AhDoubleQuoteStrings"><a title="To help distinguish keywords from." onclick="document.getElementsByTagName('article')[0].getElementsByTagName('details')[0].open=true" href="#FhDoubleQuoteStrings">[10]</a></sup><br /><aside>E.g.: `&lt;a href="github.com" &gt;`.</aside>

6. **Tags, attributes and keywords should be lowercase.**<sup id="AhLowercaseKeywords"><a title="To help distinguish text intended for humans vs. machines." onclick="document.getElementsByTagName('article')[0].getElementsByTagName('details')[0].open=true" href="#FhLowercaseKeywords">[11]</a></sup><br />All tags and attributes must be lowercase. Plus any keyword interpreted by machines, except arbitrary names likes variables, classes, IDs, etc..<br /><aside>E.g.: `&lt;link rel='icon' type='image/icon' href="favicon.ico" /&gt;`.

6. **Attribute order:**<sup id="AhAttributeOrder"><a title="It helps finding relevant parts of tags with a lot of attributes. Keeps things nice and organized." onclick="document.getElementsByTagName('article')[0].getElementsByTagName('details')[0].open=true" href="#FhAttributeOrder">[12]</a></sup><br />From left to right: IDs from more general to the most specific.<br />Leftmost: Most important attribute.

	1. Class
	1. ID
	1. Title
	1. ... Others ...
	1. Booleans
	1. Link (`href`, `src`, etc.)

#### CSS

<!--TODO-->

#### JS

<!--TODO-->

##### Naming convention

13. **Use CapitalCamelCase for custom stuff.**<sup id="AjCapitalCamelCase"><a title="Makes them clearly distinguishable from built-ins." onclick="document.getElementsByTagName('article')[0].getElementsByTagName('details')[0].open=true" href="#FjCapitalCamelCase">[13]</a></sup>

13. **The first two letters of the name are reserved for classification**<sup id="AjClassification"><a title="Helps to identify objects and their purpose. Thus helping with 3^, by providing a shorthand description of type and possibly content. Helps ensure 14^." onclick="document.getElementsByTagName('article')[0].getElementsByTagName('details')[0].open=true" href="#FjClassification">[14]</a></sup>:

|First letter|type of object                                              |
|:--:        |--                                                          |
|F           |Function                                                    |
|C           |Constant                                                    |
|L           |Variable declared with `let`                                |
|I           |Variable declared implicitly (such as a function's argument)|
|V           |Variable declared with `var`                                |
|K           |Key in a dictionary                                         |
|P           |Class                                                       |
|D           |Field                                                       |
|M           |Method                                                      |

|Second letter|type of data it holds / returns                       |
|:--:         |--                                                    |
|n            |None (e.g. when a function doesn't have return value) |
|b            |Boolean                                               |
|i            |Integer                                               |
|f            |Float                                                 |
|s            |String                                                |
|a            |Array                                                 |
|o            |Object                                                |
|v            |Variant (if it's unknown, or can have different types)|

### Rationale

<details markdown open><summary>Expand / Collapse notes</summary>

#### General

0 <a title="Structure" href="#AgStructure">^</a> Structure:
	:	Duh.

1 <a title="Tabs" href="#AgTabs">^</a> Tabs:
	:	<b>Tabs are flexible.</b> Either you prefer 2 or 4 spaces per indention level(, or any other uncommon number), using tabs lets you set up your editor to render them as short or as long as you like it. And it doesn't matter if your friends / colleagues prefer it differently, y'all can allways collaborate on the same file and still have it rendered the way you like it.
	:	Using tabs saves you at least 1 B per character;)
	:	I haven't found any -good- reason not to.

2 <a title="Indent comments" href="#AgCommentAtSameIndent">^</a> Indent comments:
	:	It looks nice and structured.

3 <a title="Add descriptive names to stuff" href="#AgDescriptiveNames">^</a> Descriptive names:
	:	It'll help remebering what it does, without having to find where it was explained.
	:	It'll also help others better understand the code.

4 <a title="Explain your code!" href="#AgAddDescriptions">^</a> Explain:
	:	This helps understand the code that was written a long time ago.
	:	But also helps others, who would like to collaborate or just having issues with the code. Especially if they aren't programmers.
	:	Also quite invaluable in debugging.
	:	*So please explain what each block of code supposed to do!*

5 <a title="Sections" href="#AgSections">^</a> Sections:
	:	Helps readability and finding relevant parts of the code.

#### HTML

6 <a title="Self-closing elements" href="#AhSpaceSlashCloseEmptyElements">^</a> Self-closing elements:
	:	For XML compatibility.

7 <a title="Boolean attributes" href="#AhBooleanAttributes">^</a> Boolean attributes:
	:	To improve readability.

8 <a title="Quote attribute values" href="#AhStringAttributeValues">^</a> Quote attribute values:
	:	For XML compatibility.
	:	And to avoid errors.

9 <a title="Single quote keywords" href="#AhSingleQuoteKeyWords">^</a> Single quote keywords:
	:	To help distinguish them.

10 <a title="Double quote strings" href="#AhDoubleQuoteStrings">^</a> Double quote strings:
	:	To help distinguish keywords from.

11 <a title="Lowercase keywords" href="#AhLowercaseKeywords">^</a> Lowercase keywords:
	:	To help distinguish text intended for humans vs. machines.

12 <a title="Attribute order" href="#AhAttributeOrder">^</a> Attribute order:
	:	It helps finding relevant parts of tags with a lot of attributes.
	:	Keeps things nice and organized.

#### CSS

<!--dl>
	<dt id="Fc">13 <a href="#Ac">^</a> </dt>
		<dd></dd>
</dl-->

#### JS

##### Naming convention

13 <a title="CapitalCamelCase" href="#AjCapitalCamelCase">^</a> CapitalCamelCase:
	:	Makes them clearly distinguishable from built-ins.

14 <a title="Classification" href="#AjClassification">^</a> Classification:
	:	Helps to identify objects and their purpose.
	:	Thus helping with 3<a title="Add descriptive names to stuff" href="#AgDescriptiveNames">^</a>, by providing a shorthand description of type and possibly content.
	:	Helps ensure 13<a title="CapitalCamelCase" href="#AjCapitalCamelCase">^</a>.

</details>
