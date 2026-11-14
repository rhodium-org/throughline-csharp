# Microsoft C# coding conventions — throughline source

This document is **generated from the graph** by `tl docs`; `tl docs --check` gates it in CI. The prose headings are hand-owned — everything between `tl:*` markers is injected from the YAML items, so the published spec can never drift from the graph.

This source re-expresses **Microsoft's C# coding conventions** as a grounded IDD graph: each major section is a `user_requirement`, and every individual rule is a `system_requirement` that `implements` its section. The guide reference lives in `attrs.source_ref`; the throughline UIDs are this source's own and immutable — a consumer cites a rule as `csharp:SR-0001`, never by section name.

It carries
<!-- tl:count type == 'user_requirement' -->
12
<!-- tl:end --> sections and
<!-- tl:count type == 'system_requirement' -->
68
<!-- tl:end --> style rules.

## Purpose

<!-- tl:item INT-0001 -->
**INT-0001 — C# is written in one consistent, correct, readable style** — `intent`, status `proposed`

> Microsoft's C# coding conventions exist so that C# code — and the samples and documentation that teach it — reads as though written by one author: consistent naming, layout and language-feature choices that favour clarity, correctness and modern idioms, so that any developer can read, copy, change and maintain code they did not write.

**source_ref**: Microsoft C# Coding Conventions
<!-- tl:end -->

## Naming Rules

<!-- tl:item UR-0001 -->
**UR-0001 — Naming Rules** — `user_requirement`, status `proposed`

> Rules the compiler enforces for a valid identifier name.

*Derives from:* INT-0001

**source_ref**: Microsoft C# Coding Conventions: Identifiers — Naming Rules
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Microsoft C# Coding Conventions: Identifiers — Naming Rules') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0001 | system_requirement | proposed | Start every identifier with a letter or underscore |
| SR-0002 | system_requirement | proposed | Use only permitted Unicode characters in identifiers |
| SR-0003 | system_requirement | proposed | Prefix a keyword identifier with @ when unavoidable |
| SR-0004 | system_requirement | proposed | Never use two consecutive underscores in a name |
<!-- tl:end -->

## Naming Conventions

<!-- tl:item UR-0002 -->
**UR-0002 — Naming Conventions** — `user_requirement`, status `proposed`

> Conventions for the casing, prefixes and choice of identifier names.

*Derives from:* INT-0001

**source_ref**: Microsoft C# Coding Conventions: Identifiers — Naming Conventions
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Microsoft C# Coding Conventions: Identifiers — Naming Conventions') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0005 | system_requirement | proposed | Name types, namespaces and public members in PascalCase |
| SR-0006 | system_requirement | proposed | Name classes and methods in PascalCase |
| SR-0007 | system_requirement | proposed | Name parameters and local variables in camelCase |
| SR-0008 | system_requirement | proposed | Prefix private and internal non-constant fields with an underscore |
| SR-0009 | system_requirement | proposed | Prefix private or internal static fields with s_ |
| SR-0010 | system_requirement | proposed | Name all constants in PascalCase |
| SR-0011 | system_requirement | proposed | Prefix an interface name with a capital I |
| SR-0012 | system_requirement | proposed | End an attribute type name with Attribute |
| SR-0013 | system_requirement | proposed | Name enums with a singular or plural noun by flag-ness |
| SR-0014 | system_requirement | proposed | Case a record's positional parameters as public properties |
| SR-0015 | system_requirement | proposed | Use meaningful, descriptive names and prefer clarity to brevity |
| SR-0016 | system_requirement | proposed | Avoid abbreviations, acronyms and single-letter names |
| SR-0017 | system_requirement | proposed | Name namespaces in reverse domain notation |
<!-- tl:end -->

## Type Parameter Naming

<!-- tl:item UR-0003 -->
**UR-0003 — Type Parameter Naming** — `user_requirement`, status `proposed`

> Conventions for naming generic type parameters.

*Derives from:* INT-0001

