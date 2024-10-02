# packagets

An alternative format for `package.json` files.

`packagets` watches your folder for changes to `package.ts` and uses it to generate a `package.json` file. 

`package.ts` is a Typescript file that has a default export that is used to define your package.json fields.

That's it!

## What Does It Look Like

```typescript
export default {
  scripts: {
    packagets: 'bun index.ts',
  },
  devDependencies: {
    '@types/bun': 'latest',
  },
  peerDependencies: {
    typescript: '^5.0.0',
  }
}
```

## But Why, Though

* some out of the box defaults
* comments!
* trailing commas!
* re-use common fields
* because we can

## How

Install

`bun add github:scally/packagets`
