# Nyx Programming Language Specification

This repository hosts the specification for the Nyx Programming Language.

## Contents

- [Introduction]("#introduction")
- [Appendix A: Grammar]("./grammar.md")

## Introduction

This specification defines the Nyx Programming Language.

Nyx is inspired by several technologies, including but not limited to Python, Ruby, Scheme, Swift, Rust, the ML family of functional languages, JavaScript, and Julia.

Its features include first-class functions and closures, static type checking and inference, arbitrary-precision decimal numbers, a combination of prototypal and class-based objects, algebraic data types, and hygienic macros.

It is designed for use in both browser and server-side environments and interoperativity with the JavaScript language and libraries.

This specification focuses on *what the language does* more than *how the interpreter does it*. Where this specification and the actual behavior of the interpreter differ, the specification should be seen as the goal for implementation in the interpreter (and presumably the interpreter should eventually be updated to match the specification). We've tried to be reasonably precise in this document, but we'll err on the side of readability over exact technical correctness.