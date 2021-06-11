![tspec](tspec-logo.png)

# Specification v0.1

Tspec Structured Plain Embedded Commands is a simple specification for writing text documents where some of the lines
can be interpreted and executed by a program. It can be though of a very high level programming language where you
define your own keywords and everything is comment except execution is indicated by a little star.

## Structure of a Tspec File

A Tspec file should have a `.tspec` extension although this is not strictly necessary. Contents of the file is free form
plain text except there may be one or more `steps` included. Steps are indicated by little star sign `*` (asterisk) at
the begining of every line. There may be white space before or after the sign and parsers should ignore that. If there
are no lines starting with a star sign, parsers should still treat the file as a Tspec file but not performa and actions
on it.

# Implementations

* [dotnet](https://github.com/tspec/lib-cs)
