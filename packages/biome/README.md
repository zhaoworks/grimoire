# Biome

> [Biome](https://biomejs.dev/) or biomejs is a modern toolchain in the JavaScript ecosystem, compared to eslint and prettier. We choose it because it's fast, simple and has everything we need together (formatting and linting).

### Formatter

Basic options

- Indent size: 2

The main JavaScript options

- Semicolons: always
- Quote style: single
- JSX quote style: double

### Linter rules

Biome has a few categories of linting rules which you can see at the [linter rules](https://biomejs.dev/linter/rules/) page.

We are using the recommended rules and some others that are listed below.

All the rules below are set to `error`.

#### Complexity

- [useSimplifiedLogicExpression](https://biomejs.dev/linter/rules/use-simplified-logic-expression/)

#### Correctness

- [noUnusedImports](https://biomejs.dev/linter/rules/no-unused-imports/)

#### Style

- [noNegationElse](https://biomejs.dev/linter/rules/no-negation-else)
- [noDefaultExport](https://biomejs.dev/linter/rules/no-default-export/)
- [useCollapsedElseIf](https://biomejs.dev/linter/rules/use-collapsed-else-if/)
- [useShorthandArrayType](https://biomejs.dev/linter/rules/use-shorthand-array-type/)
- [useShorthandAssign](https://biomejs.dev/linter/rules/use-shorthand-assign/)
- [useForOf](https://biomejs.dev/linter/rules/use-for-of/)
- [useFilenamingConvention](https://biomejs.dev/linter/rules/use-filenaming-convention/) - `kebab-case` and `export`

#### Suspicious

- [noEmptyBlockStatements](https://biomejs.dev/linter/rules/no-empty-block-statements/)
- [useAwait](https://biomejs.dev/linter/rules/use-await/)
