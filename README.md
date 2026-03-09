# VHDL 20xx Just New Implementations/Features

## Documents

- [`VHDL-2008 Feature Reference`](./VHDL-2008.md)
- [`VHDL-2019 Feature Reference`](./VHDL-2019.md)

## Quick Index

| Document                                      | What it covers                                | Examples                            | Primary upstream                                               |
| --------------------------------------------- | --------------------------------------------- | ----------------------------------- | -------------------------------------------------------------- |
| [VHDL-2008 Feature Reference](./VHDL-2008.md) | VHDL-2008 language additions and improvements | Small, focused snippets per feature | IEEE P1076, VHDL-200X Fast Track proposals, Ashenden and Lewis |
| [VHDL-2019 Feature Reference](./VHDL-2019.md) | VHDL-2019 language additions and library APIs | Small, focused snippets per feature | SynthWorks VHDL_2019, IEEE P1076                               |

### VHDL-2008 sections (short list)

| Section | Topic                                                                                                                           | Description                                                    |
| ------: | ------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------- |
|       1 | [Context declarations](./VHDL-2008.md#1-context-declarations)                                                                   | Groups library/use clauses into reusable named contexts        |
|       2 | [Hierarchical or external names](./VHDL-2008.md#2-hierarchicalexternal-names)                                                   | Access signals across hierarchy without modifying RTL          |
|       3 | [process(all)](./VHDL-2008.md#3-processall)                                                                                     | Automatically infers complete sensitivity list for processes   |
|       4 | [Enhanced bit string literals](./VHDL-2008.md#4-enhanced-bit-string-literals)                                                   | Adds signed/unsigned indicators and don't-care support         |
|       5 | [Generics on packages](./VHDL-2008.md#5-generics-on-packages)                                                                   | Enables parameterizable packages for reusable components       |
|       6 | [Generic types](./VHDL-2008.md#6-generic-types)                                                                                 | Functions can work with any type using generic type parameters |
|       7 | [Array and record operations](./VHDL-2008.md#7-array-and-record-operations)                                                     | Element-wise logical operations on arrays                      |
|       8 | [Fixed and floating point packages](./VHDL-2008.md#8-fixed-and-floating-point-packages)                                         | Standard packages for fixed and floating point arithmetic      |
|       9 | [Unconstrained array elements](./VHDL-2008.md#9-unconstrained-array-elements)                                                   | Arrays can have elements with different dimensions             |
|      10 | [Read-out ports](./VHDL-2008.md#10-read-out-ports)                                                                              | Output ports can be read from within the architecture          |
|      11 | [Enhanced port association](./VHDL-2008.md#11-enhanced-port-association)                                                        | Expressions allowed directly in port maps                      |
|      12 | [Simplified sensitivity lists](./VHDL-2008.md#12-simplified-sensitivity-lists)                                                  | Automatic sensitivity inference using process(all)             |
|      13 | [Force and release](./VHDL-2008.md#13-force-and-release)                                                                        | Override signal values in testbenches for fault injection      |
|      14 | [Unary reduction operators](./VHDL-2008.md#14-unary-reduction-operators)                                                        | Reduce vectors to single bit with logical operations           |
|      15 | [Conditional and selected assignment](./VHDL-2008.md#15-conditional-and-selected-assignment)                                    | Inline conditional logic in concurrent statements              |
|      16 | [Standard vector types in std.standard](./VHDL-2008.md#16-standard-types-boolean_vector-integer_vector-real_vector-time_vector) | Predefined array types for boolean, integer, real, and time    |
|      17 | [Enhanced std_logic operators](./VHDL-2008.md#17-enhanced-std_logic-operators)                                                  | Matching operations and improved conversions                   |
|      18 | [TO_STRING and from string](./VHDL-2008.md#18-to_string-and-from-string)                                                        | Built-in string conversion for all types                       |
|      19 | [Minimum and maximum functions](./VHDL-2008.md#19-minimum-and-maximum-functions)                                                | Standard min/max functions for scalar types                    |
|      20 | [Stop and finish](./VHDL-2008.md#20-stop-and-finish)                                                                            | Control simulation termination with stop/finish procedures     |

### VHDL-2019 sections (short list)

| Section | Topic                                                                                                  | Description                                                         |
| ------: | ------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------- |
|       1 | [Conditional analysis](./VHDL-2019.md#1-conditional-analysis)                                          | Conditional compilation based on tool vendor and version            |
|       2 | [Conditional expressions and return when](./VHDL-2019.md#2-conditional-expressions--return-when)       | Early return from procedures with conditional syntax                |
|       3 | [Interface lists](./VHDL-2019.md#3-interface-lists)                                                    | Parameters can reference earlier parameters using 'Subtype          |
|       4 | [Result type functions](./VHDL-2019.md#4-result-type-functions)                                        | Functions query their return type size and bounds                   |
|       5 | [Date and time](./VHDL-2019.md#5-date-and-time)                                                        | Access system date/time with EPOCH, LOCALTIME, GMTIME functions     |
|       6 | [Environment variables](./VHDL-2019.md#6-environment-variables)                                        | Query OS environment variables with GETENV function                 |
|       7 | [Directory I/O](./VHDL-2019.md#7-directory-io)                                                         | Read and manipulate directories with DIR_OPEN and related functions |
|       8 | [File I/O extensions](./VHDL-2019.md#8-file-io-extensions)                                             | Enhanced file operations with state, seek, and position functions   |
|       9 | [File composites](./VHDL-2019.md#9-file-composites)                                                    | Arrays and records can contain file types                           |
|      10 | [Empty records](./VHDL-2019.md#10-empty-records)                                                       | Records can have no elements for token/marker types                 |
|      11 | [Function inout parameters](./VHDL-2019.md#11-function-inout-parameters)                               | Functions can have inout and protected type parameters              |
|      12 | [Range expressions](./VHDL-2019.md#12-range-expressions)                                               | Convert ranges to/from records as first-class data                  |
|      13 | [Subprogram generics](./VHDL-2019.md#13-subprogram-generics)                                           | Functions and procedures can have generic type parameters           |
|      14 | [To_string for vectors](./VHDL-2019.md#14-to_string-for-vectors)                                       | Extended to_string support for composite types                      |
|      15 | [Interfaces with unspecified types](./VHDL-2019.md#15-interfaces-with-unspecified-types)               | Generic algorithms work with any array type                         |
|      16 | [Assert API](./VHDL-2019.md#16-assert-api)                                                             | Programmatic control over assertion formatting and counters         |
|      17 | [Protected types generics](./VHDL-2019.md#17-protected-types---generics)                               | Protected types can have generic parameters                         |
|      18 | [Protected types function parameters](./VHDL-2019.md#18-protected-types---function-parameters)         | Protected types can be passed to subprograms                        |
|      19 | [Protected types arrays and scoreboards](./VHDL-2019.md#19-protected-types---arraysscoreboards)        | Protected types can be array elements                               |
|      20 | [Protected types entity ports](./VHDL-2019.md#20-protected-types---entity-ports)                       | Protected types accessible via external names                       |
|      21 | [Partially connected vectors](./VHDL-2019.md#21-partially-connected-vectors)                           | Individual vector elements can be left unconnected                  |
|      22 | [Sequential declaration regions](./VHDL-2019.md#22-sequential-declaration-regions)                     | Block statements with local declarations in processes               |
|      23 | [Report calling path](./VHDL-2019.md#23-report-calling-path)                                           | GET_CALL_PATH function returns call stack information               |
|      24 | [Anonymous types](./VHDL-2019.md#24-anonymous-types)                                                   | Ports and generics can use inline type declarations                 |
|      25 | [Enhanced enumeration attributes](./VHDL-2019.md#25-enhanced-enumeration-attributes)                   | Object-level shorthand for IMAGE, POS, SUCC, PRED                   |
|      26 | [Inferred constraints from initial values](./VHDL-2019.md#26-inferred-constraints-from-initial-values) | Array bounds inferred from initialization                           |
|      27 | [64-bit integer support](./VHDL-2019.md#27-64-bit-integer-support)                                     | Extended integer range for 64-bit operations                        |
