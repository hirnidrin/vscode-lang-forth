# Forth syntax highlighting for VS Code

## Purpose

This *Visual Studio Code* extension provides syntax highlighting for the Forth programming language. 

It also supports
* line comments with the "\\" char, bound to the default VS Code line comment keys.
* block comments: Forth does not have a standard block comment mechanism. The extension experimentally implements the somewhat ugly *0 [IF] ... [THEN]* workaround, bound to the default VS Code block comment toggle key.
* code completion (auto close) for the : ... ; pair

It does NOT provide identifier navigation, code snippets, folding, completion, templates, compiling or debug support.

## How to use

* After installing and activating the extension in VS Code, any file with one of the extensions *.fs .4th .fth .frt .forth* is recognized as Forth source file, and syntax highlighting kicks in.

* You can make it work for more file extensions by adding them to your VS Code *User Settings* in the settings.json file, for example: 

        "files.associations": {
            "*.444": "forth",
        }

## Bug Report

Report bugs and issues [here](https://github.com/hirnidrin/vscode-lang-forth/issues).

## Credits

The syntax highlighting file ./syntaxes/forth.tmLanguage.json of the initial release is an exact (jsonified) copy of [Maximilian Irro's Forth for Atom](https://github.com/mpgirro/language-forth) package, which he released under an MIT license.  Thank you for doing the hard part!

## Changelog

### Version 0.0.1

Initial release.
