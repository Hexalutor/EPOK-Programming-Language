EPOK BONSAI MINI 1.0

Release Date: October 27, 2026

Created by: Hexalutor

Commit: SERISSA


===================
WHAT IS EPOK?

EPOK is a lightweight interpreted programming language
focused on simplicity, numerical computing, education,
and arbitrary precision arithmetic.

The language includes a custom lexer, parser,
type checker, virtual machine, REPL, import/export
system, arrays, matrices, BigInt support and BigFloat
support.


===================
DISCLAIMER

EPOK is still under active development.

Although the core language is stable and extensively
tested, bugs may still exist.

Unexpected runtime errors, parser edge cases,
unhandled exceptions, semantic inconsistencies and
uncovered NoneType situations are still possible.

If something crashes, behaves incorrectly or produces
an unclear error message, assume it may be a language
bug.


===================
FEATURES

- Variables
- Constants
- Functions
- Recursion
- Modules
- Import / Export
- REPL

Control Flow

- if
- elif
- else
- while
- for

Types

- bool
- int
- float
- string
- bigint
- bigfloat

Collections

- arrays
- matrices

Operators

+
-
*
/
%
**

+=
-=
*=
/=
%=
**=


===================
ARBITRARY PRECISION

bigint (1000)

bigfloat (1000)

EPOK supports arbitrary precision integers and
floating-point values.


===================
RUNNING EPOK

Start REPL:

epok.exe

Execute a file:

epok.exe hello.epok

Show version:

epok.exe --version


===================
COMPLETE EXAMPLE


epok main {

const LIMIT = 5

int counter = 0

print("EPOK Showcase\n")

while counter < LIMIT:

    print counter

    counter += 1

end

int power = 2

power *= 5

print power

print 2 ** 8

print sqrt(25)

print qbrt(27)

print pow(2, 10)

print strlen("hello")

print strcat(
    "EPOK ",
    "1.0"
)

print substr(
    "showcase",
    0,
    4
)

print pi

array int numbers

new array int 3 = numbers

numbers[0] = 10
numbers[1] = 20
numbers[2] = 30

print numbers[0]
print numbers[1]
print numbers[2]

matrix int mat

new matrix int 2 2 = mat

at mat 0 0 = 1
at mat 0 1 = 2

print at mat 0 0
print at mat 0 1

def factorial(int n) -> int:

    if n == 0:
        return 1
    end

    return n * factorial(
        n - 1
    )

end

print factorial(5)

for i from 1 to 3:

    print i

end

bigint (100) huge

huge = 999999999999999999999999999999999999

print huge

bigfloat (50) bf

bf = 1

bf = bf / 3

print bf

}

===================
STATUS

Stable core release.

Implemented:

- Lexer
- Parser
- Type Checker
- IR Generator
- Virtual Machine
- REPL
- Arrays
- Matrices
- Import / Export
- BigInt
- BigFloat
- Arbitrary Precision
- Numeric Promotion
- Compound Assignment Operators
- Exponentiation Operator (**)

710+ automated tests passing.


===================
PLANNED FEATURES

- Closure support
- Lambda support
- Python Bridge