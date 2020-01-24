# Typescript.tools

##### Collection of resources related to Typescript internals.

<br/>

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

5. [Typescript API Playground](https://typescript-api-playground.glitch.me/) - Great live examples on how to consume a custom transformer end-to-end on the browser. Very useful for building interactive ts tools that run on the browser. It shows how to create a virtual source file from input raw string, run transformers on it and then emits the result to string and shows it on the page.

6. [Compiler API through Deno](https://deno.land/std/manual.md#compiler-api) - Deno is a new secure runtime for JavaScript and TypeScript. It allows runtime access to the built in TypeScript compiler.

## Wrappers and utils

1. [ts-morph](https://github.com/dsherret/ts-morph) - Easier and nicer abstraction layer on top of TS internals. Exposes underlying constructs for advanced usecases.

   _Slower startup due to extra initial overhead._

2. [byots](https://github.com/basarat/byots) - Modified version of Typescript lib, which exposes more internal apis. Matching releases are created automatically.

   _TS has anyway opened up more apis, is it worth using anymore ??_

3. [ttypescript](https://github.com/cevek/ttypescript) - TSC drop-in replacement which supports passing custom transformers as cmdline argument.

## Tools built using it

1. Typescript language service plugin in VS Code (inbuilt), [atom](https://github.com/TypeStrong/atom-typescript), [Sublime Text](https://github.com/Microsoft/TypeScript-Sublime-Plugin) - Supports similar feature set in multiple editors

2. [Typedoc](https://typedoc.org/) - Very popular Typescript documentation generator which extracts type definitions and inline jsdoc comments into separate documents.

3. (shameless plug) [webpack-strip-log-loader](https://github.com/bendtherules/webpack-strip-log-loader) - webpack plugin to remove some module (or symbol) and their usages recursively in a project. Uses TSC api internally.

<title>Collection of resources related to Typescript internals</title>
<link rel="icon" href="favicon.ico" type="image/x-icon" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/css/bootstrap.min.css" integrity="sha384-Vkoo8x4CGsO3+Hhxv8T/Q5PaXtkKtu6ug5TOeNV6gBiFeWPGFN9MuhOf23Q9Ifjh" crossorigin="anonymous">
<style type="text/css" media="screen">
  body {
      padding: 1em;
      max-width: 960px;
      margin: auto;
  }
  body>h1 {
      color: darkcyan;
      margin-bottom: 0.5em;
  }
  h1, h2 {
  padding-bottom: .3em;
  border-bottom: 1px solid #eaecef;
  }
</style>
