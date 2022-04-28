# Contributing

## Purpose of this Repo

I wonder if this gets copied when I create a repo based on this template?

## Opening Issues

- If you found a [bug](https://github.com/nighterrors/[RepoGoesHere]/issues/new?assignees=&labels=bug&template=bug_report.md&title=%5BBUG%5D)
- Have a [suggestion](https://github.com/nighterrors/[RepoGoesHere]/issues/new?assignees=&labels=&template=suggestion.md&title=%5BIMP%5D)

## Coding Style

### Based on

[WordPress Coding Standards](https://codex.wordpress.org/WordPress_Coding_Standards#Indentation)

### Key rules

#### General

- **_Use `tab` characters to indent lines!_**
- **Comments are not allowed at the ends of machine readable lines**, unless:
- **It's work-in-progress.**<br /><aside>Eg.: Todo, Fixme, etc.</aside>
- **It's a demonstration** and the comment explains what happens in that line or tells what to do with it.
- **Comments should start at the same indent as the line they belong to.**
- 

#### HTML

- **Close self closing tags with ` />`.**
- **Booleans in HTML should be in short form.**<br /><aside>Eg.: ✅`defer` instead of 🚫`defer=true`.</aside>
- **Arguments should always be quoted.**
- **Use single quote `'` for well known keywords.**<br /><aside>Eg.: `<html lang='en' >`.</aside>
- **But double quotes `"` for arbitrary strings.**<br /><aside>Eg.: `<a href="github.com" >`.</aside>
- **Attribute order:**
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

## Pull Requests
