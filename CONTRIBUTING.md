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

- **_Use `tab` characters to indent lines!_**<sup id="Ag001">[[1]](#Fg001)</sup>
- **Comments are not allowed at the ends of machine readable lines**<sup id="Ag002">[[2]](#Fg002)</sup>, unless:
	- **It's work-in-progress.**<br /><aside>Eg.: Todo, Fixme, etc.</aside>
	- **It's a demonstration** and the comment explains what happens in that line or tells what to do with it.
- **Comments should start at the same indent as the line they belong to.**<sup id="Ag003">[[3]](#Fg003)</sup>
- 

#### HTML

- **Close self closing tags with ` />`.**<sup id="Ah004">[[4]](#Fh004)</sup>
- **Booleans in HTML should be in short form.**<sup id="Ah005">[[5]](#Fh005)</sup><br /><aside>Eg.: ✅`defer` instead of 🚫`defer=true`.</aside>
- **Arguments should always be quoted.**<sup id="Ah006">[[6]](#Fh006)</sup>
- **Use single quote `'` for well known keywords.**<sup id="Ah007">[[7]](#Fh007)</sup><br /><aside>Eg.: `<html lang='en' >`.</aside>
- **But double quotes `"` for arbitrary strings.**<sup id="Ah008">[[8]](#Fh008)</sup><br /><aside>Eg.: `<a href="github.com" >`.</aside>
- **Attribute order:**<sup id="Ah009">[[9]](#Fh009)</sup>
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

- **Use CapitalCamelCase for custom stuff**, so they're clearly distinguishable from built-ins.
- **The first two letters of the name are reserved for classification**:

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
	<dt id="Fg001"><a href="#Ag001">1^</a></dt>	<dd></dd>
												<dd></dd>
												<dd></dd>
	<dt id="Fg002"><a href="#Ag002">2^</a></dt>	<dd></dd>
	<dt id="Fg003"><a href="#Ag003">3^</a></dt>	<dd></dd>
</dl>

#### HTML

<dl>
	<dt id="Fh004"><a href="#Ah004">4^</a></dt>	<dd> </dd>
	<dt id="Fh005"><a href="#Ah005">5^</a></dt>	<dd> </dd>
	<dt id="Fh006"><a href="#Ah006">6^</a></dt>	<dd> </dd>
	<dt id="Fh007"><a href="#Ah007">7^</a></dt>	<dd> </dd>
	<dt id="Fh008"><a href="#Ah008">8^</a></dt>	<dd> </dd>
	<dt id="Fh009"><a href="#Ah009">9^</a></dt>	<dd> </dd>
</dl>

#### CSS

<dl>
	<dt id="Fc010"><a href="#Ac010">10^</a></dt>	<dd> </dd>
	<dt id="Fc011"><a href="#Ac011">11^</a></dt>	<dd> </dd>
	<dt id="Fc012"><a href="#Ac012">12^</a></dt>	<dd> </dd>
	<dt id="Fc013"><a href="#Ac013">13^</a></dt>	<dd> </dd>
	<dt id="Fc014"><a href="#Ac014">14^</a></dt>	<dd> </dd>
	<dt id="Fc015"><a href="#Ac015">15^</a></dt>	<dd> </dd>
</dl>

#### JS

<dl>
	<dt id="Fj016"><a href="#Aj016">16^</a></dt>	<dd> </dd>
	<dt id="Fj017"><a href="#Aj017">17^</a></dt>	<dd> </dd>
	<dt id="Fj018"><a href="#Aj018">18^</a></dt>	<dd> </dd>
	<dt id="Fj019"><a href="#Aj019">19^</a></dt>	<dd> </dd>
	<dt id="Fj020"><a href="#Aj020">20^</a></dt>	<dd> </dd>
	<dt id="Fj021"><a href="#Aj021">21^</a></dt>	<dd> </dd>
</dl>

## Pull Requests
