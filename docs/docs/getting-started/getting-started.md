---
uid: getting-started
title: Getting started with bUnit
---

# Getting started with bUnit

To get started writing tests for your Blazor components, you first need to set up a test project. Then you can start writing your tests, using either C# or Razor syntax.

The sections below takes you through each of the steps you need to get started:

## Creating a test project

First you need a test project to store your component tests inside. This is covered on the <xref:create-test-project> page.

## The basics of testing Blazor components

To test a component, you first have to render it with parameters, cascading values, and services passed into it. Then, you need access to the component's instance and the markup it has produced, so you can inspect and interact with both.

There are three different ways of doing this in bUnit:

1. [**C# based tests**](/docs/csharp-based-testing.html)  
   With C# based tests, you write all your testing logic in C# files, i.e. like regular unit tests.
2. [**Razor based tests**](/docs/razor-based-testing.html)  
   With Razor based tests, you write tests in `.razor` files, which allows you to declare, in Razor syntax, the component under test and other markup fragments you need. You still write your assertions via C# in the .razor file, inside `@code {...}` blocks.
3. [**Snapshot tests**](/docs/snapshot-testing.html)  
   Snapshot tests are written in `.razor` files. A test contains a definition of an input markup/component and the expected output markup. The library will then automatically perform an semantic HTML comparison. Very little C# is needed in this, usually only to configure services.

To learn more, read the [Basics of Blazor component testing](/docs/basics-of-blazor-component-testing.html) page.

## Examples

To see examples of how to work assert and manipulate a rendered component, go to the following pages:

- [C# test examples in the sample project](https://github.com/egil/bunit/tree/master/sample/tests/Tests)
- [Razor based test examples in the sample project](https://github.com/egil/bunit/tree/master/sample/tests/RazorTestComponents)
- [Snapshot test examples in the sample project](https://github.com/egil/bunit/tree/master/sample/tests/SnapshotTests)
