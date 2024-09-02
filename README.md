# Grimoire

> This is the zhaoworks code style and best practices repository. Here you will find the code style decisions, guides on how to setup tools and more.

## Packages

- [Biome](packages/biome/README.md)

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
