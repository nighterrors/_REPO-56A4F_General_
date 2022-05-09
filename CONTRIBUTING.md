# Contributing

[[Intro goes here.]] <!--TODO-->

## Purpose of this Repo

[[@Purpose]]

## Community Standards

[See my community standards](https://github.com/nighterrors/_REPO-56A4F_General_/blob/main/CODE_OF_CONDUCT.md)

[[Spoiler: Tere are none:( - This is just a template, after all.]]

## Forum <!--TODO-->

- [Help out by answering questions](https://github.com/nighterrors/_REPO-56A4F_General_/discussions/categories/q-a).
- *[Especially if you are bilingual](https://github.com/nighterrors/_REPO-56A4F_General_/discussions/categories/foreign-help)!*

## Documentation <!--TODO-->

- [Help out by writing documentation](https://github.com/nighterrors/_REPO-56A4F_General_/wiki).

## Coding Style

### Based on

- [WordPress Coding Standards](https://codex.wordpress.org/WordPress_Coding_Standards#Indentation)

#### See also

- [Clean Code Explained](https://www.freecodecamp.org/news/clean-coding-for-beginners/)
- [I Shall Call It.. SomethingManager](https://blog.codinghorror.com/i-shall-call-it-somethingmanager/)

### Key rules

#### General

<ol start="0">
<li><em>Indentation should reflect logical structure.</em><sup id="AgStructure"><a title="Duh." href="#FgStructure">[0]</a></sup></li>
<li><strong><em>Use <kbd>tab</kbd> characters to indent lines!</em></strong><sup id="AgTabs"><a title="Tabs are flexible. Either you prefer 2 or 4 spaces per indention level(, or any other uncommon number), using tabs lets you set up your editor to render them as short or as long as you like it. And it doesn't matter if your friends / colleagues prefer it differently, y'all can allways collaborate on the same file and still have it rendered the way you like it. Using tabs saves you at least 1 B per character;) I haven't found any -good- reason not to." href="#FgTabs">[1]</a></sup></li>
<li><strong>Comments should start at the same indent as the line they belong to.</strong><sup id="AgCommentAtSameIndent"><a title="It looks nice and structured." href="#FgCommentAtSameIndent">[2]</a></sup></li>
<li><em>Prefer descriptive names over explanations.</em><sup id="AgDescriptiveNames"><a title="It'll help remebering what it does, without having to find where it was explained. It'll also help others better understand the code." href="#FgDescriptiveNames">[3]</a></sup></li>
<li><em>But describe what needs to be in comments.</em><sup id="AgAddDescriptions"><a title="This helps understand the code that was written a long time ago. But also helps others, who would like to collaborate or just having issues with the code. Especially if they aren't programmers. Also quite invaluable in debugging. So please explain what each block of code supposed to do!" href="#FgAddDescriptions">[4]</a><sup></li>
<li><em>Use comments to further structure your code</em> by adding titles to sections.<sup id="AgSections"><a title="Helps readability and finding relevant parts of the code." href="#FgSections">[5]</a></sup></li>
</ol>

#### HTML

<ol start="6">
<li><strong>Close self-closing elements with <code> /&gt;</code>.</strong><sup id="AhSpaceSlashCloseEmptyElements"><a title="For XML compatibility." href="#FhSpaceSlashCloseEmptyElements">[6]</a></sup><br /><aside>As per W3C recommendation, these tags should be closed with exactly one space followed by a forward slash.</aside></li>
<li><strong>Booleans in HTML should be in short form.</strong><sup id="AhBooleanAttributes"><a title="To improve readability." href="#FhBooleanAttributes">[7]</a></sup><br /><aside>E.g.: ✅<code>defer</code> instead of ❌<code>defer=true</code>.</aside></li>
<li><strong>Attribute values should always be quoted.</strong><sup id="AhStringAttributeValues"><a title="For XML compatibility. And to avoid errors." href="#FhStringAttributeValues">[8]</a></sup></li>
<li><strong>Use single quote <code>'</code> for well known keywords.</strong><sup id="AhSingleQuoteKeyWords"><a title="To help distinguish them." href="#FhSingleQuoteKeyWords">[9]</a></sup><br /><aside>E.g.: <code>&lt;html lang='en' &gt;</code>.</aside></li>
<li><strong>But double quotes <code>"</code> for arbitrary strings.</strong><sup id="AhDoubleQuoteStrings"><a title="To help distinguish keywords from." href="#FhDoubleQuoteStrings">[10]</a></sup><br /><aside>E.g.: <code>&lt;a href="github.com" &gt;</code>.</aside></li>
<li><strong>Tags, attributes and keywords should be lowercase.</strong><sup id="AhLowercaseKeywords"><a title="To help distinguish text intended for humans vs. machines." href="#FhLowercaseKeywords">[11]</a></sup><br />All tags and attributes must be lowercase. Plus any keyword interpreted by machines, except arbitrary names likes variables, classes, IDs, etc..<br /><aside>E.g.: <code>&lt;link rel='icon' type='image/icon' href="favicon.ico" /&gt;</code></li>
<li><strong>Attribute order:</strong><sup id="AhAttributeOrder"><a title="It helps finding relevant parts of tags with a lot of attributes. Keeps things nice and organized." href="#FhAttributeOrder">[12]</a></sup><br />From left to right: IDs from more general to the most specific.<br />Leftmost: Most important attribute.</li>
	<ol>
		<li>Class</li>
		<li>ID</li>
		<li>Title</li>
		<li>... Others ...</li>
		<li>Booleans</li>
		<li>Link (<code>href</code>, <code>src</code>, etc.)</li>
	</ol>
</ol>

#### CSS

<!--TODO-->

#### JS

<!--TODO-->

##### Naming convention

<ol start="14">
<li><strong>Use CapitalCamelCase for custom stuff.</strong><sup id="AjCapitalCamelCase"><a title="Makes them clearly distinguishable from built-ins." href="#FjCapitalCamelCase">[14]</a></sup></li>
<li><strong>The first two letters of the name are reserved for classification</strong><sup id="AjClassification"><a title="Helps to identify objects and their purpose. Thus helping with 3^, by providing a shorthand description of type and possibly content. Helps ensure 14^." href="#FjClassification">[15]</a></sup>:</li>
</ol>

<table>
	<!-- FIXME: Column alignment -->
	<colgroup>
		<col align='center' />
		<col align='justify' />
	</colgroup>
	<tr>
		<th>First letter</th>
		<th>type of object</th>
	</tr>
	<tr>
		<td>F</td>
		<td>Function</td>
	</tr>
	<tr>
		<td>C</td>
		<td>Constant</td>
	</tr>
	<tr>
		<td>L</td>
		<td>Variable declared with <code>let</code></td>
	</tr>
	<tr>
		<td>I</td>
		<td>Variable declared implicitly (such as a function's argument)</td>
	</tr>
	<tr>
		<td>V</td>
		<td>Variable declared with <code>var</code></td>
	</tr>
	<tr>
		<td>K</td>
		<td>Key in a dictionary</td>
	</tr>
	<tr>
		<td>P</td>
		<td>Class</td>
	</tr>
	<tr>
		<td>D</td>
		<td>Field</td>
	</tr>
	<tr>
		<td>M</td>
		<td>Method</td>
	</tr>
</table>

<table>
	<!-- FIXME: Column alignment -->
	<colgroup>
		<col align='center' />
		<col align='justify' />
	</colgroup>
	<tr>
		<th>Second letter</th>
		<th>type of data it holds / returns</th>
	<tr>
		<td>n</td>
		<td>None (e.g. when a function doesn't have return value)</td>
	</tr>
	<tr>
		<td>b</td>
		<td>Boolean</td>
	</tr>
	<tr>
		<td>i</td>
		<td>Integer</td>
	</tr>
	<tr>
		<td>f</td>
		<td>Float</td>
	</tr>
	<tr>
		<td>s</td>
		<td>String</td>
	</tr>
	<tr>
		<td>a</td>
		<td>Array</td>
	</tr>
	<tr>
		<td>o</td>
		<td>Object</td>
	</tr>
	<tr>
		<td>v</td>
		<td>Variant (if it's unknown, or can have different types)</td>
	</tr>
</table>

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
	<dt id="FhSpaceSlashCloseEmptyElements">6 <a title="Self-closing elements" href="#AhSpaceSlashCloseEmptyElements">^</a> Self-closing elements:</dt>
		<dd>For XML compatibility.</dd>
	<dt id="FhBooleanAttributes">7 <a title="Boolean attributes" href="#AhBooleanAttributes">^</a> Boolean attributes:</dt>
		<dd>To improve readability.</dd>
	<dt id="FhStringAttributeValues">8 <a title="Quote attribute values" href="#AhStringAttributeValues">^</a> Quote attribute values:</dt>
		<dd>For XML compatibility.</dd>
		<dd>And to avoid errors.</dd>
	<dt id="FhSingleQuoteKeyWords">9 <a title="Single quote keywords" href="#AhSingleQuoteKeyWords">^</a> Single quote keywords:</dt>
		<dd>To help distinguish them.</dd>
	<dt id="FhDoubleQuoteStrings">10 <a title="Double quote strings" href="#AhDoubleQuoteStrings">^</a> Double quote strings:</dt>
		<dd>To help distinguish keywords from.</dd>
	<dt id="FhLowercaseKeywords">11 <a title="Lowercase keywords" href="#AhLowercaseKeywords">^</a> Lowercase keywords:</dt>
		<dd>To help distinguish text intended for humans vs. machines.</dd>
	<dt id="FhAttributeOrder">12 <a title="Attribute order" href="#AhAttributeOrder">^</a> Attribute order:</dt>
		<dd>It helps finding relevant parts of tags with a lot of attributes.</dd>
		<dd>Keeps things nice and organized.</dd>
</dl>

#### CSS

<!--dl>
	<dt id="Fc">13 <a href="#Ac">^</a> </dt>
		<dd></dd>
</dl-->

#### JS

##### Naming convention

<dl>
	<dt id="FjCapitalCamelCase">14 <a title="CapitalCamelCase" href="#AjCapitalCamelCase">^</a> CapitalCamelCase:</dt>
		<dd>Makes them clearly distinguishable from built-ins.</dd>
	<dt id="FjClassification">15 <a title="Classification" href="#AjClassification">^</a> Classification:</dt>
		<dd>Helps to identify objects and their purpose.</dd>
		<dd>Thus helping with 3<a title="Add descriptive names to stuff" href="#AgDescriptiveNames">^</a>, by providing a shorthand description of type and possibly content.</dd>
		<dd>Helps ensure 14<a title="CapitalCamelCase" href="#AjCapitalCamelCase">^</a>.</dd>
	<!--dt id="Fj">16 <a title="" href="#Aj">^</a> </dt>
		<dd> </dd-->
</dl>

## Pull Requests

[[@PR]]
