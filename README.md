# Jasmine Problem Matcher

[![issues](https://img.shields.io/github/issues/SeanSobey/JasmineProblemMatcher.svg)](https://github.com/SeanSobey/JasmineProblemMatcher/issues)
[![license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/SeanSobey/JasmineProblemMatcher/blob/master/LICENSE)

A problem matcher to show [Jasmine](https://jasmine.github.io/) spec errors when running tests in the terminal.

## Preview

![preview](./images/preview.png)

## Usage

You can enable this problem matcher by using its name "$jasmine".

The following example shows how to add problem matchers to your project:

```json
{
	"version": "2.0.0",
	"type": "shell",
	"tasks": [
		{
			"taskName": "test",
			"command": "jasmine",
			"group": "test",
			"args": [],
			"problemMatcher": "$jasmine"
		}
	]
}
```

Note: If you are using Typescript you can use [jasmine-ts-console-reporter](https://www.npmjs.com/package/jasmine-ts-console-reporter) to remap the matched error file to your typescript source.
