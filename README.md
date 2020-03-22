# VsCode GroovyLint (and fix!)

**Lint** and **fix** your groovy files and Jenkinsfile 

This extension is based on [npm-groovy-lint](https://github.com/nvuillam/npm-groovy-lint#README) package, itself based on [CodeNarc](https://codenarc.github.io/CodeNarc/) groovy linter

Autofixing is still experimental, please post an [issue](https://github.com/nvuillam/vscode-groovy-lint/issues) if you detect any problem

## Features

| Command                         | Description                                                                                    | Access                                                                                                   |
|---------------------------------|------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------|
| **Analyze code**                | Lint the code of the current tab                                                               | Ctrl+Shit+F9<br/>Editor contextual menu</br>Status bar GroovyLint item<br/>Command pannel (Ctrl+Shipf+P) |
| **Fix all errors**              | Fix the code of the current tab                                                                | Ctrl+Shit+F10<br/>Editor contextual menu</br>Command pannel (Ctrl+Shipf+P)                                |
| Fix single error                | Apply quick fix for a single error                                                             | Quick Fix contextual menu<br/>Diagnostic contextual menu                                                 |
| Fix _errorType_ in file         | Apply quick fix for all errors of the same type in the currrent tab                            | Quick Fix contextual menu<br/>Diagnostic contextual menu                                                 |
| Ignore _errorType_ in all files | Updates configuration file (usually .groovylintrc.js in root folder) to ignore this error type | Quick Fix contextual menu<br/>Diagnostic contextual menu                                                 |

## Extension Settings

| Parameter                        | Description                                                                                     | Default          |
|----------------------------------|-------------------------------------------------------------------------------------------------|------------------|
| `groovyLint.basic.enable`        | Controls whether GroovyLint is enabled or not                                                   | true             |
| `groovyLint.basic.run`           | Run the linter on save (onSave) or on type (onType)                                             | onSave           |
| `groovyLint.basic.autoFixOnSave` | Turns auto fix on save on or off                                                                | false            |
| `groovyLint.basic.loglevel`      | Linting error level (error, warning,info)                                                       | info             |
| `groovyLint.basic.verbose`       | Turn on to have verbose logs                                                                    | false            |
| `groovyLint.basic.config`        | [NPM groovy lint configuration file](https://github.com/nvuillam/npm-groovy-lint#configuration) | .groovylintrc.js |

## Known Issues

As CodeNarc is runned in background with java/groovy, performances could be improved on large files (do not hesitate to provide advices !)
But do not worry, as the groovy linting is provided by a background local server, your VsCode won't be slowed

## Release Notes

Users appreciate release notes as you update your extension.

### 0.1.0

Initial release of VsCode Groovy Lint

-----------------------------------------------------------------------------------------------------------