**source_ref**: Microsoft C# Coding Conventions: Identifiers — Type Parameter Naming
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Microsoft C# Coding Conventions: Identifiers — Type Parameter Naming') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0018 | system_requirement | proposed | Give generic type parameters descriptive names |
| SR-0019 | system_requirement | proposed | Use T for a single self-explanatory type parameter |
| SR-0020 | system_requirement | proposed | Prefix a descriptive type-parameter name with T |
| SR-0021 | system_requirement | proposed | Encode a type parameter's constraint in its name |
<!-- tl:end -->

## General Language Guidelines

<!-- tl:item UR-0004 -->
**UR-0004 — General Language Guidelines** — `user_requirement`, status `proposed`

> Cross-cutting guidance on modern features, keywords, types and clarity.

*Derives from:* INT-0001

**source_ref**: Microsoft C# Coding Conventions: Language — General Guidelines
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Microsoft C# Coding Conventions: Language — General Guidelines') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0022 | system_requirement | proposed | Use modern language features and avoid outdated constructs |
| SR-0023 | system_requirement | proposed | Use language keyword type names, not runtime types |
| SR-0024 | system_requirement | proposed | Prefer int to unsigned types |
| SR-0025 | system_requirement | proposed | Catch only exceptions you can handle, using specific types |
| SR-0026 | system_requirement | proposed | Use async and await for I/O-bound work |
| SR-0027 | system_requirement | proposed | Write for clarity and simplicity |
<!-- tl:end -->

## Strings, Collections and Delegates

<!-- tl:item UR-0005 -->
**UR-0005 — Strings, Collections and Delegates** — `user_requirement`, status `proposed`

> Guidance on string building, collection initialisation and delegate use.

*Derives from:* INT-0001

**source_ref**: Microsoft C# Coding Conventions: Language — Strings, Collections and Delegates
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Microsoft C# Coding Conventions: Language — Strings, Collections and Delegates') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0028 | system_requirement | proposed | Concatenate short strings with interpolation |
| SR-0029 | system_requirement | proposed | Use expression-based, not positional, interpolation |
| SR-0030 | system_requirement | proposed | Build strings in loops with StringBuilder |
| SR-0031 | system_requirement | proposed | Prefer raw string literals to escapes or verbatim strings |
| SR-0032 | system_requirement | proposed | Initialise every collection with a collection expression |
| SR-0033 | system_requirement | proposed | Use Func<> and Action<> instead of custom delegate types |
| SR-0034 | system_requirement | proposed | Use the concise syntax to create a delegate instance |
<!-- tl:end -->

## Object Instantiation and Initialization

<!-- tl:item UR-0006 -->
**UR-0006 — Object Instantiation and Initialization** — `user_requirement`, status `proposed`

> Guidance on the new operator, object initializers and required properties.

*Derives from:* INT-0001

**source_ref**: Microsoft C# Coding Conventions: Language — Object Instantiation and Initialization
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Microsoft C# Coding Conventions: Language — Object Instantiation and Initialization') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0035 | system_requirement | proposed | Use a concise instantiation form when types match |
| SR-0036 | system_requirement | proposed | Use object initializers to simplify creation |
| SR-0037 | system_requirement | proposed | Force initialization with required, not constructors |
<!-- tl:end -->

## Exception Handling and Resource Management

<!-- tl:item UR-0007 -->
**UR-0007 — Exception Handling and Resource Management** — `user_requirement`, status `proposed`

> Guidance on try-catch, using statements and event handlers.

*Derives from:* INT-0001

**source_ref**: Microsoft C# Coding Conventions: Language — Exception Handling and Resource Management
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Microsoft C# Coding Conventions: Language — Exception Handling and Resource Management') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0038 | system_requirement | proposed | Use try-catch for most exception handling |
| SR-0039 | system_requirement | proposed | Replace a Dispose-only try-finally with using |
| SR-0040 | system_requirement | proposed | Prefer the braceless using declaration |
| SR-0041 | system_requirement | proposed | Use a lambda for a handler you never remove |
<!-- tl:end -->

## Implicit Typing and Operators

<!-- tl:item UR-0008 -->
**UR-0008 — Implicit Typing and Operators** — `user_requirement`, status `proposed`

> Guidance on var, conditional logical operators and static member access.

*Derives from:* INT-0001

