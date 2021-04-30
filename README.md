# Nyx Programming Language Specification

This repository hosts the specification for the Nyx Programming Language.

## Contents

- [Introduction]("#introduction")
- [Appendix A: Grammar]("./grammar.md")

## Introduction

This specification defines the Nyx Programming Language.

Nyx is inspired by several technologies, including but not limited to Python, Ruby, Scheme, Swift, Rust, the ML family of functional languages, JavaScript, and Julia.

Its features include first-class functions and closures, static type checking and inference, arbitrary-precision decimal numbers for use in scientific and technical computing, Unicode-aware textual data, a combination of prototypal and class-based objects, algebraic data types, both mutable and immutable data structures, and hygienic macros. This combination allows you to implement programs for virtually any problem domain in a dynamic fashion, with the advantages of both dynamic and static languages at your disposal.

It is designed for use in both browser and server-side environments and interoperativity with the JavaScript language and libraries.

This specification focuses on *what the language does* more than *how the interpreter does it*. Where this specification and the actual behavior of the interpreter differ, the specification should be seen as the goal for implementation in the interpreter (and presumably the interpreter should eventually be updated to match the specification). We've tried to be reasonably precise in this document, but we'll err on the side of readability over exact technical correctness.

## About Nyx

Nyx is a multi-paradigm language, including aspects of functional, object-oriented, and imperative programming. The emphasis is on expressiveness and ease of use, though performance is also a consideration.

Nyx performs computations on data objects within a host environment, which includes the interpreter itself, any runtime objects, and facilities for interacting with operating system, browser, and other system functionalities. A data object is not necessarily the same thing as an object in object-oriented programming, although all values in Nyx can be manipulated as objects with their own internal state information and a set of bundled operations for interacting with and manipulating that information. This document specifies the facilities of the language itself without specifying requirements for a host environment except to indicate certain properties and functionalities the host environment may be required to expose to Nyx in order for the language to interact with it.
