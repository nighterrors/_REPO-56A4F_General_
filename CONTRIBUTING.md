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

Also please follow our [branch hierarchy](#branch-hierarchy)!

### Branch Hierarchy

<?>
This repo comes with 3 major branches:
1. [`main`](https://github.com/nighterrors/_REPO-56A4F_General_/tree/main) - For active develoopment. *Merges into `test`.*
2. [`test`](https://github.com/nighterrors/_REPO-56A4F_General_/tree/test) - For testing. *Merges into `prod`.*
3. [`prod`](https://github.com/nighterrors/_REPO-56A4F_General_/tree/prod) - For releases.

And 3 types of side branches:
- `feat/[feature's name]` - For feature develoopment. *Merges into `main`.*
- `bgfx/[bug track id]` - For bug fixes. *Merges into `main` or `test`.*
- `htfx/[bug track id]` - For hot fixes. *Merges into `prod`.* 
<?/?>

```mermaid
graph LR

feat/some_feature --> main
feat/some_other_feature --> main
feat/some_feature --> bgfx/#id1
bgfx/#id1 --> main

main --> test
main --> bgfx/#id2
bgfx/#id2 --> test

test --> prod
htfx/#id3 --> prod
```

#### Workflow

<?>
1. Development happens on separate *Feature* branches (`feat/[feature's name]`).
2. Once a feature is complete, it's merged into `main`. 
3. When a development phase is complete, `main` is merged into `test`, where the testing takes place.
4. Once all tests are passed, `test` merged into the default branch: `prod`, thus concluding that phase.

```puml
@startuml

feat_a_b -> main
main -> test
main -> test
test -> prod

@enduml
```

```puml
@startuml

feat_c_d_e -> main
main -> test
test -> prod

@enduml
```

-	Bug fixes branch out from wherever they were discovered and merged into either:
	-	`main` if they were discovered during development phase;
	-	Also `main` if the fix will be part of the next `major` or `minor` realease.
	-	or `test` if it'll be part of a `patch` release.
-	Hot fixes similar to bug fixes have their independent branches. But unlike the former they -after careful testing- merge directly into `prod`.

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

0. *Indentation should reflect logical structure.*

	:	Duh.

0. ***Use <kbd>tab</kbd> characters to indent lines!***

	:	**Tabs are flexible.** Either you prefer 2 or 4 spaces per indention level(, or any other uncommon number), using tabs lets you set up your editor to render them as short or as long as you like it. And it doesn't matter if your friends / colleagues prefer it differently, y'all can allways collaborate on the same file and still have it rendered the way you like it.

	:	Using tabs saves you at least 1 B per character;)

	:	I haven't found any -good- reason not to.

0. **Comments should start at the same indent as the line they belong to.**

	:	It looks nice and structured.

0. *Prefer descriptive names over explanations.*

	:	It'll help remebering what it does, without having to find where it was explained.

	:	It'll also help others better understand the code.

0. *But describe what needs to be in comments.*

	:	This helps understand the code that was written a long time ago.

	:	But also helps others, who would like to collaborate or just having issues with the code. Especially if they aren't programmers.

	:	Also quite invaluable in debugging.

	:	*So please explain what each block of code supposed to do!*

0. *Use comments to further structure your code* by adding titles to sections.

	:	Helps readability and finding relevant parts of the code.

#### HTML

6. **Close self-closing elements with ` />`.**

	:	For XML compatibility.

	>	As per W3C recommendation, these tags should be closed with exactly one space followed by a forward slash.

6. **Booleans in HTML should be in short form.**

	:	To improve readability.

	>	E.g.: ✅`defer` instead of ❌`defer=true`.

6. **Attribute values should always be quoted.**

	:	For XML compatibility.

	:	And to avoid errors.

6. **Use single quote `'` for well known keywords.**

	:	To help distinguish them.

	>	E.g.: `<html lang='en' >`.

6. **But double quotes `"` for arbitrary strings.**

	:	To help distinguish keywords from.

	>	E.g.: `<a href="github.com" >`.

6. **Tags, attributes and keywords should be lowercase.**

	:	To help distinguish text intended for humans vs. machines.

	>	All tags and attributes must be lowercase. Plus any keyword interpreted by machines, except arbitrary names likes variables, classes, IDs, etc..
	>	E.g.: `<link rel='icon' type='image/icon' href="favicon.ico" />`.

6. **Attribute order:**

	:	It helps finding relevant parts of tags with a lot of attributes.

	:	Keeps things nice and organized.

	1. Class
	2. ID
	3. Title
	4. ... Others ...
	5. Booleans
	6. Link (`href`, `src`, etc.)

	>	From left to right: IDs from more general to the most specific.
	>	Leftmost: Most important attribute.

#### CSS

<!--TODO-->

#### JS

<!--TODO-->

##### Naming convention

13. **Use CapitalCamelCase for custom stuff.**

	:	Makes them clearly distinguishable from built-ins.

13. **The first two letters of the name are reserved for classification**

	:	Helps to identify objects and their purpose.

	:	Thus helping with 3), by providing a shorthand description of type and possibly content.

	:	Helps ensure 13).

|First letter	|type of object													|
|:--:			|--																|
|F				|Function														|
|C				|Constant														|
|L				|Variable declared with `let`									|
|I				|Variable declared implicitly (such as a function's argument)	|
|V				|Variable declared with `var`									|
|K				|Key in a dictionary											|
|P				|Class															|
|D				|Field															|
|M				|Method															|

|Second letter	|type of data it holds / returns								|
|:--:			|--																|
|- or _			|None (e.g. when a function doesn't have return value)			|
|b				|Boolean														|
|n				|General numeric value											|
|i				|Integer														|
|f				|Float															|
|s				|String															|
|a				|Array															|
|o				|Object															|
|v				|Variant (if it's unknown, or can have different types)			|