**source_ref**: Microsoft C# Coding Conventions: Language — Implicit Typing and Operators
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Microsoft C# Coding Conventions: Language — Implicit Typing and Operators') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0042 | system_requirement | proposed | Use var only when the type is obvious from the right side |
| SR-0043 | system_requirement | proposed | Do not use var when the type is not apparent |
| SR-0044 | system_requirement | proposed | Use var for the for-loop variable, but not foreach |
| SR-0045 | system_requirement | proposed | Prefer dynamic to var for run-time type inference |
| SR-0046 | system_requirement | proposed | Use && and \|\| rather than & and \| for comparisons |
| SR-0047 | system_requirement | proposed | Qualify a static member with its own class name |
<!-- tl:end -->

## LINQ Queries

<!-- tl:item UR-0009 -->
**UR-0009 — LINQ Queries** — `user_requirement`, status `proposed`

> Guidance on writing and formatting LINQ query expressions.

*Derives from:* INT-0001

**source_ref**: Microsoft C# Coding Conventions: Language — LINQ Queries
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Microsoft C# Coding Conventions: Language — LINQ Queries') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0048 | system_requirement | proposed | Use meaningful names for query variables |
| SR-0049 | system_requirement | proposed | Alias anonymous-type members to correct Pascal casing |
| SR-0050 | system_requirement | proposed | Rename result properties that would otherwise be ambiguous |
| SR-0051 | system_requirement | proposed | Use implicit typing for query and range variables |
| SR-0052 | system_requirement | proposed | Align query clauses under the from clause |
| SR-0053 | system_requirement | proposed | Place where clauses before later clauses |
| SR-0054 | system_requirement | proposed | Access inner collections with multiple from clauses |
<!-- tl:end -->

## Namespaces and Using Directives

<!-- tl:item UR-0010 -->
**UR-0010 — Namespaces and Using Directives** — `user_requirement`, status `proposed`

> Guidance on namespace declarations and the placement of using directives.

*Derives from:* INT-0001

**source_ref**: Microsoft C# Coding Conventions: Language — Namespaces and Using Directives
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Microsoft C# Coding Conventions: Language — Namespaces and Using Directives') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0055 | system_requirement | proposed | Use a file-scoped namespace declaration |
| SR-0056 | system_requirement | proposed | Place using directives outside the namespace |
<!-- tl:end -->

## Layout Conventions

<!-- tl:item UR-0011 -->
**UR-0011 — Layout Conventions** — `user_requirement`, status `proposed`

> Conventions for indentation, line length, braces and statement layout.

*Derives from:* INT-0001

**source_ref**: Microsoft C# Coding Conventions: Style — Layout Conventions
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Microsoft C# Coding Conventions: Style — Layout Conventions') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0057 | system_requirement | proposed | Indent with four spaces, never tabs |
| SR-0058 | system_requirement | proposed | Write one statement and one declaration per line |
| SR-0059 | system_requirement | proposed | Limit lines to 65 characters |
| SR-0060 | system_requirement | proposed | Use Allman braces aligned to the indentation level |
| SR-0061 | system_requirement | proposed | Break a line before a binary operator |
| SR-0062 | system_requirement | proposed | Separate method and property definitions with a blank line |
| SR-0063 | system_requirement | proposed | Use parentheses to make expression clauses apparent |
<!-- tl:end -->

## Commenting Conventions

<!-- tl:item UR-0012 -->
**UR-0012 — Commenting Conventions** — `user_requirement`, status `proposed`

> Conventions for comment style, placement and documentation comments.

*Derives from:* INT-0001

**source_ref**: Microsoft C# Coding Conventions: Style — Commenting Conventions
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Microsoft C# Coding Conventions: Style — Commenting Conventions') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0064 | system_requirement | proposed | Use single-line comments for brief explanations |
| SR-0065 | system_requirement | proposed | Use XML documentation comments for members |
| SR-0066 | system_requirement | proposed | Place a comment on its own line, not at line end |
| SR-0067 | system_requirement | proposed | Begin a comment with a capital and end with a period |
| SR-0068 | system_requirement | proposed | Put one space after the comment delimiter |
<!-- tl:end -->

