# Contributing

## Purpose of this Repo

I wonder if this gets copied when I create a repo based on this template? - *It does*
So I guess, this'll be a good starting point do new repos?

## Opening Issues

- Before opening a new ticket, please [check if there's already one](https://github.com/nighterrors/[RepoGoesHere]/issues?q=is%3Aissue)!

- If you found a [bug](https://github.com/nighterrors/[RepoGoesHere]/issues/new?assignees=&labels=bug&template=bug_report.md&title=%5BBUG%5D)
- Have a [suggestion](https://github.com/nighterrors/[RepoGoesHere]/issues/new?assignees=&labels=&template=suggestion.md&title=%5BIMP%5D)

## Coding Style

### Based on

* [WordPress Coding Standards](https://codex.wordpress.org/WordPress_Coding_Standards#Indentation)

#### See also

* [Clean Code Explained](https://www.freecodecamp.org/news/clean-coding-for-beginners/)
* [I Shall Call It.. SomethingManager](https://blog.codinghorror.com/i-shall-call-it-somethingmanager/)

### Key rules

#### General

- *Indentation should reflect logical structure.*<sup id="AgStructure"><a title="Duh." href="#FgStructure">[0]</a></sup>
- **_Use `tab` characters to indent lines!_**<sup id="AgTabs"><a title="Tabs are flexible. Either you prefer 2 or 4 spaces per indention level(, or any other uncommon number), using tabs lets you set up your editor to render them as short or as long as you like it. And it doesn't matter if your friends / colleagues prefer it differently, y'all can allways collaborate on the same file and still have it rendered the way you like it. Using tabs saves you at least 1 B per character;) I haven't found any -good- reason not to." href="#FgTabs">[1]</a></sup>
- **Comments should start at the same indent as the line they belong to.**<sup id="AgCommentAtSameIndent"><a title="It looks nice and structured." href="#FgCommentAtSameIndent">[2]</a></sup>
- *Prefer descriptive names over explanations.*<sup id="AgDescriptiveNames"><a title="It'll help remebering what it does, without having to find where it was explained. It'll also help others better understand the code." href="#FgDescriptiveNames">[3]</a></sup>
- *But describe what needs to be in comments.*<sup id="AgAddDescriptions">[\[4\]](#FgAddDescriptions)</sup>
- *Use comments to further structure your code* by adding titles to sections.<sup id="AgSections">[\[5\]](#FgSections)</sup>

#### HTML

- **Close self closing elements with ` />`.**<sup id="AhSpaceSlashCloseEmptyElements">[\[6\]](#FhSpaceSlashCloseEmptyElements)</sup><br /><aside>As per W3C recommendation, these tags should be closed with exactly one space followed by a forward slash.</aside>
- **Booleans in HTML should be in short form.**<sup id="AhBooleanAttributes">[\[7\]](#FhBooleanAttributes)</sup><br /><aside>Eg.: ✅`defer` instead of 🚫`defer=true`.</aside>
- **Attribute values should always be quoted.**<sup id="AhStringAttributeValues">[\[8\]](#FhStringAttributeValues)</sup>
- **Use single quote `'` for well known keywords.**<sup id="AhSingleQuoteKeyWords">[\[9\]](#FhSingleQuoteKeyWords)</sup><br /><aside>Eg.: `<html lang='en' >`.</aside>
- **But double quotes `"` for arbitrary strings.**<sup id="AhDoubleQuoteStrings">[\[10\]](#FhDoubleQuoteStrings)</sup><br /><aside>Eg.: `<a href="github.com" >`.</aside>
- **Tags, attributes and keywords should be lowercase.**<sup id="AhLowercaseKeywords">[\[11\]](#FhLowercaseKeywords)</sup><br /><aside>E.g.: `<link�rel='icon'�type='image/icon'�href="favicon.ico"�/>`
- **Attribute order:**<sup id="AhAttributeOrder">[\[12\]](#FhAttributeOrder)</sup>
	1. Class
	2. ID
	3. Title
	4. Others
	5. Booleans
	6. Link (`href`, `src`, etc.)

#### CSS

<!--TODO-->

#### JS

<!--TODO-->

##### Naming convention

- **Use CapitalCamelCase for custom stuff**<sup id="AjCapitalCamelCase">[\[16\]](#FjCapitalCamelCase)</sup>, so they're clearly distinguishable from built-ins.
- **The first two letters of the name are reserved for classification**<sup id="AjClassification">[\[17\]](#FjClassification)</sup>:

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
	<dt id="FgStructure">0 <a title="Structure" href="#AgStructure">^</a> Structure:</dt>
		<dd>Duh.</dd>
	<dt id="FgTabs">1 <a title="Tabs" href="#AgTabs">^</a> Tabs:</dt>
		<dd><b>Tabs are flexible.</b> Either you prefer 2 or 4 spaces per indention level(, or any other uncommon number), using tabs lets you set up your editor to render them as short or as long as you like it. And it doesn't matter if your friends / colleagues prefer it differently, y'all can allways collaborate on the same file and still have it rendered the way you like it.</dd>
		<dd>Using tabs saves you at least 1 B per character;)</dd>
		<dd>I haven't found any -good- reason not to.</dd>
	<dt id="FgCommentAtSameIndent">2 <a title="Indent comments" href="#AgCommentAtSameIndent">^</a> Indent comments:</dt>
		<dd>It looks nice and structured.</dd>
	<dt id="FgDescriptiveNames">3 <a title="Add descriptive names to stuff" href="#AgDescriptiveNames">^</a> Descriptive names:</dt>
		<dd>It'll help remebering what it does, without having to find where it was explained.</dd>
		<dd>It'll also help others better understand the code.</dd>
	<dt id="FgAddDescriptions">4 <a title="Explain your code!" href="#AgAddDescriptions">^</a> Explain:</dt>
		<dd>This helps understand the code that was written a long time ago.</dd>
		<dd>But also helps others, who would like to collaborate or just having issues with the code. Especially if they aren't programmers.</dd>
		<dd>Also quite invaluable in debugging.</dd>
  <dd><em>So please explain what each block of code supposed to do!</em></dd>
 <dt id="FgSections">5 <a title="Sections" href="#AgSections">^</a> Sections:</dt>
  <dd>Helps readability and finding relevant parts of the code.</dd>
</dl>

#### HTML

<dl>
	<dt id="FhSpaceSlashCloseEmptyElements">6 <a href="#AhSpaceSlashCloseEmptyElements">^</a> Closing empty elements:</dt>
		<dd>For XML compatibility.</dd>
	<dt id="FhBooleanAttributes">7<a href="#AhBooleanAttributes">^</a> Boolean attributes:</dt>
		<dd>To improve readability.</dd>
	<dt id="FhStringAttributeValues">8 <a href="#AhStringAttributeValues">^</a> Quote attribute values:</dt>
		<dd>For XML compatibility.</dd>
  <dd>And to avoid errors.</dd>
	<dt id="FhSingleQuoteKeyWords">9 <a href="#AhSingleQuoteKeyWords">^</a> Single quote keywords:</dt>
		<dd>To help distinguish them.</dd>
	<dt id="FhDoubleQuoteStrings">10 <a href="#AhDoubleQuoteStrings">^</a> Double quote strings:</dt>
		<dd>To help distinguish keywords from.</dd>
 <dt id="FhLowercaseKeywords">11 <a href="#AhLowercaseKeywords">^</a> Lowercase keywords:</dt>
  <dd></dd>
	<dt id="FhAttributeOrder">12 <a href="#AhAttributeOrder">^</a></dt>
		<dd> </dd>
</dl>

#### CSS

<dl>
	<dt id="Fc"><a href="#Ac">10^</a></dt>
		<dd> </dd>
</dl>

#### JS

<dl>
	<dt id="FjCapitalCamelCase"><a href="#AjCapitalCamelCase">16^</a></dt>
		<dd> </dd>
	<dt id="FjClassification"><a href="#AjClassification">17^</a></dt>
		<dd> </dd>
	<dt id="Fj"><a href="#Aj">18^</a></dt>
		<dd> </dd>
</dl>

## Pull Requests

<!--Explain how to send PRs.-->
