# Typescript.tools

---

### Collection of resources related to Typescript compiler api (and related things)

TSC = Typescript compiler

## AST Playground

1. [ASTExplorer](https://astexplorer.net/#/gist/84d8957b9cf1e9e9f0cdda496755c52e/latest) - Shows AST returned by TSC parser. Very useful.

2. [TypeScript AST Viewer](https://ts-ast-viewer.com) - SImilar to ASTExplorer, but custom made for Typescript. Very useful for checking symbols (not shown in ASTExplorer).

## Reading and examples

1. [Typescript Architectural Overview](https://github.com/microsoft/TypeScript/wiki/Architectural-Overview) - Explains how all the different parts of TS are connected together. Also defines the common terminologies.

2. [Typescript compiler wiki page](https://github.com/microsoft/TypeScript/wiki/Using-the-Compiler-API) - Example code to use diff parts of TS. Show boilerplate code and some example.

   _More services covered, less depth._

3. [Typescript Deep Dive by Basarat](https://basarat.gitbook.io/typescript/overview) - Good introduction to various parts of TSC api.

   _Gives the initial hints and basic concept of many apis, but often doesn't show full examples or connect the different parts it is describing. Feels like a developer's note._

4. [Typescript Transformer Handbook](https://github.com/madou/typescript-transformer-handbook) - Lots of links and examples on how to write custom transformer. More of complete working examples, less theory. Same techniques apply for using TSC api directly.

## Wrappers and utils

1. [ts-morph](https://github.com/dsherret/ts-morph) - Easier and nicer abstraction layer on top of TS internals. Exposes underlying constructs for advanced usecases.

   _Slower startup due to extra initial overhead._

2. [byots](https://github.com/basarat/byots) - Modified version of Typescript lib, which exposes more internal apis. Matching releases are created automatically.

   _TS has anyway opened up more apis, is it worth using anymore ??_

3. [ttypescript](https://github.com/cevek/ttypescript) - TSC drop-in replacement which supports passing custom transformers as cmdline argument.

## Tools built using it

1. Typescript language service plugin in VS Code (inbuilt), [atom](https://github.com/TypeStrong/atom-typescript), [Sublime Text](https://github.com/Microsoft/TypeScript-Sublime-Plugin) - Supports similar feature set in multiple editors

2. Typedoc - Very popular Typescript documentation generator which extracts type definitions and inline jsdoc comments into separate documents.


<link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/css/bootstrap.min.css" integrity="sha384-Vkoo8x4CGsO3+Hhxv8T/Q5PaXtkKtu6ug5TOeNV6gBiFeWPGFN9MuhOf23Q9Ifjh" crossorigin="anonymous">
<style type="text/css" media="screen">
    body {
        margin: 2em;
    }
    body>h1 {
        color: darkcyan;
    }
</style>
