# Bun

## Quickstart

```bash
    bun init
    bun run index.ts
```

```js
console.log("Hello via Bun!");

const server = Bun.serve({
    port: 3000,
    fetch(req) {
        return new Response("Bun!");
    }
});

console.log(`Listening on http://localhost:${server.port}...`);
```

```bash
    bun run index.ts
```

```json
{
  "name": "quickstart",
  "module": "index.ts",
  "type": "module",
  "scripts": {
    "start": "bun run index.ts"
  },
  "devDependencies": {
    "bun-types": "^0.7.0"
  }
}
```

```bash
    bun run start

    # 
```

## Install a package

```bash
    bun add figlet
    bun add -d @types/figlet # TypeScript users only
```

```bash
bun add -d bun-types 
```