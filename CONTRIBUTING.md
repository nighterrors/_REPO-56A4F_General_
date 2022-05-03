# Contributing

## Purpose of this Repo

I wonder if this gets copied when I create a repo based on this template?

## Opening Issues

- If you found a [bug](https://github.com/nighterrors/[RepoGoesHere]/issues/new?assignees=&labels=bug&template=bug_report.md&title=%5BBUG%5D)
- Have a [suggestion](https://github.com/nighterrors/[RepoGoesHere]/issues/new?assignees=&labels=&template=suggestion.md&title=%5BIMP%5D)

## Coding Style

### Based on

* [WordPress Coding Standards](https://codex.wordpress.org/WordPress_Coding_Standards#Indentation)

See also:

* [Clean Code Explained](https://www.freecodecamp.org/news/clean-coding-for-beginners/)
* [I Shall Call It.. SomethingManager](https://blog.codinghorror.com/i-shall-call-it-somethingmanager/)

### Key rules

#### General

- *Indentation should reflect logical structure.*
- **_Use `tab` characters to indent lines!_**<sup id="Ag001Tabs">[[1]](#Fg001Tabs)</sup>
- **Comments are not allowed at the ends of machine readable lines.**<sup id="Ag002DontCommentAtEndOfLine">[[2]](#Fg002DontCommentAtEndOfLine)</sup>, unless:
	- **It's work-in-progress.**<br /><aside>Eg.: Todo, Fixme, etc.</aside>
	- **It's a demonstration** and the comment explains what happens in that line or tells what to do with it.
- **Comments should start at the same indent as the line they belong to.**<sup id="Ag003CommentAtSameIndent">[[3]](#Fg003CommentAtSameIndent)</sup>
- *Prefer descriptive names over explanations.*<sup id="Ag004DescriptiveNames">[[4]](#Fg004DescriptiveNames)</sup>
- *But describe what needs to be in comments.*<sup id="Ag005AddDescriptions">[[5]](#Fg005AddDescriptions)</sup>

#### HTML

- **Close self closing tags with ` />`.**<sup id="Ah006SlashCloseEmptyElements">[[6]](#Fh006SlashCloseEmptyElements)</sup>
- **Booleans in HTML should be in short form.**<sup id="Ah007BooleanAttributes">[[7]](#Fh007BooleanAttributes)</sup><br /><aside>Eg.: ✅`defer` instead of 🚫`defer=true`.</aside>
- **Attribute values should always be quoted.**<sup id="Ah008StringAttributeValues">[[8]](#Fh008StringAttributeValues)</sup>
- **Use single quote `'` for well known keywords.**<sup id="Ah009SingleQuoteKeyWords">[[9]](#Fh009SingleQuoteKeyWords)</sup><br /><aside>Eg.: `<html lang='en' >`.</aside>
- **But double quotes `"` for arbitrary strings.**<sup id="Ah010DoubleQuoteStrings">[[10]](#Fh010DoubleQuoteStrings)</sup><br /><aside>Eg.: `<a href="github.com" >`.</aside>
- **Attribute order:**<sup id="Ah011AttributeOrder">[[11]](#Fh011AttributeOrder)</sup>
	1. Class
	2. ID
	3. Title
	4. Others
	5. Booleans
	6. Link (`href`, `src`, etc.)

#### CSS

- 

#### JS

##### Naming convention

- **Use CapitalCamelCase for custom stuff**<sup id="Aj016CapitalCamelCase">[[16]](#Fj016CapitalCamelCase)</sup>, so they're clearly distinguishable from built-ins.
- **The first two letters of the name are reserved for classification**<sup id="Aj017Classification">[[17]](#Fj017Classification)</sup>:

	|First letter|type of object|
	|:---:|---|
	|F|Function|
	|C|Constant|
	|L|Variable declared with `let`|
	|I|Variable declared implicitly (such as a function's argument)|
	|V|Variable declared with `var`|
	|K|Key in a dictionary|
	|P|Class|
	|D|Field|
	|M|Method|

	|Second letter|type of data it holds / returns|
	|:---:|---|
	|n|None (e.g. when a function doesn't have return value)|
	|b|Boolean|
	|i|Integer|
	|f|Float|
	|s|String|
	|a|Array|
	|o|Object|
	|v|Variant (if it's unknown, or can have different types)|

### Rationale

#### General

<dl>
	<dt id="Fg001Tabs"><a title="Use `tab` characters to indent lines!" href="#Ag001Tabs">1^</a></dt>
		<dd>**Tabs are flexible.** Either you prefer 2 or 4 spaces per indention level(, or any other uncommon number), using tabs lets you set up your editor to render them as short or as long as you like it. And it doesn't matter if your friends / colleagues prefer it differently, y'all can allways collaborate on the same file and still have it rendered the way you like it.</dd>
		<dd></dd>
		<dd>Using tabs saves you at least 1 B per character;)</dd>
	<dt id="Fg002DontCommentAtEndOfLine"><a title="Comments are not allowed at the ends of machine readable lines" href="#Ag002DontCommentAtEndOfLine">2^</a></dt>
		<dd></dd>
	<dt id="Fg003CommentAtSameIndent"><a title="Comments should start at the same indent as the line they belong to." href="#Ag003CommentAtSameIndent">3^</a></dt>
		<dd></dd>
</dl>

#### HTML

<dl>
	<dt id="Fh006SlashCloseEmptyElements"><a href="#Ah006SlashCloseEmptyElements">6^</a></dt>
		<dd> </dd>
	<dt id="Fh007BooleanAttributes"><a href="#Ah007BooleanAttributes">7^</a></dt>
		<dd> </dd>
	<dt id="Fh008StringAttributeValues"><a href="#Ah008StringAttributeValues">8^</a></dt>
		<dd> </dd>
	<dt id="Fh009SingleQuoteKeyWords"><a href="#Ah009SingleQuoteKeyWords">9^</a></dt>
		<dd> </dd>
	<dt id="Fh010DoubleQuoteStrings"><a href="#Ah010DoubleQuoteStrings">10^</a></dt>
		<dd> </dd>
	<dt id="Fh011AttributeOrder"><a href="#Ah011AttributeOrder">11^</a></dt>
		<dd> </dd>
</dl>

#### CSS

<dl>
	<dt id="Fc010"><a href="#Ac010">10^</a></dt>
		<dd> </dd>
	<dt id="Fc011"><a href="#Ac011">11^</a></dt>
		<dd> </dd>
	<dt id="Fc012"><a href="#Ac012">12^</a></dt>
		<dd> </dd>
	<dt id="Fc013"><a href="#Ac013">13^</a></dt>
		<dd> </dd>
	<dt id="Fc014"><a href="#Ac014">14^</a></dt>
		<dd> </dd>
	<dt id="Fc015"><a href="#Ac015">15^</a></dt>
		<dd> </dd>
</dl>

#### JS

<dl>
	<dt id="Fj016CapitalCamelCase"><a href="#Aj016CapitalCamelCase">16^</a></dt>
		<dd> </dd>
	<dt id="Fj017Classification"><a href="#Aj017Classification">17^</a></dt>
		<dd> </dd>
	<dt id="Fj018"><a href="#Aj018">18^</a></dt>
		<dd> </dd>
	<dt id="Fj019"><a href="#Aj019">19^</a></dt>
		<dd> </dd>
	<dt id="Fj020"><a href="#Aj020">20^</a></dt>
		<dd> </dd>
	<dt id="Fj021"><a href="#Aj021">21^</a></dt>
		<dd> </dd>
</dl>

## Pull Requests
