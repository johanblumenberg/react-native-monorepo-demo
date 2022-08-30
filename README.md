# Demo of react-native setup in a monorepo

This repository demonstrates how to set up multiple `react-native` apps in the same monorepo.

## Setup

The apps are created using these commands:

```
$ mkdir apps
$ cd apps
$ npx react-native init App1
$ npx react-native init App2
```

The result can be seen in commit https://github.com/johanblumenberg/react-native-monorepo-demo/commit/4f135daead6a319c267c9ab6520051b19cca4314

## Convert to monorepo

Converting to a monorepo consists of adding a root `package.json` file having a `workspace` definition, and changing some `react-native` paths in the build scripts to point to `node_modules` in the root.

The changes can be seen in commit https://github.com/johanblumenberg/react-native-monorepo-demo/commit/df5204446abc71599867682be7dfd54444cb5328
