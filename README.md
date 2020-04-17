# Lerna without yarn workspaces

```
npm install lerna -g
```

:thinking: I'd like to install this non-globally, but then: how would I use lerna inside of a package in this repo?


## Gotchas
Cannot have @scope name in the root/package.json 

## Adding a peer dependency to a package


```
lerna add react packages/two --peer
```