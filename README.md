# component-trace

Search a directory and see if any of the components depend on something. It
checks the `dependencies` keys and the `local` array.

```
npm install -g component-trace
```

## Usage

```
component trace <name>
```

Example:

```
component trace component/emitter
```

Output:

```
overlay @ /apps/project/components/segmentio-overlay/component.json
toggle @ /apps/project/components/segmentio-toggle/component.json
```

## Notes

Skips `node_modules` directories.

## Why

I needed to do some refactoring. This is quicker than searching by hand.