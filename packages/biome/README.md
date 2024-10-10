# Biome

> [Biome](https://biomejs.dev/) or biomejs is a modern toolchain in the JavaScript ecosystem, compared to eslint and prettier. We choose it because it's fast, simple and has everything we need together (formatting and linting).

### How to setup biomejs

Install biome and zhaoworks biome config

```sh
bun add @biomejs/biome @zhaoworks/biome -D
```

Create a `biome.json` file and paste the following content

```json
{
  "$schema": "https://biomejs.dev/schemas/1.8.3/schema.json",
  "extends": ["@zhaoworks/biome"]
}
```

You should use the latest biome json `$schema`.

### How to use

- Use biome CLI
- [Integrate biome in your editor](https://biomejs.dev/guides/integrate-in-editor/)

Using the CLI, there are three commands

```sh
# only runs the formatter
bun biome format --write ./path/to/execute

# only runs the linter
bun biome lint --write ./path

# runs both linter and formatter
bun biome check --write ./path
```

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
