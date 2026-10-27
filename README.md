# EPOK

EPOK is an experimental general-purpose programming language built entirely from scratch.

The project was created as a long-term exploration of programming language design, interpreters, type systems, virtual machines and arbitrary-precision arithmetic. Rather than being built on top of an existing language runtime, EPOK implements its own lexer, parser, type checker, intermediate representation generator and virtual machine.

The language aims to remain simple, readable and educational while providing features usually found in significantly larger projects.

Current capabilities include:

- Variables and constants
- Functions and recursion
- Nested functions
- Static type checking
- Arrays
- Matrices
- Import / Export system
- Interactive REPL
- BigInt arbitrary-precision integers
- BigFloat arbitrary-precision floating point numbers
- Built-in mathematical library
- Built-in string manipulation library
- Compound assignment operators
- Bitwise operations
- Custom virtual machine execution

EPOK currently supports:

```text
bool
int
float
string
bigint
bigfloat
```

as well as:

```text
if
else
while
for
break
continue
```

and the following arithmetic operators:

```text
+
-
*
/
%
**
```

The language also provides built-in support for:

```text
sin
cos
tan
arcsin
arccos
arctan
sqrt
qbrt
pow
ln
log
fact
mean
median
variance
strlen
strcat
substr
```

and mathematical constants:

```text
pi
e
phi
```

## Example

```epok
epok main {

    const LIMIT = 5

    int counter = 0

    while counter < LIMIT:

        print counter

        counter += 1

    end

}
```

## Usage

Start the interactive REPL:

```bash
epok.exe
```

Execute a source file:

```bash
epok.exe file.epok
```

Display version information:

```bash
epok.exe --version
```

Exit the REPL:

```text
:quit
```

## Stability

EPOK has been extensively tested and currently includes more than 700 automated tests.

Despite this, the language is still under active development and bugs may exist. Parser edge cases, runtime issues, unhandled exceptions and uncovered `NoneType` situations are still possible.

## Current Release

Public Version:

```text
EPOK Bonsai Mini 1.0
```

Codename:

```text
SERISSA
```

Release Date:

```text
October 27, 2026
```

Internal Version:

```text
0.3.8.0
```

Current issues:

```text
BIGFLOAT and BIGINT

bigfloat precision appears capped around 28 digits.
Possible Decimal context precision issue.
```

## License

GNU GPL v3.0
